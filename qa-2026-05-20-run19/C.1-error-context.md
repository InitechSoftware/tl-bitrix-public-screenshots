# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: C.1-inbound-creates-activity.spec.ts >> C.1 — inbound WA message → CRM Activity with TLAI_WHATSAPP custom type
- Location: tests\e2e-playwright\specs\C.1-inbound-creates-activity.spec.ts:80:1

# Error details

```
Error: no TimelinesAI WhatsApp activity created within 60s (checked PROVIDER_TYPE_ID=TLAI_WHATSAPP and SUBJECT prefix "WhatsApp · ")

expect(received).toBeTruthy()

Received: undefined
```

# Test source

```ts
  38  |  * End-to-end flow:
  39  |  *   1. Fire an inbound message via `sendInbound()` — POSTs the +44 token to
  40  |  *      send +44 → +37, returning the message_uid.
  41  |  *   2. Poll the integration's `sdk_events` table for a
  42  |  *      `message:received:new` row containing that text.
  43  |  *   3. Poll Bitrix `crm.activity.list` (via webhook) for an activity
  44  |  *      matching EITHER shape (a) or (b).
  45  |  *   4. Screenshot the Deal/Contact timeline.
  46  |  */
  47  | 
  48  | import { test, expect } from '@playwright/test';
  49  | import { pinScreenshot } from '../screenshot-helper.js';
  50  | import { sendInbound } from '../lib/sendInbound.js';
  51  | import { getLatestSdkEvent } from '../lib/reset.js';
  52  | 
  53  | interface BitrixActivityRow {
  54  |   ID?: string | number;
  55  |   PROVIDER_ID?: string;
  56  |   PROVIDER_TYPE_ID?: string;
  57  |   SUBJECT?: string;
  58  |   TYPE_ID?: string | number;
  59  |   CREATED?: string;
  60  | }
  61  | 
  62  | /**
  63  |  * Identify a TimelinesAI WhatsApp card under either production shape:
  64  |  *
  65  |  *   (a) plain-activity path (#77/#104) — PROVIDER_TYPE_ID='TLAI_WHATSAPP'.
  66  |  *   (b) configurable-activity path (#164/#167, the default since 2026-05-15)
  67  |  *       — SUBJECT starts with `WhatsApp · ` (the buildActivitySubject
  68  |  *       header). The configurable path doesn't expose its `typeId` on
  69  |  *       `crm.activity.list`, but SUBJECT is byte-identical to the
  70  |  *       rendered card header and is uniquely ours.
  71  |  */
  72  | function isTlaiWhatsappActivity(row: BitrixActivityRow): boolean {
  73  |   if (row.PROVIDER_TYPE_ID === 'TLAI_WHATSAPP') return true;
  74  |   if (typeof row.SUBJECT === 'string' && row.SUBJECT.startsWith('WhatsApp · ')) {
  75  |     return true;
  76  |   }
  77  |   return false;
  78  | }
  79  | 
  80  | test('C.1 — inbound WA message → CRM Activity with TLAI_WHATSAPP custom type', async ({
  81  |   page,
  82  |   request,
  83  | }, testInfo) => {
  84  |   const portal = process.env.BITRIX_PORTAL_URL;
  85  |   const webhook = process.env.BITRIX_WEBHOOK_URL;
  86  |   const contactId = process.env.E2E_BITRIX_TEST_CONTACT_ID;
  87  | 
  88  |   test.skip(
  89  |     !portal || !webhook || !contactId,
  90  |     'Set BITRIX_PORTAL_URL, BITRIX_WEBHOOK_URL, E2E_BITRIX_TEST_CONTACT_ID to run.',
  91  |   );
  92  | 
  93  |   // 1. Trigger inbound via TL Public API double-token (Recipe 6).
  94  |   const runId = new Date().toISOString();
  95  |   const text = `06-inbound-test ${runId}`;
  96  |   const { messageUid } = await sendInbound({
  97  |     from: '+447441447478',
  98  |     to: '+37122455329',
  99  |     text,
  100 |   });
  101 |   testInfo.annotations.push({
  102 |     type: 'inbound-uid',
  103 |     description: `messageUid=${messageUid} text="${text}"`,
  104 |   });
  105 | 
  106 |   // 2. Wait for the webhook to land. Poll sdk_events up to 30s.
  107 |   let receivedText = '';
  108 |   for (let attempt = 0; attempt < 30; attempt++) {
  109 |     const evt = await getLatestSdkEvent('received');
  110 |     if (evt && evt.text === text) {
  111 |       receivedText = evt.text;
  112 |       break;
  113 |     }
  114 |     await page.waitForTimeout(1_000);
  115 |   }
  116 |   expect(receivedText, 'sdk_events did not record inbound within 30s').toBe(text);
  117 | 
  118 |   // 3. Poll Bitrix for a TimelinesAI WhatsApp activity on the test contact.
  119 |   // Accepts EITHER production shape — see `isTlaiWhatsappActivity` above for
  120 |   // why both (a) and (b) need to match.
  121 |   let activity: BitrixActivityRow | undefined;
  122 |   for (let attempt = 0; attempt < 30; attempt++) {
  123 |     const res = await request.get(`${webhook}/crm.activity.list`, {
  124 |       params: {
  125 |         'filter[OWNER_TYPE_ID]': '3', // Contact
  126 |         'filter[OWNER_ID]': contactId!,
  127 |         'order[CREATED]': 'DESC',
  128 |       },
  129 |     });
  130 |     const body = (await res.json()) as { result?: BitrixActivityRow[] };
  131 |     activity = (body.result ?? []).find(isTlaiWhatsappActivity);
  132 |     if (activity) break;
  133 |     await page.waitForTimeout(2_000);
  134 |   }
  135 |   expect(
  136 |     activity,
  137 |     'no TimelinesAI WhatsApp activity created within 60s (checked PROVIDER_TYPE_ID=TLAI_WHATSAPP and SUBJECT prefix "WhatsApp · ")',
> 138 |   ).toBeTruthy();
      |     ^ Error: no TimelinesAI WhatsApp activity created within 60s (checked PROVIDER_TYPE_ID=TLAI_WHATSAPP and SUBJECT prefix "WhatsApp · ")
  139 |   testInfo.annotations.push({
  140 |     type: 'matched-activity',
  141 |     description: `id=${activity?.ID} provider_id=${activity?.PROVIDER_ID ?? '<none>'} provider_type_id=${activity?.PROVIDER_TYPE_ID ?? '<none>'} subject="${activity?.SUBJECT ?? ''}"`,
  142 |   });
  143 | 
  144 |   // 4. UI screenshot.
  145 |   await page.goto(`${portal}/crm/contact/details/${contactId}/`);
  146 |   await page.waitForTimeout(3_000);
  147 |   await pinScreenshot(page, 'contact-timeline-with-tlai-activity', testInfo);
  148 | });
  149 | 
```