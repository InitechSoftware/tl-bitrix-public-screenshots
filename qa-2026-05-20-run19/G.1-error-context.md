# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: G.1-bizproc-robot.spec.ts >> G.1 — Deal automation lists "Send WhatsApp (TimelinesAI)" robot
- Location: tests\e2e-playwright\specs\G.1-bizproc-robot.spec.ts:54:1

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByText(/send whatsapp.*timelinesai|timelinesai.*whatsapp|отправить whatsapp.*timelinesai/i).first()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByText(/send whatsapp.*timelinesai|timelinesai.*whatsapp|отправить whatsapp.*timelinesai/i).first()

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - group [ref=e2]
  - dialog "Sales automation" [active] [ref=e6]:
    - iframe [ref=e9]:
      - generic [active] [ref=f2e1]:
        - generic [ref=f2e3]:
          - generic [ref=f2e4]:
            - generic [ref=f2e6]:
              - generic [ref=f2e9]:
                - generic [ref=f2e10]: Sales automation
                - button "Add current page to left menu" [ref=f2e11] [cursor=pointer]
              - generic [ref=f2e13]:
                - generic [ref=f2e14]:
                  - button "Extensions" [ref=f2e15] [cursor=pointer]:
                    - generic [ref=f2e16]: Extensions
                  - button [ref=f2e17] [cursor=pointer]
                - button "Test mode" [ref=f2e18] [cursor=pointer]:
                  - generic [ref=f2e20]: Test mode
            - navigation [ref=f2e22]:
              - list [ref=f2e23]:
                - listitem [ref=f2e24]:
                  - button "Automation rules" [ref=f2e25] [cursor=pointer]:
                    - generic [ref=f2e28]: Automation rules
                - listitem [ref=f2e29]:
                  - button "Variables" [ref=f2e30] [cursor=pointer]:
                    - generic [ref=f2e33]: Variables
                - listitem [ref=f2e34]:
                  - button "Constants" [ref=f2e35] [cursor=pointer]:
                    - generic [ref=f2e38]: Constants
                - listitem [ref=f2e39]:
                  - button "Test logs" [ref=f2e40] [cursor=pointer]:
                    - generic [ref=f2e43]: Test logs
          - generic [ref=f2e46]:
            - generic [ref=f2e48]:
              - generic [ref=f2e52]: Automation rules and triggers
              - generic [ref=f2e53]:
                - button "Create" [ref=f2e54] [cursor=pointer]:
                  - generic [ref=f2e56]: Create
                - button "Default pipeline" [ref=f2e57] [cursor=pointer]:
                  - generic [ref=f2e59]: Default pipeline
              - textbox "search" [ref=f2e64]
            - generic [ref=f2e65]:
              - generic [ref=f2e67]:
                - generic [ref=f2e68]:
                  - generic [ref=f2e69]: New
                  - generic [ref=f2e72] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e73]:
                  - generic [ref=f2e74]: Create papers
                  - generic [ref=f2e77] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e78]:
                  - generic [ref=f2e79]: Invoice
                  - generic [ref=f2e82] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e83]:
                  - generic [ref=f2e84]: In progress
                  - generic [ref=f2e87] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e88]:
                  - generic [ref=f2e89]: Final invoice
                  - generic [ref=f2e92] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e93]:
                  - generic [ref=f2e94]: Deal won
                  - generic [ref=f2e97] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e98]:
                  - generic [ref=f2e99]: Deal lost
                  - generic [ref=f2e102] [cursor=pointer]:
                    - generic: add
                - generic [ref=f2e103]:
                  - generic [ref=f2e104]: Analyze failure
                  - generic [ref=f2e107] [cursor=pointer]:
                    - generic: add
                - link [ref=f2e108] [cursor=pointer]:
                  - /url: /crm/configs/status/?ACTIVE_TAB=status_tab_DEAL_STAGE
              - generic [ref=f2e111]: Triggers
              - generic [ref=f2e124]:
                - generic [ref=f2e126]: Automation rules
                - generic [ref=f2e130]:
                  - generic [ref=f2e131]:
                    - generic [ref=f2e132]:
                      - generic [ref=f2e133]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e134]:
                          - generic "immediately" [ref=f2e136] [cursor=pointer]
                          - generic "Notification" [ref=f2e138]
                          - generic [ref=f2e139]:
                            - generic [ref=f2e140]: "to:"
                            - generic "Responsible person" [ref=f2e141] [cursor=pointer]
                        - generic [ref=f2e144] [cursor=pointer]: actions
                        - generic [ref=f2e145] [cursor=pointer]: edit
                      - generic [ref=f2e146]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e147]:
                          - generic "1 day, after previous" [ref=f2e149] [cursor=pointer]
                          - generic "Notification" [ref=f2e151]
                          - generic [ref=f2e152]:
                            - generic [ref=f2e153]: "to:"
                            - generic "Responsible person" [ref=f2e154] [cursor=pointer]
                        - generic [ref=f2e157] [cursor=pointer]: actions
                        - generic [ref=f2e158] [cursor=pointer]: edit
                      - generic [ref=f2e159]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e160]:
                          - generic "3 days" [ref=f2e162] [cursor=pointer]
                          - generic "Control" [ref=f2e164]
                          - generic [ref=f2e165]:
                            - generic [ref=f2e166]: "to:"
                            - generic "To supervisor" [ref=f2e167] [cursor=pointer]
                        - generic [ref=f2e170] [cursor=pointer]: actions
                        - generic [ref=f2e171] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e172] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e173] [cursor=pointer]: Group actions
                  - generic [ref=f2e174]:
                    - generic [ref=f2e175]:
                      - generic [ref=f2e176]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e177]:
                          - generic "immediately" [ref=f2e179] [cursor=pointer]
                          - generic "Notification" [ref=f2e181]
                          - generic [ref=f2e182]:
                            - generic [ref=f2e183]: "to:"
                            - generic "Responsible person" [ref=f2e184] [cursor=pointer]
                        - generic [ref=f2e187] [cursor=pointer]: actions
                        - generic [ref=f2e188] [cursor=pointer]: edit
                      - generic [ref=f2e189]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e190]:
                          - generic "2 days" [ref=f2e192] [cursor=pointer]
                          - generic "Notification" [ref=f2e194]
                          - generic [ref=f2e195]:
                            - generic [ref=f2e196]: "to:"
                            - generic "Responsible person" [ref=f2e197] [cursor=pointer]
                        - generic [ref=f2e200] [cursor=pointer]: actions
                        - generic [ref=f2e201] [cursor=pointer]: edit
                      - generic [ref=f2e202]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e203]:
                          - generic "3 days" [ref=f2e205] [cursor=pointer]
                          - generic "Control" [ref=f2e207]
                          - generic [ref=f2e208]:
                            - generic [ref=f2e209]: "to:"
                            - generic "To supervisor" [ref=f2e210] [cursor=pointer]
                        - generic [ref=f2e213] [cursor=pointer]: actions
                        - generic [ref=f2e214] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e215] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e216] [cursor=pointer]: Group actions
                  - generic [ref=f2e217]:
                    - generic [ref=f2e218]:
                      - generic [ref=f2e219]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e220]:
                          - generic "immediately" [ref=f2e222] [cursor=pointer]
                          - generic "Notification" [ref=f2e224]
                          - generic [ref=f2e225]:
                            - generic [ref=f2e226]: "to:"
                            - generic "Responsible person" [ref=f2e227] [cursor=pointer]
                        - generic [ref=f2e230] [cursor=pointer]: actions
                        - generic [ref=f2e231] [cursor=pointer]: edit
                      - generic [ref=f2e232]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e233]:
                          - generic "2 days" [ref=f2e235] [cursor=pointer]
                          - generic "Schedule a call" [ref=f2e237]
                          - generic [ref=f2e238]:
                            - generic [ref=f2e239]: "to:"
                            - generic "Responsible person" [ref=f2e240] [cursor=pointer]
                        - generic [ref=f2e243] [cursor=pointer]: actions
                        - generic [ref=f2e244] [cursor=pointer]: edit
                      - generic [ref=f2e245]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e246]:
                          - generic "3 days, after previous" [ref=f2e248] [cursor=pointer]
                          - generic "Control" [ref=f2e250]
                          - generic [ref=f2e251]:
                            - generic [ref=f2e252]: "to:"
                            - generic "To supervisor" [ref=f2e253] [cursor=pointer]
                        - generic [ref=f2e256] [cursor=pointer]: actions
                        - generic [ref=f2e257] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e258] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e259] [cursor=pointer]: Group actions
                  - generic [ref=f2e260]:
                    - generic [ref=f2e261]:
                      - generic [ref=f2e262]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e263]:
                          - generic "immediately" [ref=f2e265] [cursor=pointer]
                          - generic "Notification" [ref=f2e267]
                          - generic [ref=f2e268]:
                            - generic [ref=f2e269]: "to:"
                            - generic "Responsible person" [ref=f2e270] [cursor=pointer]
                        - generic [ref=f2e273] [cursor=pointer]: actions
                        - generic [ref=f2e274] [cursor=pointer]: edit
                      - generic [ref=f2e275]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e276]:
                          - generic "4 days" [ref=f2e278] [cursor=pointer]
                          - generic "Control" [ref=f2e280]
                          - generic [ref=f2e281]:
                            - generic [ref=f2e282]: "to:"
                            - generic "To supervisor" [ref=f2e283] [cursor=pointer]
                        - generic [ref=f2e286] [cursor=pointer]: actions
                        - generic [ref=f2e287] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e288] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e289] [cursor=pointer]: Group actions
                  - generic [ref=f2e290]:
                    - generic [ref=f2e291]:
                      - generic [ref=f2e292]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e293]:
                          - generic "immediately" [ref=f2e295] [cursor=pointer]
                          - generic "Notification" [ref=f2e297]
                          - generic [ref=f2e298]:
                            - generic [ref=f2e299]: "to:"
                            - generic "Responsible person" [ref=f2e300] [cursor=pointer]
                        - generic [ref=f2e303] [cursor=pointer]: actions
                        - generic [ref=f2e304] [cursor=pointer]: edit
                      - generic [ref=f2e305]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e306]:
                          - generic "2 days" [ref=f2e308] [cursor=pointer]
                          - generic "Schedule a call" [ref=f2e310]
                          - generic [ref=f2e311]:
                            - generic [ref=f2e312]: "to:"
                            - generic "Responsible person" [ref=f2e313] [cursor=pointer]
                        - generic [ref=f2e316] [cursor=pointer]: actions
                        - generic [ref=f2e317] [cursor=pointer]: edit
                      - generic [ref=f2e318]:
                        - generic:
                          - checkbox
                        - generic [ref=f2e319]:
                          - generic "1 day, after previous" [ref=f2e321] [cursor=pointer]
                          - generic "Notification" [ref=f2e323]
                          - generic [ref=f2e324]:
                            - generic [ref=f2e325]: "to:"
                            - generic "Responsible person" [ref=f2e326] [cursor=pointer]
                        - generic [ref=f2e329] [cursor=pointer]: actions
                        - generic [ref=f2e330] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e331] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e332] [cursor=pointer]: Group actions
                  - generic [ref=f2e333]:
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e334] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e335] [cursor=pointer]: Group actions
                  - generic [ref=f2e336]:
                    - generic [ref=f2e338]:
                      - generic:
                        - checkbox
                      - generic [ref=f2e339]:
                        - generic "immediately" [ref=f2e341] [cursor=pointer]
                        - generic "Control" [ref=f2e343]
                        - generic [ref=f2e344]:
                          - generic [ref=f2e345]: "to:"
                          - generic "To supervisor" [ref=f2e346] [cursor=pointer]
                      - generic [ref=f2e349] [cursor=pointer]: actions
                      - generic [ref=f2e350] [cursor=pointer]: edit
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e351] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e352] [cursor=pointer]: Group actions
                  - generic [ref=f2e353]:
                    - generic:
                      - link "Edit in Workflow Designer" [ref=f2e354] [cursor=pointer]:
                        - /url: "#"
                      - generic [ref=f2e355] [cursor=pointer]: Group actions
        - generic:
          - generic:
            - generic: "Selected:"
          - generic:
            - generic:
              - generic:
                - img
              - generic: select all in stage
            - generic:
              - generic:
                - img
              - generic: COPY
            - generic:
              - generic:
                - img
              - generic: MOVE
            - generic:
              - generic:
                - img
              - generic: DISABLE
            - generic:
              - generic:
                - img
              - generic: DELETE
        - dialog [ref=f2e356]:
          - generic [ref=f2e358]:
            - generic [ref=f2e359]: Smarter Business
            - generic [ref=f2e361]: Improve your business performance while saving on operational costs and avoiding overblown staff! The CRM will remind you of things that need to be done or even do it on its own. Never miss a lead!
            - link "Learn more" [ref=f2e362] [cursor=pointer]:
              - /url: ""
          - button "Close" [ref=f2e363] [cursor=pointer]
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
            - listitem "Deals" [ref=e229]:
              - link "Deals" [ref=e230] [cursor=pointer]:
                - /url: /crm/deal/kanban/category/0/
                - generic [ref=e233]: Deals
            - listitem [ref=e234]:
              - button "Inventory" [ref=e235] [cursor=pointer]:
                - generic [ref=e238]: Inventory
            - listitem [ref=e240]:
              - button "Customers" [ref=e241] [cursor=pointer]:
                - generic [ref=e244]: Customers
            - listitem [ref=e246]:
              - button "New Sales" [ref=e247] [cursor=pointer]:
                - generic [ref=e248]:
                  - generic [ref=e249]: New
                  - generic [ref=e251]: Sales
            - listitem [ref=e253]:
              - button "Analytics" [ref=e254] [cursor=pointer]:
                - generic [ref=e257]: Analytics
            - listitem [ref=e259]:
              - button "More" [ref=e260] [cursor=pointer]:
                - generic [ref=e263]: More
        - generic [ref=e265]:
          - search [ref=e268]:
            - textbox [disabled] [ref=e269]:
              - /placeholder: find people, documents, and more
            - button "Search" [ref=e270]
          - link "Bitrix 24" [ref=e274] [cursor=pointer]:
            - /url: /
            - generic [ref=e275]:
              - generic [ref=e276]: Bitrix
              - generic [ref=e277]: "24"
          - button [ref=e278] [cursor=pointer]
          - generic [ref=e280]:
            - button "Invite" [ref=e282] [cursor=pointer]: Invite
            - button "Buy Now" [ref=e284] [cursor=pointer]: Buy Now
            - button "Helpdesk 6" [ref=e286] [cursor=pointer]:
              - text: Helpdesk
              - generic [ref=e290]: "6"
    - button "Profile" [ref=e292] [cursor=pointer]
    - main [ref=e298]:
      - generic [ref=e299]:
        - generic [ref=e300]:
          - generic [ref=e302]:
            - generic [ref=e305]:
              - generic [ref=e306]: Deals
              - button "Add current page to left menu" [ref=e307] [cursor=pointer]
            - generic [ref=e309]:
              - generic [ref=e310]:
                - link "Create" [ref=e311] [cursor=pointer]:
                  - /url: /crm/deal/details/0/?st%5Btool%5D=crm&st%5Bc_section%5D=deal_section&st%5Bc_sub_section%5D=list&st%5Bc_element%5D=create_button&st%5Bp1%5D=crmMode_simple&st%5Bcategory%5D=entity_operations&st%5Bevent%5D=entity_add_open&st%5Btype%5D=deal&category_id=0
                  - generic [ref=e312]: Create
                - button [ref=e313] [cursor=pointer]
              - button "Default pipeline" [ref=e314] [cursor=pointer]:
                - generic [ref=e316]: Default pipeline
            - generic [ref=e319]:
              - generic [ref=e321]: Deals in progress
              - textbox "search" [ref=e323]
            - button [ref=e328] [cursor=pointer]
          - generic [ref=e331]:
            - generic [ref=e333]:
              - generic [ref=e335] [cursor=pointer]: Kanban
              - generic:
                - generic: List
              - generic [ref=e337] [cursor=pointer]: Activities
              - generic [ref=e339] [cursor=pointer]: Calendar
            - generic [ref=e341]:
              - generic [ref=e342] [cursor=pointer]:
                - generic [ref=e346]: "0"
                - generic [ref=e347]: Inbound
              - generic [ref=e348] [cursor=pointer]:
                - generic [ref=e352]: "0"
                - generic [ref=e353]: Planned
              - generic [ref=e354] [cursor=pointer]:
                - generic [ref=e355]: More
                - generic [ref=e359]: "0"
            - generic [ref=e362]:
              - generic [ref=e365] [cursor=pointer]: Repeat sales
              - link "Automation rules" [ref=e366] [cursor=pointer]:
                - /url: /crm/deal/automation/0/
                - generic [ref=e368]: Automation rules
              - generic [ref=e369]:
                - button "Extensions" [ref=e370] [cursor=pointer]:
                  - generic [ref=e371]: Extensions
                - button [ref=e372] [cursor=pointer]
        - generic [ref=e376]:
          - generic [ref=e377]:
            - table [ref=e383]:
              - rowgroup [ref=e384]:
                - row "Deal Stage Activity Client Amount/Currency Responsible Created Customer journey" [ref=e385]:
                  - columnheader [ref=e386]:
                    - checkbox [ref=e389]
                  - columnheader [ref=e390]
                  - columnheader "Deal" [ref=e392] [cursor=pointer]:
                    - generic [ref=e395]: Deal
                  - columnheader "Stage" [ref=e397] [cursor=pointer]:
                    - generic [ref=e400]: Stage
                  - columnheader "Activity" [ref=e402] [cursor=pointer]:
                    - generic [ref=e405]: Activity
                  - columnheader "Client" [ref=e407] [cursor=pointer]:
                    - generic [ref=e410]: Client
                  - columnheader "Amount/Currency" [ref=e412] [cursor=pointer]:
                    - generic [ref=e415]: Amount/Currency
                  - columnheader "Responsible" [ref=e417] [cursor=pointer]:
                    - generic [ref=e420]: Responsible
                  - columnheader "Created" [ref=e422] [cursor=pointer]:
                    - generic [ref=e425]: Created
                  - columnheader "Customer journey" [ref=e428]:
                    - generic [ref=e431]: Customer journey
                  - columnheader
              - rowgroup [ref=e433]:
                - 'row "WhatsApp: Test Sales New No activities $0 Anton Patrai 05/17/2026 Other traffic Application" [ref=e434]':
                  - cell [ref=e435]:
                    - generic [ref=e436]:
                      - checkbox
                  - cell [ref=e437]:
                    - link [ref=e439] [cursor=pointer]:
                      - /url: "#"
                  - 'cell "WhatsApp: Test Sales" [ref=e440]':
                    - generic [ref=e443]:
                      - 'link "WhatsApp: Test" [ref=e445] [cursor=pointer]':
                        - /url: /crm/deal/details/7/
                      - generic [ref=e446]: Sales
                  - cell "New" [ref=e447]:
                    - generic [ref=e449]:
                      - table [ref=e451]:
                        - rowgroup [ref=e452]:
                          - row [ref=e453]:
                            - cell [ref=e454]
                            - cell [ref=e456]
                            - cell [ref=e458]
                            - cell [ref=e460]
                            - cell [ref=e462]
                            - cell [ref=e464]
                      - generic [ref=e466]: New
                  - cell "No activities" [ref=e467]:
                    - generic [ref=e470]: No activities
                  - cell [ref=e471]
                  - cell "$0" [ref=e473]:
                    - generic [ref=e475]: $0
                  - cell "Anton Patrai" [ref=e476]:
                    - link "Anton Patrai" [ref=e480] [cursor=pointer]:
                      - /url: ""
                      - generic [ref=e483]: Anton Patrai
                  - cell "05/17/2026" [ref=e484]:
                    - generic [ref=e486]: 05/17/2026
                  - cell "Other traffic Application" [ref=e487]:
                    - generic [ref=e490]:
                      - text: Other traffic
                      - text: Application
                  - cell
                - 'row "WhatsApp: F16 Header Verify Sales New No activities F16 Header Verify $0 Anton Patrai 05/14/2026 Other traffic Application" [ref=e494]':
                  - cell [ref=e495]:
                    - generic [ref=e496]:
                      - checkbox
                  - cell [ref=e497]:
                    - link [ref=e499] [cursor=pointer]:
                      - /url: "#"
                  - 'cell "WhatsApp: F16 Header Verify Sales" [ref=e500]':
                    - generic [ref=e503]:
                      - 'link "WhatsApp: F16 Header Verify" [ref=e505] [cursor=pointer]':
                        - /url: /crm/deal/details/5/
                      - generic [ref=e506]: Sales
                  - cell "New" [ref=e507]:
                    - generic [ref=e509]:
                      - table [ref=e511]:
                        - rowgroup [ref=e512]:
                          - row [ref=e513]:
                            - cell [ref=e514]
                            - cell [ref=e516]
                            - cell [ref=e518]
                            - cell [ref=e520]
                            - cell [ref=e522]
                            - cell [ref=e524]
                      - generic [ref=e526]: New
                  - cell "No activities" [ref=e527]:
                    - generic [ref=e530]: No activities
                  - cell "F16 Header Verify" [ref=e531]:
                    - link "F16 Header Verify" [ref=e536] [cursor=pointer]:
                      - /url: /crm/contact/details/5/
                  - cell "$0" [ref=e537]:
                    - generic [ref=e539]: $0
                  - cell "Anton Patrai" [ref=e540]:
                    - link "Anton Patrai" [ref=e544] [cursor=pointer]:
                      - /url: ""
                      - generic [ref=e547]: Anton Patrai
                  - cell "05/14/2026" [ref=e548]:
                    - generic [ref=e550]: 05/14/2026
                  - cell "Other traffic Application" [ref=e551]:
                    - generic [ref=e554]:
                      - text: Other traffic
                      - text: Application
                  - cell
                - 'row "WhatsApp: F16 Synthetic Sender Sales New No activities F16 Synthetic Sender $0 Anton Patrai 05/14/2026 Other traffic Application" [ref=e558]':
                  - cell [ref=e559]:
                    - generic [ref=e560]:
                      - checkbox
                  - cell [ref=e561]:
                    - link [ref=e563] [cursor=pointer]:
                      - /url: "#"
                  - 'cell "WhatsApp: F16 Synthetic Sender Sales" [ref=e564]':
                    - generic [ref=e567]:
                      - 'link "WhatsApp: F16 Synthetic Sender" [ref=e569] [cursor=pointer]':
                        - /url: /crm/deal/details/3/
                      - generic [ref=e570]: Sales
                  - cell "New" [ref=e571]:
                    - generic [ref=e573]:
                      - table [ref=e575]:
                        - rowgroup [ref=e576]:
                          - row [ref=e577]:
                            - cell [ref=e578]
                            - cell [ref=e580]
                            - cell [ref=e582]
                            - cell [ref=e584]
                            - cell [ref=e586]
                            - cell [ref=e588]
                      - generic [ref=e590]: New
                  - cell "No activities" [ref=e591]:
                    - generic [ref=e594]: No activities
                  - cell "F16 Synthetic Sender" [ref=e595]:
                    - link "F16 Synthetic Sender" [ref=e600] [cursor=pointer]:
                      - /url: /crm/contact/details/3/
                  - cell "$0" [ref=e601]:
                    - generic [ref=e603]: $0
                  - cell "Anton Patrai" [ref=e604]:
                    - link "Anton Patrai" [ref=e608] [cursor=pointer]:
                      - /url: ""
                      - generic [ref=e611]: Anton Patrai
                  - cell "05/14/2026" [ref=e612]:
                    - generic [ref=e614]: 05/14/2026
                  - cell "Other traffic Application" [ref=e615]:
                    - generic [ref=e618]:
                      - text: Other traffic
                      - text: Application
                  - cell
                - 'row "WhatsApp: Test Sales New No activities Sarah Johnson $0 Anton Patrai 05/12/2026 Other traffic Application" [ref=e622]':
                  - cell [ref=e623]:
                    - generic [ref=e624]:
                      - checkbox
                  - cell [ref=e625]:
                    - link [ref=e627] [cursor=pointer]:
                      - /url: "#"
                  - 'cell "WhatsApp: Test Sales" [ref=e628]':
                    - generic [ref=e631]:
                      - 'link "WhatsApp: Test" [ref=e633] [cursor=pointer]':
                        - /url: /crm/deal/details/1/
                      - generic [ref=e634]: Sales
                  - cell "New" [ref=e635]:
                    - generic [ref=e637]:
                      - table [ref=e639]:
                        - rowgroup [ref=e640]:
                          - row [ref=e641]:
                            - cell [ref=e642]
                            - cell [ref=e644]
                            - cell [ref=e646]
                            - cell [ref=e648]
                            - cell [ref=e650]
                            - cell [ref=e652]
                      - generic [ref=e654]: New
                  - cell "No activities" [ref=e655]:
                    - generic [ref=e658]: No activities
                  - cell "Sarah Johnson" [ref=e659]:
                    - link "Sarah Johnson" [ref=e664] [cursor=pointer]:
                      - /url: /crm/contact/details/1/
                  - cell "$0" [ref=e665]:
                    - generic [ref=e667]: $0
                  - cell "Anton Patrai" [ref=e668]:
                    - link "Anton Patrai" [ref=e672] [cursor=pointer]:
                      - /url: ""
                      - generic [ref=e675]: Anton Patrai
                  - cell "05/12/2026" [ref=e676]:
                    - generic [ref=e678]: 05/12/2026
                  - cell "Other traffic Application" [ref=e679]:
                    - generic [ref=e682]:
                      - text: Other traffic
                      - text: Application
                  - cell
            - generic [ref=e686]:
              - table [ref=e689]:
                - rowgroup [ref=e690]:
                  - 'row "Selected: 0 / 4 Total: Show quantity Pages:1 Records: 20" [ref=e691]':
                    - 'cell "Selected: 0 / 4" [ref=e692]':
                      - generic [ref=e693]:
                        - text: "Selected:"
                        - generic [ref=e694]: 0 / 4
                    - 'cell "Total: Show quantity" [ref=e695]':
                      - generic [ref=e697]:
                        - text: "Total:"
                        - link "Show quantity" [ref=e698] [cursor=pointer]:
                          - /url: "#"
                    - cell "Pages:1" [ref=e699]:
                      - generic [ref=e700]: Pages:1
                    - 'cell "Records: 20" [ref=e701]':
                      - generic [ref=e702]:
                        - text: "Records:"
                        - generic [ref=e703] [cursor=pointer]:
                          - generic: "20"
              - table [ref=e706]:
                - rowgroup [ref=e707]:
                  - 'row "Delete Edit Start dialing Select action For All Selected: 0 / 4" [ref=e708]':
                    - cell "Delete Edit Start dialing Select action For All" [ref=e709]:
                      - generic:
                        - generic "Delete"
                      - generic:
                        - generic "Edit selected items": Edit
                      - generic:
                        - generic "Start dialing"
                      - generic:
                        - generic:
                          - generic: Select action
                      - generic [ref=e710]:
                        - checkbox "For All" [ref=e712]
                        - generic [ref=e714]: For All
                    - 'cell "Selected: 0 / 4" [ref=e715]':
                      - generic [ref=e716]:
                        - text: "Selected:"
                        - generic [ref=e717]: 0 / 4
          - iframe
    - contentinfo [ref=e718]:
      - generic [ref=e719]:
        - generic [ref=e720]:
          - link "Bitrix 24" [ref=e722] [cursor=pointer]:
            - /url: https://www.bitrix24.com
            - generic [ref=e723]:
              - generic [ref=e724]: Bitrix
              - generic [ref=e725]: "24"
          - button "English" [ref=e727] [cursor=pointer]
        - generic [ref=e728]: © 2026 Bitrix24
        - generic [ref=e729]:
          - button "Implementation request" [ref=e730] [cursor=pointer]
          - button "Themes" [ref=e731] [cursor=pointer]
          - button "Print" [ref=e732] [cursor=pointer]
    - region "Chat bar" [ref=e734]:
      - generic [ref=e736]:
        - generic [ref=e741] [cursor=pointer]: "9"
        - generic [ref=e748]:
          - generic "General chat" [ref=e752] [cursor=pointer]
          - generic [ref=e756] [cursor=pointer]:
            - generic "Bitrix24 Support" [ref=e757]:
              - img "Bitrix24 Support" [ref=e758]
            - generic [ref=e759]: "1"
          - generic "Company News" [ref=e763] [cursor=pointer]
          - generic "My Notes" [ref=e768] [cursor=pointer]
  - generic:
    - generic:
      - generic:
        - generic: The server connection is successfully established
