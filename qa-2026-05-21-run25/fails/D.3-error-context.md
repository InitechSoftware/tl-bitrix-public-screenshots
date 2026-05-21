# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: D.3-settings-pipeline-mapping.spec.ts >> D.3 — changing pipeline mapping routes new Deals to selected pipeline
- Location: tests\e2e-playwright\specs\D.3-settings-pipeline-mapping.spec.ts:173:1

# Error details

```
Error: Expected a NEW Deal on Contact 1 (ID>1) after inbound; none appeared within 60s. afterMaxId=1

expect(received).toBeTruthy()

Received: undefined
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - group [ref=e2]
  - dialog "WhatsApp settings" [ref=e6]:
    - iframe [active] [ref=e9]:
      - iframe [active] [ref=f1e7]:
        - generic [active] [ref=f2e1]: TimelinesAI connector settings. Open this view through your Bitrix24 portal.
    - generic:
      - button "Close" [ref=e10] [cursor=pointer]:
        - generic "Close" [ref=e11]
      - generic:
        - button "Copy link" [ref=e13] [cursor=pointer]:
          - generic "Copy link" [ref=e14]
        - button "Open in a new window" [ref=e16] [cursor=pointer]:
          - generic "Open in a new window" [ref=e17]
        - button "Print":
          - generic "Print"
  - generic [ref=e19]:
    - navigation "Main menu" [ref=e21]:
      - button "Expand menu" [ref=e24] [cursor=pointer]
      - generic [ref=e26]:
        - generic [ref=e27]:
          - list [ref=e28]:
            - listitem [ref=e29]:
              - button "Collaboration" [expanded] [ref=e30] [cursor=pointer]
            - listitem [ref=e33]:
              - list [ref=e34]:
                - listitem [ref=e35]:
                  - link "Messenger, 1 new" [ref=e36] [cursor=pointer]:
                    - /url: /online/
                    - generic [ref=e42]: "1"
                - listitem [ref=e45]:
                  - link "Collabs" [ref=e46] [cursor=pointer]:
                    - /url: /online/?IM_COLLAB
                - listitem [ref=e51]:
                  - link "Feed" [ref=e52] [cursor=pointer]:
                    - /url: /stream/
                - listitem [ref=e57]:
                  - link:
                    - /url: /company/personal/user/1/calendar/?EVENT_ID=NEW
                  - link "Calendar" [ref=e58] [cursor=pointer]:
                    - /url: /company/personal/user/1/calendar/
                - listitem [ref=e63]:
                  - link "Documents" [ref=e64] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/documents/?st[tool]=docs&st[category]=docs&st[event]=open_section&st[c_section]=left_menu
                - listitem [ref=e69]:
                  - link "Boards" [ref=e70] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/boards/?c_section=left_menu
                - listitem [ref=e75]:
                  - link "Drive" [ref=e76] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/path/
                - listitem [ref=e81]:
                  - link "Webmail" [ref=e82] [cursor=pointer]:
                    - /url: /mail/?source=left_menu
                - listitem [ref=e87]:
                  - link:
                    - /url: /company/personal/user/1/groups/create/
                  - link "Workgroups" [ref=e88] [cursor=pointer]:
                    - /url: /workgroups/
            - listitem [ref=e93]:
              - link:
                - /url: /company/personal/user/1/tasks/task/edit/0/?ta_sec=tasks&ta_el=left_menu&miniform=true
              - link "Tasks and Projects" [ref=e94] [cursor=pointer]:
                - /url: /company/personal/user/1/tasks/?ta_sec=left_menu
            - listitem [ref=e99]:
              - link "CRM, 2 new" [ref=e100] [cursor=pointer]:
                - /url: /crm/deal/?redirect_to
                - generic [ref=e106]: "2"
            - listitem [ref=e109]:
              - link "Booking" [ref=e110] [cursor=pointer]:
                - /url: /booking/
            - listitem [ref=e115]:
              - link "Inventory management" [ref=e116] [cursor=pointer]:
                - /url: /shop/documents/inventory/
            - listitem [ref=e121]:
              - link "Marketing" [ref=e122] [cursor=pointer]:
                - /url: /marketing/
            - listitem [ref=e127]:
              - link "Sites and stores" [ref=e128] [cursor=pointer]:
                - /url: /sites/
            - listitem [ref=e133]:
              - link "e-Signature for HR" [ref=e134] [cursor=pointer]:
                - /url: /sign/b2e/
            - listitem [ref=e139]:
              - link "e-Signature" [ref=e140] [cursor=pointer]:
                - /url: /sign/
            - listitem [ref=e145]:
              - link "BI Builder" [ref=e146] [cursor=pointer]:
                - /url: /bi/dashboard
            - listitem [ref=e151]:
              - link "Employees" [ref=e152] [cursor=pointer]:
                - /url: /company/
            - listitem [ref=e157]:
              - link "Automation" [ref=e158] [cursor=pointer]:
                - /url: /bizproc/userprocesses/
            - listitem [ref=e163]:
              - button "Applications" [expanded] [ref=e164] [cursor=pointer]
            - listitem [ref=e167]:
              - list [ref=e168]:
                - listitem [ref=e169]:
                  - link "Market" [ref=e170] [cursor=pointer]:
                    - /url: /market/
                - listitem [ref=e175]:
                  - link "Developer resources" [ref=e176] [cursor=pointer]:
                    - /url: /devops/
                - listitem [ref=e181]:
                  - link "MCP connections" [ref=e182] [cursor=pointer]:
                    - /url: /mcp/
                - listitem [ref=e187]:
                  - link "WhatsApp integration by TimelinesAI" [ref=e188] [cursor=pointer]:
                    - /url: /marketplace/app/1/
                    - generic [ref=e190]: WI
                - listitem [ref=e193]:
                  - link "WhatsApp audit log" [ref=e194] [cursor=pointer]:
                    - /url: /devops/placement/733/
                    - generic [ref=e196]: WA
                - listitem [ref=e199]:
                  - link "WhatsApp settings" [ref=e200] [cursor=pointer]:
                    - /url: /devops/placement/735/
                    - generic [ref=e202]: WS
          - list [ref=e205]:
            - listitem [ref=e206] [cursor=pointer]
            - listitem [ref=e209]:
              - link "Subscription" [ref=e210] [cursor=pointer]:
                - /url: /settings/license.php?TARIFF_WIDGET=Y
        - button "Show all" [ref=e215]
      - generic [ref=e220]:
        - button [ref=e221]
        - button "Upgrade your plan" [ref=e226] [cursor=pointer]:
          - generic:
            - generic: Upgrade your plan
    - banner [ref=e228]:
      - generic [ref=e229]:
        - navigation [ref=e231]:
          - list [ref=e232]:
            - listitem [ref=e233]:
              - button "Chats 1" [ref=e234] [cursor=pointer]:
                - generic [ref=e237]: Chats
                - generic [ref=e238]: "1"
            - listitem [ref=e239]:
              - button "Task chats" [ref=e240] [cursor=pointer]:
                - generic [ref=e243]: Task chats
            - listitem [ref=e244]:
              - button "CoPilot" [ref=e245] [cursor=pointer]:
                - generic [ref=e248]: CoPilot
            - listitem [ref=e249]:
              - button "Collabs" [ref=e250] [cursor=pointer]:
                - generic [ref=e253]: Collabs
            - listitem [ref=e254]:
              - button "Channels" [ref=e255] [cursor=pointer]:
                - generic [ref=e258]: Channels
            - listitem [ref=e259]:
              - button "Contact Center" [ref=e260] [cursor=pointer]:
                - generic [ref=e263]: Contact Center
            - listitem [ref=e264]:
              - button "More 9" [ref=e265] [cursor=pointer]:
                - generic [ref=e268]: More
                - generic [ref=e270]: "9"
        - generic [ref=e271]:
          - search [ref=e274]:
            - textbox [disabled] [ref=e275]:
              - /placeholder: find people, documents, and more
            - button "Search" [ref=e276]
          - link "Bitrix 24" [ref=e280] [cursor=pointer]:
            - /url: /
            - generic [ref=e281]:
              - generic [ref=e282]: Bitrix
              - generic [ref=e283]: "24"
          - button [ref=e284] [cursor=pointer]
          - generic [ref=e286]:
            - button "Invite" [ref=e288] [cursor=pointer]: Invite
            - button "Buy Now" [ref=e290] [cursor=pointer]: Buy Now
            - button "Helpdesk 6" [ref=e292] [cursor=pointer]:
              - text: Helpdesk
              - generic [ref=e296]: "6"
    - button "Profile" [ref=e297] [cursor=pointer]
    - main [ref=e303]:
      - generic [ref=e310]:
        - generic [ref=e312]:
          - generic [ref=e313]:
            - button [ref=e314] [cursor=pointer]
            - textbox "Find employee or chat" [ref=e319]
          - generic [ref=e326]:
            - generic [ref=e328] [cursor=pointer]:
              - generic "General chat" [ref=e331]
              - generic [ref=e333]:
                - generic [ref=e334]:
                  - generic "General chat" [ref=e337]
                  - generic [ref=e339]: May 17
                - generic [ref=e342]: Anton Patrai granted administrator permissions to WhatsApp integration by TimelinesAI.
            - generic [ref=e345] [cursor=pointer]:
              - generic "Bitrix24 Support" [ref=e348]:
                - img "Bitrix24 Support" [ref=e349]
              - generic [ref=e350]:
                - generic [ref=e351]:
                  - generic "Bitrix24 Support" [ref=e355]
                  - generic [ref=e357]: May 12
                - generic [ref=e358]:
                  - generic [ref=e360]: "👋 Hi there! I’m your Bitrix24 assistant. I can help you: • Build your CRM in minutes • Create smart automations • Launch a chat, site, or project • Or just find the right button when you’re stuck! Ask away — I’m online 24/7 or learn more 👉 here. [Attachment]"
                  - generic [ref=e364]: "1"
            - generic [ref=e366] [cursor=pointer]:
              - generic "Company News" [ref=e369]
              - generic [ref=e371]:
                - generic [ref=e372]:
                  - generic "Company News" [ref=e375]
                  - generic [ref=e377]: May 12
                - generic [ref=e380]: Share important information and news. Follow to remain informed about the latest developments. Leave comments and discuss posts.
            - generic [ref=e383] [cursor=pointer]:
              - generic "My Notes" [ref=e386]
              - generic [ref=e387]:
                - generic [ref=e388]:
                  - generic "Notes" [ref=e391]
                  - generic [ref=e393]: May 12
                - generic [ref=e396]: Visible to you only
        - generic [ref=e400]:
          - generic [ref=e402]: Select a chat to start communicating
          - generic [ref=e403]: or
          - generic [ref=e404] [cursor=pointer]: Invite users
  - generic:
    - generic:
      - generic:
        - generic: The server connection is successfully established
  - dialog [ref=e405]:
    - generic [ref=e409]:
      - generic [ref=e410]:
        - heading "Invite sales representatives" [level=4] [ref=e411]
        - text: Learn Bitrix24 CRM features and start selling in no time.
      - button "User invitation" [ref=e412] [cursor=pointer]:
        - generic [ref=e413]: User invitation
    - button "Close" [ref=e414] [cursor=pointer]
```

