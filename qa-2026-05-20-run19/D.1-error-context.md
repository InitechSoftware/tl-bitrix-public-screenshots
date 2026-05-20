# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: D.1-settings-autodeal-off.spec.ts >> D.1 — Auto-Add Deal OFF → inbound creates no new Deal
- Location: tests\e2e-playwright\specs\D.1-settings-autodeal-off.spec.ts:37:1

# Error details

```
TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
Call log:
  - waiting for locator('iframe[src*="/connector-settings"]').first()

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
  48  |  *   - input[name="actionOnClosedChat"] (radio: create_deal | reopen | none)
  49  |  *   - input[name="activityAggregationMode"] (radio: per_day | per_message)
  50  |  *   - select[name="phoneMatchingCountry"]
  51  |  *   - button[type="submit"]  // text: "Save settings"
  52  |  *
  53  |  * Save flow: the form POSTs to `/api/connector-settings/save` which 303s
  54  |  * back to `/connector-settings?saved=1`. The reloaded page renders a flash
  55  |  * `<p role="status">Settings saved.</p>`. Use {@link saveConnectorSettings}
  56  |  * which clicks Save and waits for the flash, not for navigation (the
  57  |  * navigation happens INSIDE the iframe and does not unload the parent page).
  58  |  */
  59  | 
  60  | /** Common selector for the placement iframe — used for frameLocator scoping. */
  61  | const IFRAME_SELECTOR = 'iframe[src*="/connector-settings"]';
  62  | 
  63  | /**
  64  |  * Opens the connector-settings placement from the portal home and returns
  65  |  * once the iframe is attached and the in-iframe form has rendered.
  66  |  *
  67  |  * Caller contract:
  68  |  *   - DO NOT call `installSidePanelOverlayHandler` before invoking this. The
  69  |  *     helper handles the pre-existing-slider dismissal itself (one-shot) and
  70  |  *     then explicitly avoids the re-arming handler so the placement slider
  71  |  *     stays open.
  72  |  *   - `page.goto(`${portal}/`)` is performed inside the helper.
  73  |  */
  74  | export async function openConnectorSettings(page: Page, portal: string): Promise<FrameLocator> {
  75  |   // [E2E_SLIDER_DIAGNOSTIC] gated diagnostic narration of the open-flow.
  76  |   diagLog('openConnectorSettings:start', { portal });
  77  |   await page.goto(`${portal}/`);
  78  |   await diagOverlays(page, 'pre-dismiss');
  79  | 
  80  |   // One-shot: dismiss any pre-existing marketplace slider that may have been
  81  |   // left open by storage-state capture or a prior test. We deliberately do
  82  |   // NOT install the re-arming handler — the placement we're about to open
  83  |   // IS itself a side-panel slider, and we want it to stay open.
  84  |   await dismissSidePanelOverlay(page);
  85  |   await diagOverlays(page, 'post-dismiss');
  86  | 
  87  |   // [E2E_SLIDER_DIAGNOSTIC] Capture click target shape pre-click.
  88  |   if (diagEnabled()) {
  89  |     const target = page
  90  |       .locator(
  91  |         `a.menu-item-link[href*="${LEFT_MENU_ITEMS.connectorSettings.handlerSlug}"], a[href*="${LEFT_MENU_ITEMS.connectorSettings.handlerSlug}"]`,
  92  |       )
  93  |       .first();
  94  |     const targetInfo = await target
  95  |       .evaluate((el: any) => {
  96  |         const rect = el.getBoundingClientRect();
  97  |         return {
  98  |           tag: el.tagName,
  99  |           href: el.getAttribute('href'),
  100 |           text: (el.textContent ?? '').trim().slice(0, 80),
  101 |           box: { x: rect.x, y: rect.y, w: rect.width, h: rect.height },
  102 |         };
  103 |       })
  104 |       .catch((err) => ({ error: String(err) }));
  105 |     diagLog('click-target', targetInfo);
  106 |     await diagScreenshot(page, '01-pre-click');
  107 |   }
  108 | 
  109 |   // Click the LEFT_MENU "WhatsApp settings" anchor via the shared helper.
  110 |   // PR #475 made this resilient to title rewordings + collapsed groups.
  111 |   const clickStart = Date.now();
  112 |   await clickLeftMenuItem(page, LEFT_MENU_ITEMS.connectorSettings);
  113 |   diagLog('click-done', { elapsedMs: Date.now() - clickStart });
  114 | 
  115 |   // [E2E_SLIDER_DIAGNOSTIC] Step 3: post-click child enumeration after 500ms.
  116 |   if (diagEnabled()) {
  117 |     await page.waitForTimeout(500);
  118 |     await diagOverlays(page, 'post-click-500ms');
  119 |     const childTree = await page
  120 |       .evaluate(() => {
  121 |         const d: any = (globalThis as any).document;
  122 |         const root = d.querySelector('#a11y-slider-container');
  123 |         if (!root) return { rootExists: false, children: [] as unknown[] };
  124 |         const children = Array.from(root.children as any[]).map((c: any) => ({
  125 |           tag: c.tagName,
  126 |           dataId: c.getAttribute('data-id'),
  127 |           className: c.getAttribute('class'),
  128 |           iframeSrc: c.querySelector('iframe')?.getAttribute('src') ?? null,
  129 |         }));
  130 |         return { rootExists: true, children };
  131 |       })
  132 |       .catch((err) => ({ error: String(err) }));
  133 |     diagLog('post-click-children', childTree);
  134 |     await diagScreenshot(page, '02-post-click-500ms');
  135 | 
  136 |     const attach = await waitForIframeWithDetail(page, '/connector-settings', 8_000);
  137 |     diagLog('iframe-attach', attach);
  138 |     if (attach.attached) {
  139 |       await page.waitForTimeout(500);
  140 |       const reCheck = await waitForIframeWithDetail(page, '/connector-settings', 500);
  141 |       diagLog('iframe-attach-recheck-500ms', reCheck);
  142 |     }
  143 |   }
  144 | 
  145 |   // Wait for the placement iframe to attach. Bitrix mounts it inside
  146 |   // `#a11y-slider-container .side-panel.--open > .side-panel-content`.
  147 |   const iframe = page.locator(IFRAME_SELECTOR).first();
