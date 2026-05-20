# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: F.1-oc-line-picker.spec.ts >> F.1 — connector-settings shows TimelinesAI in the line picker
- Location: tests\e2e-playwright\specs\F.1-oc-line-picker.spec.ts:30:1

# Error details

```
TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
Call log:
  - waiting for locator('iframe[src*="tl-bitrix-integration.netlify.app"]').first()

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - group [ref=e2]
  - dialog "WhatsApp settings" [active] [ref=e6]:
    - iframe [ref=e9]:
      - iframe [ref=f1e7]:
        - generic [active] [ref=f2e1]:
          - heading "TimelinesAI WhatsApp connector" [level=1] [ref=f2e2]
          - paragraph [ref=f2e3]:
            - text: Inbound WhatsApp messages on
            - code [ref=f2e4]: (unknown portal)
            - text: are routed into the Bitrix Open Channels line below, alongside the existing CRM Activity logging.
          - generic [ref=f2e5]:
            - heading "Subscription" [level=2] [ref=f2e6]
            - generic [ref=f2e7]: Active — CRM Integration
            - paragraph [ref=f2e8]: 43 of 5050 messages used this period.
          - generic [ref=f2e9]:
            - heading "Status" [level=2] [ref=f2e10]
            - generic [ref=f2e11]:
              - generic [ref=f2e12]: Connector
              - generic [ref=f2e14]: Registered
            - generic [ref=f2e15]:
              - generic [ref=f2e16]: Current line
              - generic [ref=f2e17]: (no line selected yet)
            - generic [ref=f2e18]:
              - generic [ref=f2e19]: Activated on line
              - generic [ref=f2e21]: Unknown
          - generic [ref=f2e22]:
            - heading "Switch Open Line" [level=2] [ref=f2e23]
            - generic [ref=f2e24]:
              - generic [ref=f2e25]: Open Line
              - combobox [ref=f2e26]:
                - option "1 — Open Channel" [selected]
              - button "Switch line" [ref=f2e27] [cursor=pointer]
          - generic [ref=f2e28]:
            - heading "Behavior & CRM mapping" [level=2] [ref=f2e29]
            - generic [ref=f2e30]:
              - group "Auto-add" [ref=f2e31]:
                - generic [ref=f2e32]: Auto-add
                - generic [ref=f2e33] [cursor=pointer]:
                  - checkbox "Auto-Add Contact Create a Contact in Bitrix when an inbound WhatsApp arrives from an unknown phone. Turn off to drop unknown-sender messages instead." [checked] [ref=f2e34]
                  - generic [ref=f2e35]:
                    - generic [ref=f2e36]: Auto-Add Contact
                    - generic [ref=f2e37]: Create a Contact in Bitrix when an inbound WhatsApp arrives from an unknown phone. Turn off to drop unknown-sender messages instead.
                - generic [ref=f2e38] [cursor=pointer]:
                  - checkbox "Auto-Add Deal Bind the inbound message Activity to every open Deal of the matched Contact. Turn off to keep messages on the Contact only." [checked] [ref=f2e39]
                  - generic [ref=f2e40]:
                    - generic [ref=f2e41]: Auto-Add Deal
                    - generic [ref=f2e42]: Bind the inbound message Activity to every open Deal of the matched Contact. Turn off to keep messages on the Contact only.
              - group "Deal pipeline" [ref=f2e43]:
                - generic [ref=f2e44]: Deal pipeline
                - generic [ref=f2e45]: Newly-created Deals land in this pipeline (Bitrix CATEGORY_ID).
                - combobox [ref=f2e46]:
                  - option "General (default)" [selected]
              - group "On new chat (no Deal yet)" [ref=f2e47]:
                - generic [ref=f2e48]: On new chat (no Deal yet)
                - generic [ref=f2e49] [cursor=pointer]:
                  - radio "Create a new Deal Open a Deal in the selected pipeline and bind the Contact." [checked] [ref=f2e50]
                  - generic [ref=f2e51]:
                    - generic [ref=f2e52]: Create a new Deal
                    - generic [ref=f2e53]: Open a Deal in the selected pipeline and bind the Contact.
                - generic [ref=f2e54] [cursor=pointer]:
                  - radio "Create a new Lead Open a Lead instead of a Deal — sales-leads-first orgs." [ref=f2e55]
                  - generic [ref=f2e56]:
                    - generic [ref=f2e57]: Create a new Lead
                    - generic [ref=f2e58]: Open a Lead instead of a Deal — sales-leads-first orgs.
                - generic [ref=f2e59] [cursor=pointer]:
                  - radio "Do nothing Log the message on the Contact only; no Deal or Lead is created." [ref=f2e60]
                  - generic [ref=f2e61]:
                    - generic [ref=f2e62]: Do nothing
                    - generic [ref=f2e63]: Log the message on the Contact only; no Deal or Lead is created.
              - group "On closed-Deal chat" [ref=f2e64]:
                - generic [ref=f2e65]: On closed-Deal chat
                - generic [ref=f2e66] [cursor=pointer]:
                  - radio "Create a new Deal Open a fresh Deal in the selected pipeline." [checked] [ref=f2e67]
                  - generic [ref=f2e68]:
                    - generic [ref=f2e69]: Create a new Deal
                    - generic [ref=f2e70]: Open a fresh Deal in the selected pipeline.
                - generic [ref=f2e71] [cursor=pointer]:
                  - radio "Reopen the most recent closed Deal Flip STAGE_ID back to NEW on the latest closed Deal for this Contact." [ref=f2e72]
                  - generic [ref=f2e73]:
                    - generic [ref=f2e74]: Reopen the most recent closed Deal
                    - generic [ref=f2e75]: Flip STAGE_ID back to NEW on the latest closed Deal for this Contact.
                - generic [ref=f2e76] [cursor=pointer]:
                  - radio "Do nothing Leave closed Deals alone; log the message on the Contact only." [ref=f2e77]
                  - generic [ref=f2e78]:
                    - generic [ref=f2e79]: Do nothing
                    - generic [ref=f2e80]: Leave closed Deals alone; log the message on the Contact only.
              - group "Activity aggregation" [ref=f2e81]:
                - generic [ref=f2e82]: Activity aggregation
                - generic [ref=f2e83] [cursor=pointer]:
                  - radio "One Activity per day Collapse the day's messages for this Contact into a single Activity (default)." [checked] [ref=f2e84]
                  - generic [ref=f2e85]:
                    - generic [ref=f2e86]: One Activity per day
                    - generic [ref=f2e87]: Collapse the day's messages for this Contact into a single Activity (default).
                - generic [ref=f2e88] [cursor=pointer]:
                  - radio "One Activity per message Create a fresh Activity for every inbound message — more granular timeline, more rows." [ref=f2e89]
                  - generic [ref=f2e90]:
                    - generic [ref=f2e91]: One Activity per message
                    - generic [ref=f2e92]: Create a fresh Activity for every inbound message — more granular timeline, more rows.
              - group "Phone matching" [ref=f2e93]:
                - generic [ref=f2e94]: Phone matching
                - generic [ref=f2e95]: Default country for phone numbers without a country code in Bitrix CRM.
                - combobox [ref=f2e96]:
                  - option "Auto (portal locale)" [selected]
                  - option "United States (+1)"
                  - option "United Kingdom (+44)"
                  - option "Canada (+1)"
                  - option "Australia (+61)"
                  - option "India (+91)"
                  - option "Germany (+49)"
                  - option "France (+33)"
                  - option "Brazil (+55)"
                  - option "Mexico (+52)"
                  - option "Netherlands (+31)"
                  - option "Spain (+34)"
                  - option "Italy (+39)"
                  - option "United Arab Emirates (+971)"
                  - option "South Africa (+27)"
              - button "Save settings" [ref=f2e97] [cursor=pointer]
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
              - link "CRM" [ref=e100] [cursor=pointer]:
                - /url: /crm/deal/?redirect_to
            - listitem [ref=e105]:
              - link "Booking" [ref=e106] [cursor=pointer]:
                - /url: /booking/
            - listitem [ref=e111]:
              - link "Inventory management" [ref=e112] [cursor=pointer]:
                - /url: /shop/documents/inventory/
            - listitem [ref=e117]:
              - link "Marketing" [ref=e118] [cursor=pointer]:
                - /url: /marketing/
            - listitem [ref=e123]:
              - link "Sites and stores" [ref=e124] [cursor=pointer]:
                - /url: /sites/
            - listitem [ref=e129]:
              - link "e-Signature for HR" [ref=e130] [cursor=pointer]:
                - /url: /sign/b2e/
            - listitem [ref=e135]:
              - link "e-Signature" [ref=e136] [cursor=pointer]:
                - /url: /sign/
            - listitem [ref=e141]:
              - link "BI Builder" [ref=e142] [cursor=pointer]:
                - /url: /bi/dashboard
            - listitem [ref=e147]:
              - link "Employees" [ref=e148] [cursor=pointer]:
                - /url: /company/
            - listitem [ref=e153]:
              - link "Automation" [ref=e154] [cursor=pointer]:
                - /url: /bizproc/userprocesses/
            - listitem [ref=e159]:
              - button "Applications" [expanded] [ref=e160] [cursor=pointer]
            - listitem [ref=e163]:
              - list [ref=e164]:
                - listitem [ref=e165]:
                  - link "Market" [ref=e166] [cursor=pointer]:
                    - /url: /market/
                - listitem [ref=e171]:
                  - link "Developer resources" [ref=e172] [cursor=pointer]:
                    - /url: /devops/
                - listitem [ref=e177]:
                  - link "MCP connections" [ref=e178] [cursor=pointer]:
                    - /url: /mcp/
                - listitem [ref=e183]:
                  - link "WhatsApp integration by TimelinesAI" [ref=e184] [cursor=pointer]:
                    - /url: /marketplace/app/1/
                    - generic [ref=e186]: WI
                - listitem [ref=e189]:
                  - link "WhatsApp audit log" [ref=e190] [cursor=pointer]:
                    - /url: /devops/placement/579/
                    - generic [ref=e192]: WA
                - listitem [ref=e195]:
                  - link "WhatsApp settings" [ref=e196] [cursor=pointer]:
                    - /url: /devops/placement/581/
                    - generic [ref=e198]: WS
          - list [ref=e201]:
            - listitem [ref=e202] [cursor=pointer]
            - listitem [ref=e205]:
              - link "Subscription" [ref=e206] [cursor=pointer]:
                - /url: /settings/license.php?TARIFF_WIDGET=Y
        - button "Show all" [ref=e211]
      - generic [ref=e216]:
        - button [ref=e217]
        - button "Upgrade your plan" [ref=e222] [cursor=pointer]:
          - generic:
            - generic: Upgrade your plan
    - banner [ref=e224]:
      - generic [ref=e225]:
        - navigation [ref=e227]:
          - list [ref=e228]:
            - listitem [ref=e229]:
              - button "Chats 1" [ref=e230] [cursor=pointer]:
                - generic [ref=e233]: Chats
                - generic [ref=e234]: "1"
            - listitem [ref=e235]:
              - button "Task chats" [ref=e236] [cursor=pointer]:
                - generic [ref=e239]: Task chats
            - listitem [ref=e240]:
              - button "CoPilot" [ref=e241] [cursor=pointer]:
                - generic [ref=e244]: CoPilot
            - listitem [ref=e245]:
              - button "Collabs" [ref=e246] [cursor=pointer]:
                - generic [ref=e249]: Collabs
            - listitem [ref=e250]:
              - button "Channels" [ref=e251] [cursor=pointer]:
                - generic [ref=e254]: Channels
            - listitem [ref=e255]:
              - button "Contact Center" [ref=e256] [cursor=pointer]:
                - generic [ref=e259]: Contact Center
            - listitem [ref=e260]:
              - button "More 9" [ref=e261] [cursor=pointer]:
                - generic [ref=e264]: More
                - generic [ref=e266]: "9"
        - generic [ref=e267]:
          - search [ref=e270]:
            - textbox [disabled] [ref=e271]:
              - /placeholder: find people, documents, and more
            - button "Search" [ref=e272]
          - link "Bitrix 24" [ref=e276] [cursor=pointer]:
            - /url: /
            - generic [ref=e277]:
              - generic [ref=e278]: Bitrix
              - generic [ref=e279]: "24"
          - button [ref=e280] [cursor=pointer]
          - generic [ref=e282]:
            - button "Invite" [ref=e284] [cursor=pointer]: Invite
            - button "Buy Now" [ref=e286] [cursor=pointer]: Buy Now
            - button "Helpdesk 6" [ref=e288] [cursor=pointer]:
              - text: Helpdesk
              - generic [ref=e292]: "6"
    - button "Profile" [ref=e293] [cursor=pointer]
    - main [ref=e299]:
      - generic [ref=e306]:
        - generic [ref=e308]:
          - generic [ref=e309]:
            - button [ref=e310] [cursor=pointer]
            - textbox "Find employee or chat" [ref=e315]
          - generic [ref=e322]:
            - generic [ref=e324] [cursor=pointer]:
              - generic "General chat" [ref=e327]
              - generic [ref=e329]:
                - generic [ref=e330]:
                  - generic "General chat" [ref=e333]
                  - generic [ref=e335]: May 17
                - generic [ref=e338]: Anton Patrai granted administrator permissions to WhatsApp integration by TimelinesAI.
            - generic [ref=e341] [cursor=pointer]:
              - generic "Bitrix24 Support" [ref=e344]:
                - img "Bitrix24 Support" [ref=e345]
              - generic [ref=e346]:
                - generic [ref=e347]:
                  - generic "Bitrix24 Support" [ref=e351]
                  - generic [ref=e353]: May 12
                - generic [ref=e354]:
                  - generic [ref=e356]: "👋 Hi there! I’m your Bitrix24 assistant. I can help you: • Build your CRM in minutes • Create smart automations • Launch a chat, site, or project • Or just find the right button when you’re stuck! Ask away — I’m online 24/7 or learn more 👉 here. [Attachment]"
                  - generic [ref=e360]: "1"
            - generic [ref=e362] [cursor=pointer]:
              - generic "Company News" [ref=e365]
              - generic [ref=e367]:
                - generic [ref=e368]:
                  - generic "Company News" [ref=e371]
                  - generic [ref=e373]: May 12
                - generic [ref=e376]: Share important information and news. Follow to remain informed about the latest developments. Leave comments and discuss posts.
            - generic [ref=e379] [cursor=pointer]:
              - generic "My Notes" [ref=e382]
              - generic [ref=e383]:
                - generic [ref=e384]:
                  - generic "Notes" [ref=e387]
                  - generic [ref=e389]: May 12
                - generic [ref=e392]: Visible to you only
        - generic [ref=e396]:
          - generic [ref=e398]: Select a chat to start communicating
          - generic [ref=e399]: or
          - generic [ref=e400] [cursor=pointer]: Invite users
  - generic:
    - generic:
      - generic:
        - generic: The server connection is successfully established
  - dialog [ref=e401]:
    - generic [ref=e405]:
      - generic [ref=e406]:
        - heading "Invite sales representatives" [level=4] [ref=e407]
        - text: Learn Bitrix24 CRM features and start selling in no time.
      - button "User invitation" [ref=e408] [cursor=pointer]:
        - generic [ref=e409]: User invitation
    - button "Close" [ref=e410] [cursor=pointer]
```