# Test source

```ts
  246 |   // + non-fatal — the pipeline assertion below remains the oracle.
  247 |   const warm = await warmBitrixContext();
  248 |   testInfo.annotations.push({ type: 'bitrix-warmup', description: warm.detail });
  249 | 
  250 |   // #596 — pre-close Contact 1's OPEN deals so the matcher
  251 |   // (`maybeCreateDealForOnlyClosed`) creates a FRESH deal in the configured
  252 |   // pipeline on the inbound below. Without this, the Sarah-Johnson fixture's
  253 |   // pre-existing open category-0 deal suppresses the create and the assertion
  254 |   // reads a stale deal. Idempotent — re-runs find nothing left to close.
  255 |   const closedDealIds = await preCloseContactOpenDeals(
  256 |     request,
  257 |     webhook!,
  258 |     TEST_CONTACT_ID,
  259 |   );
  260 |   testInfo.annotations.push({
  261 |     type: 'pre-closed-deals',
  262 |     description: `contact=${TEST_CONTACT_ID} closed=[${closedDealIds.join(',')}]`,
  263 |   });
  264 | 
  265 |   // Baseline the max deal ID on Contact 1 BEFORE the inbound, so we can
  266 |   // correlate to the deal THIS run creates (ID > baseline) rather than
  267 |   // asserting on "newest deal overall".
  268 |   const dealsBeforeRes = await request.get(`${webhook}/crm.deal.list`, {
  269 |     params: {
  270 |       'filter[CONTACT_ID]': TEST_CONTACT_ID,
  271 |       'select[0]': 'ID',
  272 |       'order[ID]': 'DESC',
  273 |       start: 0,
  274 |     },
  275 |   });
  276 |   const dealsBefore =
  277 |     ((await dealsBeforeRes.json()) as { result?: DealRow[] }).result ?? [];
  278 |   const baselineMaxId = maxDealId(dealsBefore);
  279 |   testInfo.annotations.push({
  280 |     type: 'baseline-deal-id',
  281 |     description: `baselineMaxId=${baselineMaxId} pageCount=${dealsBefore.length}`,
  282 |   });
  283 | 
  284 |   // Fire inbound.
  285 |   const runId = new Date().toISOString();
  286 |   const text = `09-pipeline-mapping ${runId}`;
  287 |   const { messageUid } = await sendInbound({
  288 |     from: '+447441447478',
  289 |     to: '+37122455329',
  290 |     text,
  291 |   });
  292 |   testInfo.annotations.push({ type: 'inbound-uid', description: messageUid });
  293 | 
  294 |   // Wait for webhook.
  295 |   let received = false;
  296 |   for (let attempt = 0; attempt < 30; attempt++) {
  297 |     const evt = await getLatestSdkEvent('received');
  298 |     if (evt && evt.text === text) {
  299 |       received = true;
  300 |       break;
  301 |     }
  302 |     await page.waitForTimeout(1_000);
  303 |   }
  304 |   expect(received).toBe(true);
  305 | 
  306 |   // Poll Contact 1's deals for the one THIS run created (ID > baseline).
  307 |   // 30 × 2s = 60s ceiling — matches D.2's deal poll, since
  308 |   // `inbound webhook → sdk_events processor → matcher → crm.deal.add` is not
  309 |   // bounded by a flat 10s wait (an interleaving Bitrix token refresh can
  310 |   // stretch it; see C.1 #549 / D.2 #546 for the same class of bug).
  311 |   let runDeal: DealRow | undefined;
  312 |   let lastAfterPage: DealRow[] = [];
  313 |   for (let attempt = 0; attempt < 30; attempt++) {
  314 |     const dealsAfterRes = await request.get(`${webhook}/crm.deal.list`, {
  315 |       params: {
  316 |         'filter[CONTACT_ID]': TEST_CONTACT_ID,
  317 |         'select[0]': 'ID',
  318 |         'select[1]': 'CATEGORY_ID',
  319 |         'select[2]': 'DATE_CREATE',
  320 |         'order[ID]': 'DESC',
  321 |         start: 0,
  322 |       },
  323 |     });
  324 |     lastAfterPage =
  325 |       ((await dealsAfterRes.json()) as { result?: DealRow[] }).result ?? [];
  326 |     // Newest deal on the contact that didn't exist at baseline time.
  327 |     runDeal = lastAfterPage.find((d) => Number(d.ID) > baselineMaxId);
  328 |     if (runDeal) break;
  329 |     await page.waitForTimeout(2_000);
  330 |   }
  331 |   testInfo.annotations.push({
  332 |     type: 'after-deal-page',
  333 |     description:
  334 |       `afterMaxId=${maxDealId(lastAfterPage)} pageCount=${lastAfterPage.length} ` +
  335 |       `top5=${lastAfterPage
  336 |         .slice(0, 5)
  337 |         .map((r) => `${r.ID}:cat${r.CATEGORY_ID ?? '?'}`)
  338 |         .join(',')}`,
  339 |   });
  340 | 
  341 |   expect(
  342 |     runDeal,
  343 |     `Expected a NEW Deal on Contact ${TEST_CONTACT_ID} (ID>${baselineMaxId}) ` +
  344 |       `after inbound; none appeared within 60s. ` +
  345 |       `afterMaxId=${maxDealId(lastAfterPage)}`,
> 346 |   ).toBeTruthy();
      |     ^ Error: Expected a NEW Deal on Contact 1 (ID>1) after inbound; none appeared within 60s. afterMaxId=1
  347 | 
  348 |   // The deal THIS run created MUST land in the selected pipeline. Product
  349 |   // applies `CATEGORY_ID = dealPipelineId` end-to-end (#596) — this asserts it.
  350 |   expect(
  351 |     String(runDeal!.CATEGORY_ID ?? ''),
  352 |     `Expected run-created Deal ${runDeal!.ID} in pipeline ${targetValue}, ` +
  353 |       `got CATEGORY_ID=${runDeal!.CATEGORY_ID}`,
  354 |   ).toBe(String(targetValue));
  355 | 
  356 |   await page.goto(`${portal}/crm/deal/details/${runDeal!.ID}/`);
  357 |   await pinScreenshot(page, 'deal-details-in-selected-pipeline', testInfo);
  358 | });
  359 | 
```