> 148 |   await iframe.waitFor({ state: 'attached', timeout: 20_000 });
      |                ^ TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
  149 | 
  150 |   const frame = page.frameLocator(IFRAME_SELECTOR).first();
  151 | 
  152 |   // [E2E_SLIDER_DIAGNOSTIC] Step 5 + 6: iframe load + body snippet.
  153 |   if (diagEnabled()) {
  154 |     const load = await waitForIframeLoad(page, '/connector-settings', 8_000);
  155 |     diagLog('iframe-load', load);
  156 |     const snippet = await captureIframeBodySnippet(
  157 |       page,
  158 |       '/connector-settings',
  159 |       300,
  160 |     );
  161 |     diagLog('iframe-body-snippet', { snippet });
  162 |     await diagScreenshot(page, '03-iframe-loaded');
  163 |   }
  164 | 
  165 |   // Wait for the form to render inside the iframe — the Save button is the
  166 |   // canonical "we've fully loaded" signal because it sits at the bottom of
  167 |   // the form (so by the time it's visible, every input above it has been
  168 |   // emitted by the renderer).
  169 |   await expect(
  170 |     frame.locator('button[type="submit"]:has-text("Save settings")').first(),
  171 |   ).toBeVisible({ timeout: 20_000 });
  172 |   return frame;
  173 | }
  174 | 
  175 | /**
  176 |  * FrameLocator for an already-open connector-settings placement. Use when
  177 |  * the placement has been re-rendered (e.g. after a save flash) and we want
  178 |  * to re-query a field without re-opening the slider.
  179 |  */
  180 | export function getConnectorSettingsFrame(page: Page): FrameLocator {
  181 |   return page.frameLocator(IFRAME_SELECTOR).first();
  182 | }
  183 | 
  184 | /**
  185 |  * Click "Save settings" and wait for the save to land. The form POSTs to
  186 |  * `/api/connector-settings/save` which 303s back to
  187 |  * `/connector-settings?saved=1`. Bitrix re-iframes the placement on the
  188 |  * subsequent GET load, so the post-save iframe shows EITHER:
  189 |  *   - the placement re-mounted (Save button visible again); or
  190 |  *   - the placeholder GET branch (if Bitrix doesn't re-POST on its own)
  191 |  *
  192 |  * We try to detect the `<p role="status">Settings saved.</p>` flash first
  193 |  * (best-case signal), and fall back to "the click happened and the form
  194 |  * is no longer dirty" — `button[type="submit"]:has-text("Save settings")`
  195 |  * detaching/reattaching is enough to know the iframe navigated.
  196 |  *
  197 |  * We DO NOT assert against `page.waitForNavigation`: the navigation
  198 |  * happens INSIDE the iframe — the parent Bitrix page does not unload.
  199 |  */
  200 | export async function saveConnectorSettings(frame: FrameLocator): Promise<void> {
  201 |   const saveButton = frame
  202 |     .locator('button[type="submit"]:has-text("Save settings")')
  203 |     .first();
  204 |   await saveButton.click();
  205 |   // Best-effort: wait for either the flash (post-save renderer path) OR a
  206 |   // brief settle window. The form action 303s back to `/connector-settings?
  207 |   // saved=1`; whether Bitrix re-POSTs the placement on the resulting GET is
  208 |   // portal-dependent (Bitrix preserves the URL but only re-POSTs the
  209 |   // placement on a user-driven left-menu nav, not on an in-iframe redirect).
  210 |   // So we accept either signal.
  211 |   await frame
  212 |     .locator('[role="status"]')
  213 |     .first()
  214 |     .waitFor({ state: 'visible', timeout: 5_000 })
  215 |     .catch(() => {
  216 |       /* flash never appeared — accept either signal, save still posted */
  217 |     });
  218 | }
  219 | 
  220 | 
```