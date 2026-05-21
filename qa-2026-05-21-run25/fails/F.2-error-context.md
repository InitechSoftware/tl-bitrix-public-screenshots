# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: F.2-oc-inbound-routing.spec.ts >> F.2 — inbound WA routes to Open Channels operator queue
- Location: tests\e2e-playwright\specs\F.2-oc-inbound-routing.spec.ts:62:1

# Error details

```
Error: Expected an OC session created/updated post-inbound; had 0 sessions before (newest DATE_CREATE=(none)), 0 after.

expect(received).toBe(expected) // Object.is equality

Expected: true
Received: false
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
  182 |       request.get(`${webhook}/imopenlines.session.list`, {
  183 |         params: { 'order[DATE_CREATE]': 'DESC' },
  184 |       }),
  185 |     {
  186 |       onRetry: (attempt, delayMs, err) =>
  187 |         testInfo.annotations.push({
  188 |           type: 'transport-retry',
  189 |           description: `imopenlines.session.list (before) attempt ${attempt} after ${delayMs}ms: ${String(err)}`,
  190 |         }),
  191 |     },
  192 |   );
  193 |   const beforeSessions =
  194 |     ((await beforeRes.json()) as { result?: SessionRow[] }).result ?? [];
  195 |   const beforeCount = beforeSessions.length;
  196 | 
  197 |   // Warm the binding's Bitrix OAuth context BEFORE the inbound (#548). After
  198 |   // A.1's wipe/reinstall the binding token is cold; the integration's first
  199 |   // post-install imconnector round trip spends time refreshing, which used to
  200 |   // delay OC-session creation past the poll window. One up-front user.current
  201 |   // round-trip forces that refresh now. Best-effort + non-fatal — the
  202 |   // OC-session poll below remains the oracle.
  203 |   const warm = await warmBitrixContext();
  204 |   testInfo.annotations.push({ type: 'bitrix-warmup', description: warm.detail });
  205 | 
  206 |   // 3. Fire inbound.
  207 |   const runId = new Date().toISOString();
  208 |   const text = `11-oc-routing ${runId}`;
  209 |   const { messageUid } = await sendInbound({
  210 |     from: '+447441447478',
  211 |     to: '+37122455329',
  212 |     text,
  213 |   });
  214 |   testInfo.annotations.push({ type: 'inbound-uid', description: messageUid });
  215 | 
  216 |   let received = false;
  217 |   const sdkDeadline = Date.now() + SDK_EVENT_POLL_MS;
  218 |   while (Date.now() < sdkDeadline) {
  219 |     const evt = await getLatestSdkEvent('received');
  220 |     if (evt && evt.text === text) {
  221 |       received = true;
  222 |       break;
  223 |     }
  224 |     await page.waitForTimeout(1_000);
  225 |   }
  226 |   expect(received, 'sdk_events did not record the inbound within 30s').toBe(
  227 |     true,
  228 |   );
  229 | 
  230 |   // 4. Poll for a new OC session. We accept either a count increase or
  231 |   // (when the portal already had sessions for this chat) a top-of-list
  232 |   // row whose DATE_CREATE is newer than the pre-inbound snapshot — Bitrix
  233 |   // re-uses the same OC session for the same chat thread, so the count
  234 |   // is sometimes stable while the timestamp advances.
  235 |   const beforeNewestDate =
  236 |     beforeSessions[0]?.DATE_CREATE ? new Date(beforeSessions[0].DATE_CREATE).getTime() : 0;
  237 |   let routedToOc = false;
  238 |   let afterCount = beforeCount;
  239 |   let lastSessions: SessionRow[] = [];
  240 |   const ocDeadline = Date.now() + OC_SESSION_POLL_MS;
  241 |   while (Date.now() < ocDeadline) {
  242 |     // Transport-retry the poll fetch too (#598) — same flake class as above.
  243 |     const res = await retryOnTransport(
  244 |       () =>
  245 |         request.get(`${webhook}/imopenlines.session.list`, {
  246 |           params: { 'order[DATE_CREATE]': 'DESC' },
  247 |         }),
  248 |       {
  249 |         onRetry: (attempt, delayMs, err) =>
  250 |           testInfo.annotations.push({
  251 |             type: 'transport-retry',
  252 |             description: `imopenlines.session.list (poll) attempt ${attempt} after ${delayMs}ms: ${String(err)}`,
  253 |           }),
  254 |       },
  255 |     );
  256 |     lastSessions = ((await res.json()) as { result?: SessionRow[] }).result ?? [];
  257 |     afterCount = lastSessions.length;
  258 |     const newestDate = lastSessions[0]?.DATE_CREATE
  259 |       ? new Date(lastSessions[0].DATE_CREATE).getTime()
  260 |       : 0;
  261 |     if (afterCount > beforeCount || newestDate > beforeNewestDate) {
  262 |       routedToOc = true;
  263 |       break;
  264 |     }
  265 |     await page.waitForTimeout(2_000);
  266 |   }
  267 | 
  268 |   // Diagnostic (#548): on failure, annotate exactly what
  269 |   // `imopenlines.session.list` last returned so the next run can tell a real
  270 |   // product gap (inbound recorded in sdk_events but no OC session ever
  271 |   // created — `imconnector.send.messages` not firing) apart from a budget
  272 |   // squeeze. sdk_events already confirmed the inbound landed above.
  273 |   if (!routedToOc) {
  274 |     testInfo.annotations.push({
  275 |       type: 'oc-session-not-found',
  276 |       description: `sdk_events recorded the inbound (received=${received}); imopenlines.session.list had ${beforeCount} sessions before (newest DATE_CREATE=${beforeSessions[0]?.DATE_CREATE ?? '(none)'}), ${afterCount} after ${OC_SESSION_POLL_MS / 1000}s. Top rows after: ${JSON.stringify(lastSessions.slice(0, 3))}`,
  277 |     });
  278 |   }
  279 |   expect(
  280 |     routedToOc,
  281 |     `Expected an OC session created/updated post-inbound; had ${beforeCount} sessions before (newest DATE_CREATE=${beforeSessions[0]?.DATE_CREATE ?? '(none)'}), ${afterCount} after.`,
> 282 |   ).toBe(true);
      |     ^ Error: Expected an OC session created/updated post-inbound; had 0 sessions before (newest DATE_CREATE=(none)), 0 after.
  283 | 
  284 |   // 5. Operator inbox screenshot.
  285 |   await page.goto(`${portal}/online/`);
  286 |   await page.waitForTimeout(3_000);
  287 |   await pinScreenshot(page, 'operator-inbox-with-new-session', testInfo);
  288 | });
  289 | 
```