# Test source

```ts
  31  |  *
  32  |  * Strategy here:
  33  |  *   1. One-shot dismiss any side-panel that may be open BEFORE the click
  34  |  *      (carries over from the install flow). Idempotent.
  35  |  *   2. Click the connector-settings left-menu item via the shared
  36  |  *      handler-URL/title locator (PR #475).
  37  |  *   3. Wait for the slider to appear AND for its inner iframe to
  38  |  *      attach. Do NOT install the auto-dismiss handler — once the
  39  |  *      slider is the panel we want, dismissing it defeats the test.
  40  |  *   4. Return a `FrameLocator` scoped to the iframe so callers can
  41  |  *      drill into the connector-settings form.
  42  |  *
  43  |  * Surface coverage:
  44  |  *   - F.1 (line picker) — searches for the "TimelinesAI" header text.
  45  |  *   - F.2 (OC routing) — picks an Open Line via `select[name="line_id"]`.
  46  |  *   - D.1 / D.2 / D.3 — toggle `name="autoAddDeal"` / `name="autoAddContact"`
  47  |  *     / `select[name="dealPipelineId"]` (kept on existing helper for now;
  48  |  *     can be migrated separately).
  49  |  */
  50  | export async function openConnectorSettingsFrame(
  51  |   page: Page,
  52  | ): Promise<FrameLocator> {
  53  |   const portal = process.env.BITRIX_PORTAL_URL!;
  54  |   const iframeUrlMatch = 'tl-bitrix-integration.netlify.app';
  55  | 
  56  |   // [E2E_SLIDER_DIAGNOSTIC] gated narration of the open-flow.
  57  |   diagLog('openConnectorSettingsFrame:start', { portal, iframeUrlMatch });
  58  |   await page.goto(`${portal}/`);
  59  |   await diagOverlays(page, 'pre-dismiss');
  60  | 
  61  |   // One-shot: clear any leftover side-panel (e.g. install Continue card)
  62  |   // BEFORE we click. We don't re-arm an auto-handler because the click
  63  |   // we're about to make will OPEN the slider we want to keep.
  64  |   await dismissSidePanelOverlay(page);
  65  |   await diagOverlays(page, 'post-dismiss');
  66  | 
  67  |   // [E2E_SLIDER_DIAGNOSTIC] Click target shape + pre-click screenshot.
  68  |   if (diagEnabled()) {
  69  |     const target = page
  70  |       .locator(
  71  |         `a.menu-item-link[href*="${LEFT_MENU_ITEMS.connectorSettings.handlerSlug}"], a[href*="${LEFT_MENU_ITEMS.connectorSettings.handlerSlug}"]`,
  72  |       )
  73  |       .first();
  74  |     const targetInfo = await target
  75  |       .evaluate((el: any) => {
  76  |         const rect = el.getBoundingClientRect();
  77  |         return {
  78  |           tag: el.tagName,
  79  |           href: el.getAttribute('href'),
  80  |           text: (el.textContent ?? '').trim().slice(0, 80),
  81  |           box: { x: rect.x, y: rect.y, w: rect.width, h: rect.height },
  82  |         };
  83  |       })
  84  |       .catch((err) => ({ error: String(err) }));
  85  |     diagLog('click-target', targetInfo);
  86  |     await diagScreenshot(page, '01-pre-click');
  87  |   }
  88  | 
  89  |   const clickStart = Date.now();
  90  |   await clickLeftMenuItem(page, LEFT_MENU_ITEMS.connectorSettings);
  91  |   diagLog('click-done', { elapsedMs: Date.now() - clickStart });
  92  | 
  93  |   // [E2E_SLIDER_DIAGNOSTIC] post-click DOM enumeration after 500ms + the
  94  |   // instrumented iframe-attach wait that runs alongside the production wait.
  95  |   if (diagEnabled()) {
  96  |     await page.waitForTimeout(500);
  97  |     await diagOverlays(page, 'post-click-500ms');
  98  |     const childTree = await page
  99  |       .evaluate(() => {
  100 |         const d: any = (globalThis as any).document;
  101 |         const root = d.querySelector('#a11y-slider-container');
  102 |         if (!root) return { rootExists: false, children: [] as unknown[] };
  103 |         const children = Array.from(root.children as any[]).map((c: any) => ({
  104 |           tag: c.tagName,
  105 |           dataId: c.getAttribute('data-id'),
  106 |           className: c.getAttribute('class'),
  107 |           iframeSrc: c.querySelector('iframe')?.getAttribute('src') ?? null,
  108 |         }));
  109 |         return { rootExists: true, children };
  110 |       })
  111 |       .catch((err) => ({ error: String(err) }));
  112 |     diagLog('post-click-children', childTree);
  113 |     await diagScreenshot(page, '02-post-click-500ms');
  114 | 
  115 |     const attach = await waitForIframeWithDetail(page, iframeUrlMatch, 8_000);
  116 |     diagLog('iframe-attach', attach);
  117 |     if (attach.attached) {
  118 |       await page.waitForTimeout(500);
  119 |       const reCheck = await waitForIframeWithDetail(page, iframeUrlMatch, 500);
  120 |       diagLog('iframe-attach-recheck-500ms', reCheck);
  121 |     }
  122 |   }
  123 | 
  124 |   // Wait for the slider to attach. Bitrix puts the placement iframe inside
  125 |   // `#a11y-slider-container .side-panel.side-panel-overlay.--open` — but
  126 |   // the iframe itself is the stable anchor (the slider may mount with a
  127 |   // skeleton before the iframe element appears).
  128 |   const iframeEl = page
  129 |     .locator('iframe[src*="tl-bitrix-integration.netlify.app"]')
  130 |     .first();
> 131 |   await iframeEl.waitFor({ state: 'attached', timeout: 20_000 });
      |                  ^ TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
  132 | 
  133 |   // [E2E_SLIDER_DIAGNOSTIC] Step 5 + 6: iframe load + body snippet.
  134 |   if (diagEnabled()) {
  135 |     const load = await waitForIframeLoad(page, iframeUrlMatch, 8_000);
  136 |     diagLog('iframe-load', load);
  137 |     const snippet = await captureIframeBodySnippet(page, iframeUrlMatch, 300);
  138 |     diagLog('iframe-body-snippet', { snippet });
  139 |     await diagScreenshot(page, '03-iframe-loaded');
  140 |   }
  141 | 
  142 |   return page
  143 |     .frameLocator('iframe[src*="tl-bitrix-integration.netlify.app"]')
  144 |     .first();
  145 | }
  146 | 
```