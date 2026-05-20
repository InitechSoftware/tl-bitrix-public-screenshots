# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: H.1-messageservice-provider.spec.ts >> H.1 — TimelinesAI appears in CRM Marketing messageservice provider list
- Location: tests\e2e-playwright\specs\H.1-messageservice-provider.spec.ts:22:1

# Error details

```
Error: TimelinesAI must appear as a messageservice provider

expect(locator).toBeVisible() failed

Locator: locator('.bx-messageservice-sender-list, .bx-messageservice-sender, [data-bx-messageservice-sender], .ui-sender-list, form[name="sender_edit_form"], .crm-settings-sender, .crm-settings-sender-list, .main-ui-grid, #workarea-content').first().locator('text=/timelinesai/i').first()
Expected: visible
Timeout: 20000ms
Error: element(s) not found

Call log:
  - TimelinesAI must appear as a messageservice provider with timeout 20000ms
  - waiting for locator('.bx-messageservice-sender-list, .bx-messageservice-sender, [data-bx-messageservice-sender], .ui-sender-list, form[name="sender_edit_form"], .crm-settings-sender, .crm-settings-sender-list, .main-ui-grid, #workarea-content').first().locator('text=/timelinesai/i').first()

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - group [ref=e2]
  - generic [ref=e4]:
    - navigation "Main menu" [ref=e6]:
      - button "Expand menu" [ref=e9] [cursor=pointer]
      - generic [ref=e11]:
        - generic [ref=e12]:
          - list [ref=e13]:
            - listitem [ref=e14]:
              - button "Collaboration" [expanded] [ref=e15] [cursor=pointer]
            - listitem [ref=e18]:
              - list [ref=e19]:
                - listitem [ref=e20]:
                  - link "Messenger, 1 new" [ref=e21] [cursor=pointer]:
                    - /url: /online/
                    - generic [ref=e27]: "1"
                - listitem [ref=e30]:
                  - link "Collabs" [ref=e31] [cursor=pointer]:
                    - /url: /online/?IM_COLLAB
                - listitem [ref=e36]:
                  - link "Feed" [ref=e37] [cursor=pointer]:
                    - /url: /stream/
                - listitem [ref=e42]:
                  - link:
                    - /url: /company/personal/user/1/calendar/?EVENT_ID=NEW
                  - link "Calendar" [ref=e43] [cursor=pointer]:
                    - /url: /company/personal/user/1/calendar/
                - listitem [ref=e48]:
                  - link "Documents" [ref=e49] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/documents/?st[tool]=docs&st[category]=docs&st[event]=open_section&st[c_section]=left_menu
                - listitem [ref=e54]:
                  - link "Boards" [ref=e55] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/boards/?c_section=left_menu
                - listitem [ref=e60]:
                  - link "Drive" [ref=e61] [cursor=pointer]:
                    - /url: /company/personal/user/1/disk/path/
                - listitem [ref=e66]:
                  - link "Webmail" [ref=e67] [cursor=pointer]:
                    - /url: /mail/?source=left_menu
                - listitem [ref=e72]:
                  - link:
                    - /url: /company/personal/user/1/groups/create/
                  - link "Workgroups" [ref=e73] [cursor=pointer]:
                    - /url: /workgroups/
            - listitem [ref=e78]:
              - link:
                - /url: /company/personal/user/1/tasks/task/edit/0/?ta_sec=tasks&ta_el=left_menu&miniform=true
              - link "Tasks and Projects" [ref=e79] [cursor=pointer]:
                - /url: /company/personal/user/1/tasks/?ta_sec=left_menu
            - listitem [ref=e84]:
              - link "CRM" [ref=e85] [cursor=pointer]:
                - /url: /crm/deal/?redirect_to
            - listitem [ref=e90]:
              - link "Booking" [ref=e91] [cursor=pointer]:
                - /url: /booking/
            - listitem [ref=e96]:
              - link "Inventory management" [ref=e97] [cursor=pointer]:
                - /url: /shop/documents/inventory/
            - listitem [ref=e102]:
              - link "Marketing" [ref=e103] [cursor=pointer]:
                - /url: /marketing/
            - listitem [ref=e108]:
              - link "Sites and stores" [ref=e109] [cursor=pointer]:
                - /url: /sites/
            - listitem [ref=e114]:
              - link "e-Signature for HR" [ref=e115] [cursor=pointer]:
                - /url: /sign/b2e/
            - listitem [ref=e120]:
              - link "e-Signature" [ref=e121] [cursor=pointer]:
                - /url: /sign/
            - listitem [ref=e126]:
              - link "BI Builder" [ref=e127] [cursor=pointer]:
                - /url: /bi/dashboard
            - listitem [ref=e132]:
              - link "Employees" [ref=e133] [cursor=pointer]:
                - /url: /company/
            - listitem [ref=e138]:
              - link "Automation" [ref=e139] [cursor=pointer]:
                - /url: /bizproc/userprocesses/
            - listitem [ref=e144]:
              - button "Applications" [expanded] [ref=e145] [cursor=pointer]
            - listitem [ref=e148]:
              - list [ref=e149]:
                - listitem [ref=e150]:
                  - link "Market" [ref=e151] [cursor=pointer]:
                    - /url: /market/
                - listitem [ref=e156]:
                  - link "Developer resources" [ref=e157] [cursor=pointer]:
                    - /url: /devops/
                - listitem [ref=e162]:
                  - link "MCP connections" [ref=e163] [cursor=pointer]:
                    - /url: /mcp/
                - listitem [ref=e168]:
                  - link "WhatsApp integration by TimelinesAI" [ref=e169] [cursor=pointer]:
                    - /url: /marketplace/app/1/
                    - generic [ref=e171]: WI
                - listitem [ref=e174]:
                  - link "WhatsApp audit log" [ref=e175] [cursor=pointer]:
                    - /url: /devops/placement/579/
                    - generic [ref=e177]: WA
                - listitem [ref=e180]:
                  - link "WhatsApp settings" [ref=e181] [cursor=pointer]:
                    - /url: /devops/placement/581/
                    - generic [ref=e183]: WS
          - list [ref=e186]:
            - listitem [ref=e187] [cursor=pointer]
            - listitem [ref=e190]:
              - link "Subscription" [ref=e191] [cursor=pointer]:
                - /url: /settings/license.php?TARIFF_WIDGET=Y
        - button "Show all" [ref=e196]
      - generic [ref=e201]:
        - button [ref=e202]
        - button "Upgrade your plan" [ref=e207] [cursor=pointer]:
          - generic:
            - generic: Upgrade your plan
    - banner [ref=e209]:
      - generic [ref=e210]:
        - navigation [ref=e212]:
          - list [ref=e213]:
            - listitem [ref=e214]:
              - link "Start" [ref=e215] [cursor=pointer]:
                - /url: /marketing/
                - generic [ref=e218]: Start
            - listitem [ref=e219]:
              - link "Campaigns" [ref=e220] [cursor=pointer]:
                - /url: /marketing/letter/
                - generic [ref=e223]: Campaigns
            - listitem [ref=e224]:
              - link "Ads" [ref=e225] [cursor=pointer]:
                - /url: /marketing/ads/
                - generic [ref=e228]: Ads
            - listitem [ref=e229]:
              - link "Segments" [ref=e230] [cursor=pointer]:
                - /url: /marketing/segment/
                - generic [ref=e233]: Segments
            - listitem [ref=e234]:
              - link "Sales Boost" [ref=e235] [cursor=pointer]:
                - /url: /marketing/rc/
                - generic [ref=e238]: Sales Boost
            - listitem [ref=e239]:
              - link "My Templates" [ref=e240] [cursor=pointer]:
                - /url: /marketing/template/
                - generic [ref=e243]: My Templates
            - listitem [ref=e244]:
              - link "Black List" [ref=e245] [cursor=pointer]:
                - /url: /marketing/blacklist/
                - generic [ref=e248]: Black List
            - listitem [ref=e249]:
              - button "More" [ref=e250] [cursor=pointer]:
                - generic [ref=e253]: More
        - generic [ref=e255]:
          - search [ref=e258]:
            - textbox [disabled] [ref=e259]:
              - /placeholder: find people, documents, and more
            - button "Search" [ref=e260]
          - link "Bitrix 24" [ref=e264] [cursor=pointer]:
            - /url: /
            - generic [ref=e265]:
              - generic [ref=e266]: Bitrix
              - generic [ref=e267]: "24"
          - button [ref=e268] [cursor=pointer]
          - generic [ref=e270]:
            - button "Invite" [ref=e272] [cursor=pointer]: Invite
            - button "Buy Now" [ref=e274] [cursor=pointer]: Buy Now
            - button "Helpdesk 6" [ref=e276] [cursor=pointer]:
              - text: Helpdesk
              - generic [ref=e280]: "6"
    - button "Profile" [ref=e282] [cursor=pointer]:
      - generic [ref=e286]: 7:04 PM
    - main [ref=e292]:
      - generic [ref=e293]:
        - generic [ref=e299]:
          - generic [ref=e300]: Error 404
          - button "Add current page to left menu" [ref=e301] [cursor=pointer]
        - generic [ref=e306]:
          - generic [ref=e307]:
            - text: Unfortunately, the page you requested
            - text: was not found.
          - generic [ref=e308]:
            - text: If you think this shouldn't have happened
            - text: please contact the website administrator.
    - contentinfo [ref=e310]:
      - generic [ref=e311]:
        - generic [ref=e312]:
          - link "Bitrix 24" [ref=e314] [cursor=pointer]:
            - /url: https://www.bitrix24.com
            - generic [ref=e315]:
              - generic [ref=e316]: Bitrix
              - generic [ref=e317]: "24"
          - button "English" [ref=e319] [cursor=pointer]
        - generic [ref=e320]: © 2026 Bitrix24
        - generic [ref=e321]:
          - button "Implementation request" [ref=e322] [cursor=pointer]
          - button "Themes" [ref=e323] [cursor=pointer]
          - button "Print" [ref=e324] [cursor=pointer]
    - region "Chat bar" [ref=e326]:
      - generic [ref=e328]:
        - generic [ref=e333] [cursor=pointer]: "9"
        - generic [ref=e340]:
          - generic "General chat" [ref=e344] [cursor=pointer]
          - generic [ref=e348] [cursor=pointer]:
            - generic "Bitrix24 Support" [ref=e349]:
              - img "Bitrix24 Support" [ref=e350]
            - generic [ref=e351]: "1"
          - generic "Company News" [ref=e355] [cursor=pointer]
          - generic "My Notes" [ref=e360] [cursor=pointer]
  - generic:
    - generic:
      - generic:
        - generic: The server connection is successfully established
  - dialog [ref=e361]:
    - generic [ref=e365]:
      - generic [ref=e366]:
        - heading "Invite sales representatives" [level=4] [ref=e367]
        - text: Learn Bitrix24 CRM features and start selling in no time.
      - button "User invitation" [ref=e368] [cursor=pointer]:
        - generic [ref=e369]: User invitation
    - button "Close" [ref=e370] [cursor=pointer]
```