```

# Test source

```ts
  12  |  * `tlai_send_whatsapp`, NAME "Send WhatsApp message (TimelinesAI)".
  13  |  *
  14  |  * Why this spec was re-fixed (#426 run-17 reopen):
  15  |  *   The previous version navigated to `/crm/deal/details/<id>/` and tried to
  16  |  *   locate an "Automation" tab at page level. On the current Bitrix UI that
  17  |  *   URL opens the deal card as a side-panel slider whose CONTENT is rendered
  18  |  *   INSIDE an `<iframe>` (the run-17 `error-context.md` page snapshot shows
  19  |  *   the Automation link as `f1e83` inside the dialog iframe, with href
  20  |  *   `/crm/deal/automation/0/?id=1`). The spec's page-level tab-strip locator
  21  |  *   never found that link.
  22  |  *
  23  |  *   On top of that, the spec called `installSidePanelOverlayHandler` BEFORE
  24  |  *   `goto`. Because the deal card IS a side-panel slider, the auto-handler
  25  |  *   kept dismissing it (`18× found locator(...side-panel.--open),
  26  |  *   intercepting action to run the handler`) — same failure shape PR #489
  27  |  *   (F.1/F.2) and PR #490 (D.1/D.2/D.3) fixed for the connector-settings
  28  |  *   slider. The re-arming handler is INCOMPATIBLE with any flow that
  29  |  *   intentionally opens a side-panel.
  30  |  *
  31  |  * Fix shape (mirrors PR #489/#490):
  32  |  *   - Navigate directly to the automation builder top-level URL
  33  |  *     (`/crm/deal/automation/0/?id=<dealId>`) — bypasses the deal-card
  34  |  *     slider/iframe entirely. The robot picker renders on this page.
  35  |  *   - Do NOT install the re-arming auto-handler. Use a one-shot dismiss
  36  |  *     for any pre-existing marketplace slider before navigation.
  37  |  *   - Try a small set of robust strategies to surface the robot row in the
  38  |  *     designer (clicking an "Add" affordance if one is visible, then
  39  |  *     text-matching the robot NAME). The NAME text "Send WhatsApp message
  40  |  *     (TimelinesAI)" comes directly from `src/lib/bitrix/bizproc.ts` and is
  41  |  *     the canonical production string.
  42  |  */
  43  | 
  44  | import { test, expect } from '@playwright/test';
  45  | import { pinScreenshot } from '../screenshot-helper.js';
  46  | import { dismissSidePanelOverlay } from '../lib/preflight.js';
  47  | 
  48  | // Production robot NAME (en + ru) from src/lib/bitrix/bizproc.ts. The
  49  | // designer surfaces one of these per the portal's language setting; the
  50  | // regex tolerates either ordering and either locale.
  51  | const ROBOT_NAME_RE =
  52  |   /send whatsapp.*timelinesai|timelinesai.*whatsapp|отправить whatsapp.*timelinesai/i;
  53  | 
  54  | test('G.1 — Deal automation lists "Send WhatsApp (TimelinesAI)" robot', async ({ page }, testInfo) => {
  55  |   const portal = process.env.BITRIX_PORTAL_URL!;
  56  |   const dealId = process.env.E2E_BITRIX_TEST_DEAL_ID ?? '1';
  57  | 
  58  |   // Land on the portal first so we can dismiss any leftover marketplace
  59  |   // slider ONCE before navigating. Mirrors the openConnectorSettings
  60  |   // (PR #490) / openConnectorSettingsFrame (PR #489) pattern: pre-existing
  61  |   // sliders intercept clicks on the new page, but we MUST NOT install the
  62  |   // re-arming handler — the automation builder itself opens sub-sliders
  63  |   // (the robot picker) and we want those to stay open.
  64  |   await page.goto(`${portal}/`);
  65  |   await dismissSidePanelOverlay(page);
  66  | 
  67  |   // Go straight to the Deal automation builder. URL extracted from the
  68  |   // run-17 page snapshot (`f1e83` link's href). Category `0` is the
  69  |   // default pipeline that every Bitrix portal ships with; the test deal
  70  |   // id=1 lives there. Direct nav avoids the deal-card slider/iframe
  71  |   // entirely so we can operate against top-level Playwright locators.
  72  |   await page.goto(`${portal}/crm/deal/automation/0/?id=${dealId}`);
  73  |   await pinScreenshot(page, '01-automation-builder', testInfo);
  74  | 
  75  |   // The automation builder may render in one of two shells depending on
  76  |   // the portal's feature flag rollout:
  77  |   //   - Kanban-style stage columns with a "+" / "Add" trigger on each
  78  |   //     column header (the legacy + most-common surface).
  79  |   //   - A flat list of stages, each with an "Add a robot" button.
  80  |   // Both ultimately open a right-side picker (slider) containing the
  81  |   // robot catalog. We try the first visible "add"-style affordance and
  82  |   // soft-fail if none is visible — some portal layouts auto-open the
  83  |   // picker on nav, and even when they don't the registered robot is
  84  |   // listed in the designer's collapsed catalog which `getByText` can
  85  |   // still match.
  86  |   const addBtn = page
  87  |     .locator(
  88  |       [
  89  |         '.bizproc-automation-robot-list-add',
  90  |         '.crm-kanban-add-trigger',
  91  |         '.ui-btn-add',
  92  |         'button:has-text("Add a robot")',
  93  |         'button:has-text("Add robot")',
  94  |         'button:has-text("Add")',
  95  |       ].join(', '),
  96  |     )
  97  |     .first();
  98  |   if (await addBtn.isVisible().catch(() => false)) {
  99  |     await addBtn.click().catch(() => {
  100 |       /* portal layouts differ; soft-fail is fine — robot row may already be in DOM */
  101 |     });
  102 |   }
  103 |   await pinScreenshot(page, '02-picker-open', testInfo);
  104 | 
  105 |   // The robot row. Bitrix lists registered REST robots under a "REST" or
  106 |   // "Marketplace" category in the picker. We don't depend on the category
  107 |   // header — just the visible NAME text registered via bizproc.robot.add.
  108 |   // `getByText` returns the first text match; combine with `.first()`
  109 |   // defensively because the designer may render both a card and a
  110 |   // tooltip for the same robot.
  111 |   const robotRow = page.getByText(ROBOT_NAME_RE).first();
> 112 |   await expect(robotRow).toBeVisible({ timeout: 15_000 });
      |                          ^ Error: expect(locator).toBeVisible() failed
  113 |   await pinScreenshot(page, '03-robot-visible', testInfo);
  114 | });
  115 | 
```