# Test source

```ts
  26  | 
  27  |   // The messageservice "SMS sender" provider list / picker surfaces in a
  28  |   // handful of places depending on Bitrix24 portal state. Run-17 of this
  29  |   // spec (see #427) showed why the previous candidate order was wrong:
  30  |   //
  31  |   //   • `/crm/configs/sms/` does NOT consistently render a sender list.
  32  |   //     On portals with no custom messageservice provider activated yet
  33  |   //     in the UI, Bitrix serves a marketing splash page titled "SMS to
  34  |   //     Clients, Customers or Employees / Powered by TWILIO.COM" with a
  35  |   //     Twilio SID/Token onboarding form. There is no provider grid on
  36  |   //     this splash, so even if TimelinesAI is registered via
  37  |   //     `messageservice.sender.add` (which install-callback confirmedly
  38  |   //     does — see PR #474 investigation), the assertion can't find it
  39  |   //     here. The page returns 200 (not 404), so the previous fallback
  40  |   //     trigger never fired.
  41  |   //
  42  |   //   • `/marketing/sender/edit/0/?TYPE=SMS` IS the messageservice
  43  |   //     sender-edit wizard. Its TYPE=SMS variant lists every registered
  44  |   //     SMS sender (Twilio, plus any `messageservice.sender.add`
  45  |   //     entries — including `tlai_whatsapp_sms` → "TimelinesAI
  46  |   //     WhatsApp"). This is the surface our README and Help Center
  47  |   //     screenshots point customers at, so it's the right canonical
  48  |   //     check.
  49  |   //
  50  |   //   • `/crm/configs/sms/?config_mess_service=Y` is the deeper CRM-
  51  |   //     Settings URL which forces the sender-table view on portals
  52  |   //     that have at least one registered sender. Kept as second
  53  |   //     fallback for completeness.
  54  |   //
  55  |   // Strategy: try the marketing sender editor FIRST (canonical
  56  |   // customer surface), then the deeper CRM-settings sender table, and
  57  |   // only at the very end the bare `/crm/configs/sms/` (which on some
  58  |   // portals is the right page and on others is the Twilio splash). On
  59  |   // every candidate, treat (a) a Bitrix "Error 404" page OR (b) the
  60  |   // Twilio-splash marketing page as a miss and move on.
  61  |   const candidates = [
  62  |     `${portal}/marketing/sender/edit/0/?TYPE=SMS`,
  63  |     `${portal}/crm/configs/sms/?config_mess_service=Y`,
  64  |     `${portal}/crm/configs/sms/`,
  65  |   ];
  66  | 
  67  |   // Markers that say "this URL is not the messageservice sender list,
  68  |   // don't bother asserting on it":
  69  |   //   - Bitrix's standard 404 heading / page-not-found copy.
  70  |   //   - The Twilio onboarding splash that `/crm/configs/sms/` renders
  71  |   //     when no senders are activated — match on the unique strings
  72  |   //     "Powered by TWILIO.COM" / "Simple and robust SMS notification".
  73  |   const skipMarkerRegex =
  74  |     /error\s*404|page you requested was not found|powered by twilio\.com|simple and robust sms notification/i;
  75  | 
  76  |   let landedOn: string | null = null;
  77  |   for (const url of candidates) {
  78  |     await page.goto(url, { waitUntil: 'domcontentloaded' });
  79  |     const shouldSkip = await page
  80  |       .locator(`text=${skipMarkerRegex.source}`)
  81  |       .first()
  82  |       .isVisible({ timeout: 2_000 })
  83  |       .catch(() => false);
  84  |     if (!shouldSkip) {
  85  |       landedOn = url;
  86  |       break;
  87  |     }
  88  |   }
  89  | 
  90  |   if (!landedOn) {
  91  |     throw new Error(
  92  |       `H.1 — no candidate URL rendered the messageservice sender list ` +
  93  |         `(all returned 404 or the Twilio onboarding splash): ${candidates.join(', ')}`,
  94  |     );
  95  |   }
  96  | 
  97  |   await pinScreenshot(page, '01-sender-loaded', testInfo);
  98  | 
  99  |   // The provider list/picker is inside the messageservice sender widget.
  100 |   // Across Bitrix versions the wrapper class varies; we union the known
  101 |   // ones. CRM settings → SMS uses `.crm-settings-sender` / a generic
  102 |   // `.ui-grid` table; the marketing wizard uses `.bx-messageservice-*` /
  103 |   // `form[name="sender_edit_form"]`. We scope to that container so we
  104 |   // don't match the left-menu marketplace app entry
  105 |   // (`.menu-item-link-text` → "WhatsApp integration by TimelinesAI"),
  106 |   // which is in the DOM but hidden. See #410.
  107 |   const senderWidget = page
  108 |     .locator(
  109 |       [
  110 |         '.bx-messageservice-sender-list',
  111 |         '.bx-messageservice-sender',
  112 |         '[data-bx-messageservice-sender]',
  113 |         '.ui-sender-list',
  114 |         'form[name="sender_edit_form"]',
  115 |         '.crm-settings-sender',
  116 |         '.crm-settings-sender-list',
  117 |         '.main-ui-grid',
  118 |         '#workarea-content',
  119 |       ].join(', '),
  120 |     )
  121 |     .first();
  122 |   const providerEntry = senderWidget.locator('text=/timelinesai/i').first();
  123 |   await expect(
  124 |     providerEntry,
  125 |     'TimelinesAI must appear as a messageservice provider',
> 126 |   ).toBeVisible({
      |     ^ Error: TimelinesAI must appear as a messageservice provider
  127 |     timeout: 20_000,
  128 |   });
  129 |   await pinScreenshot(page, '02-provider-visible', testInfo);
  130 | });
  131 | 
```