# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: I.1-audit-log-csv.spec.ts >> I.1 — audit-log CSV export downloads a non-empty file
- Location: tests\e2e-playwright\specs\I.1-audit-log-csv.spec.ts:33:1

# Error details

```
TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
Call log:
  - waiting for locator('#a11y-slider-container .side-panel.--open').first().locator('iframe[src*="tl-bitrix-integration.netlify.app"]').first()

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - group [ref=e2]
  - dialog "WhatsApp audit log" [active] [ref=e6]:
    - iframe [ref=e9]:
      - iframe [ref=f1e7]:
        - generic [active] [ref=f2e1]:
          - heading "TimelinesAI delivery log" [level=1] [ref=f2e2]
          - paragraph [ref=f2e3]:
            - text: Connection state changes and webhook processing for
            - code
            - text: . Useful for confirming an install or diagnosing delivery delays.
          - generic [ref=f2e4]:
            - generic [ref=f2e5]:
              - generic [ref=f2e6]: "Kind:"
              - button "All events" [ref=f2e8] [cursor=pointer]
              - button "Connection" [ref=f2e10] [cursor=pointer]
              - button "Webhook" [ref=f2e12] [cursor=pointer]
            - generic [ref=f2e13]:
              - generic [ref=f2e14]: "Range:"
              - button "Last 24h" [ref=f2e16] [cursor=pointer]
              - button "Last 7 days" [ref=f2e18] [cursor=pointer]
              - button "Last 30 days" [ref=f2e20] [cursor=pointer]
              - button "All time" [ref=f2e22] [cursor=pointer]
            - button "Download CSV" [ref=f2e24] [cursor=pointer]
          - table [ref=f2e25]:
            - rowgroup [ref=f2e26]:
              - row "When (UTC) Kind Name Status User Detail" [ref=f2e27]:
                - columnheader "When (UTC)" [ref=f2e28]
                - columnheader "Kind" [ref=f2e29]
                - columnheader "Name" [ref=f2e30]
                - columnheader "Status" [ref=f2e31]
                - columnheader "User" [ref=f2e32]
                - columnheader "Detail" [ref=f2e33]
            - rowgroup [ref=f2e34]:
              - row "2026-05-20 18:55:29 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e35]:
                - cell "2026-05-20 18:55:29" [ref=f2e36]
                - cell "Connection" [ref=f2e37]
                - cell "install" [ref=f2e38]
                - cell "complete" [ref=f2e39]
                - cell "tl:17278" [ref=f2e40]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e41]
              - row "2026-05-20 18:52:33 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e42]:
                - cell "2026-05-20 18:52:33" [ref=f2e43]
                - cell "Connection" [ref=f2e44]
                - cell "install" [ref=f2e45]
                - cell "complete" [ref=f2e46]
                - cell "tl:17278" [ref=f2e47]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e48]
              - row "2026-05-20 18:23:39 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e49]:
                - cell "2026-05-20 18:23:39" [ref=f2e50]
                - cell "Connection" [ref=f2e51]
                - cell "install" [ref=f2e52]
                - cell "complete" [ref=f2e53]
                - cell "tl:17278" [ref=f2e54]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e55]
              - row "2026-05-20 17:41:39 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e56]:
                - cell "2026-05-20 17:41:39" [ref=f2e57]
                - cell "Connection" [ref=f2e58]
                - cell "install" [ref=f2e59]
                - cell "complete" [ref=f2e60]
                - cell "tl:17278" [ref=f2e61]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e62]
              - 'row "2026-05-20 14:06:31 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e63]':
                - cell "2026-05-20 14:06:31" [ref=f2e64]
                - cell "Webhook" [ref=f2e65]
                - cell "ONCRMDEALUPDATE" [ref=f2e66]
                - cell "processed" [ref=f2e67]
                - cell "bx:1" [ref=f2e68]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e69]'
              - 'row "2026-05-20 14:06:31 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e70]':
                - cell "2026-05-20 14:06:31" [ref=f2e71]
                - cell "Webhook" [ref=f2e72]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e73]
                - cell "processed" [ref=f2e74]
                - cell "bx:1" [ref=f2e75]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e76]'
              - row "2026-05-20 14:04:48 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e77]:
                - cell "2026-05-20 14:04:48" [ref=f2e78]
                - cell "Connection" [ref=f2e79]
                - cell "install" [ref=f2e80]
                - cell "complete" [ref=f2e81]
                - cell "tl:17278" [ref=f2e82]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e83]
              - 'row "2026-05-20 13:25:09 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e84]':
                - cell "2026-05-20 13:25:09" [ref=f2e85]
                - cell "Connection" [ref=f2e86]
                - cell "disconnect" [ref=f2e87]
                - cell "complete" [ref=f2e88]
                - cell "—" [ref=f2e89]
                - 'cell "Disconnected: invalid_grant" [ref=f2e90]'
              - row "2026-05-20 13:24:11 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e91]:
                - cell "2026-05-20 13:24:11" [ref=f2e92]
                - cell "Connection" [ref=f2e93]
                - cell "install" [ref=f2e94]
                - cell "complete" [ref=f2e95]
                - cell "tl:17278" [ref=f2e96]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e97]
              - row "2026-05-20 13:23:41 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e98]:
                - cell "2026-05-20 13:23:41" [ref=f2e99]
                - cell "Connection" [ref=f2e100]
                - cell "install" [ref=f2e101]
                - cell "complete" [ref=f2e102]
                - cell "tl:17278" [ref=f2e103]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e104]
              - 'row "2026-05-20 12:29:05 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e105]':
                - cell "2026-05-20 12:29:05" [ref=f2e106]
                - cell "Connection" [ref=f2e107]
                - cell "disconnect" [ref=f2e108]
                - cell "complete" [ref=f2e109]
                - cell "—" [ref=f2e110]
                - 'cell "Disconnected: invalid_grant" [ref=f2e111]'
              - row "2026-05-20 12:27:33 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e112]:
                - cell "2026-05-20 12:27:33" [ref=f2e113]
                - cell "Connection" [ref=f2e114]
                - cell "install" [ref=f2e115]
                - cell "complete" [ref=f2e116]
                - cell "tl:17278" [ref=f2e117]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e118]
              - 'row "2026-05-20 11:37:17 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e119]':
                - cell "2026-05-20 11:37:17" [ref=f2e120]
                - cell "Connection" [ref=f2e121]
                - cell "disconnect" [ref=f2e122]
                - cell "complete" [ref=f2e123]
                - cell "—" [ref=f2e124]
                - 'cell "Disconnected: invalid_grant" [ref=f2e125]'
              - row "2026-05-20 11:36:00 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e126]:
                - cell "2026-05-20 11:36:00" [ref=f2e127]
                - cell "Connection" [ref=f2e128]
                - cell "install" [ref=f2e129]
                - cell "complete" [ref=f2e130]
                - cell "tl:17278" [ref=f2e131]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e132]
              - 'row "2026-05-20 11:10:52 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e133]':
                - cell "2026-05-20 11:10:52" [ref=f2e134]
                - cell "Connection" [ref=f2e135]
                - cell "disconnect" [ref=f2e136]
                - cell "complete" [ref=f2e137]
                - cell "—" [ref=f2e138]
                - 'cell "Disconnected: invalid_grant" [ref=f2e139]'
              - row "2026-05-20 11:09:26 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e140]:
                - cell "2026-05-20 11:09:26" [ref=f2e141]
                - cell "Connection" [ref=f2e142]
                - cell "install" [ref=f2e143]
                - cell "complete" [ref=f2e144]
                - cell "tl:17278" [ref=f2e145]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e146]
              - 'row "2026-05-20 10:39:27 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e147]':
                - cell "2026-05-20 10:39:27" [ref=f2e148]
                - cell "Connection" [ref=f2e149]
                - cell "disconnect" [ref=f2e150]
                - cell "complete" [ref=f2e151]
                - cell "—" [ref=f2e152]
                - 'cell "Disconnected: invalid_grant" [ref=f2e153]'
              - row "2026-05-20 10:38:09 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e154]:
                - cell "2026-05-20 10:38:09" [ref=f2e155]
                - cell "Connection" [ref=f2e156]
                - cell "install" [ref=f2e157]
                - cell "complete" [ref=f2e158]
                - cell "tl:17278" [ref=f2e159]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e160]
              - 'row "2026-05-20 10:20:26 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e161]':
                - cell "2026-05-20 10:20:26" [ref=f2e162]
                - cell "Connection" [ref=f2e163]
                - cell "disconnect" [ref=f2e164]
                - cell "complete" [ref=f2e165]
                - cell "—" [ref=f2e166]
                - 'cell "Disconnected: invalid_grant" [ref=f2e167]'
              - row "2026-05-20 10:19:07 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e168]:
                - cell "2026-05-20 10:19:07" [ref=f2e169]
                - cell "Connection" [ref=f2e170]
                - cell "install" [ref=f2e171]
                - cell "complete" [ref=f2e172]
                - cell "tl:17278" [ref=f2e173]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e174]
              - 'row "2026-05-20 09:55:41 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e175]':
                - cell "2026-05-20 09:55:41" [ref=f2e176]
                - cell "Connection" [ref=f2e177]
                - cell "disconnect" [ref=f2e178]
                - cell "complete" [ref=f2e179]
                - cell "—" [ref=f2e180]
                - 'cell "Disconnected: invalid_grant" [ref=f2e181]'
              - row "2026-05-20 09:54:18 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e182]:
                - cell "2026-05-20 09:54:18" [ref=f2e183]
                - cell "Connection" [ref=f2e184]
                - cell "install" [ref=f2e185]
                - cell "complete" [ref=f2e186]
                - cell "tl:17278" [ref=f2e187]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e188]
              - 'row "2026-05-19 10:40:31 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e189]':
                - cell "2026-05-19 10:40:31" [ref=f2e190]
                - cell "Webhook" [ref=f2e191]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e192]
                - cell "processed" [ref=f2e193]
                - cell "bx:1" [ref=f2e194]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e195]'
              - 'row "2026-05-19 10:40:31 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e196]':
                - cell "2026-05-19 10:40:31" [ref=f2e197]
                - cell "Webhook" [ref=f2e198]
                - cell "ONCRMDEALUPDATE" [ref=f2e199]
                - cell "processed" [ref=f2e200]
                - cell "bx:1" [ref=f2e201]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e202]'
              - row "2026-05-19 10:37:19 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e203]:
                - cell "2026-05-19 10:37:19" [ref=f2e204]
                - cell "Connection" [ref=f2e205]
                - cell "install" [ref=f2e206]
                - cell "complete" [ref=f2e207]
                - cell "tl:17278" [ref=f2e208]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e209]
              - 'row "2026-05-19 09:31:23 Connection disconnect complete — Disconnected: invalid_grant" [ref=f2e210]':
                - cell "2026-05-19 09:31:23" [ref=f2e211]
                - cell "Connection" [ref=f2e212]
                - cell "disconnect" [ref=f2e213]
                - cell "complete" [ref=f2e214]
                - cell "—" [ref=f2e215]
                - 'cell "Disconnected: invalid_grant" [ref=f2e216]'
              - row "2026-05-19 09:26:01 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e217]:
                - cell "2026-05-19 09:26:01" [ref=f2e218]
                - cell "Connection" [ref=f2e219]
                - cell "install" [ref=f2e220]
                - cell "complete" [ref=f2e221]
                - cell "tl:17278" [ref=f2e222]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e223]
              - row "2026-05-18 21:03:22 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e224]:
                - cell "2026-05-18 21:03:22" [ref=f2e225]
                - cell "Connection" [ref=f2e226]
                - cell "install" [ref=f2e227]
                - cell "complete" [ref=f2e228]
                - cell "tl:17278" [ref=f2e229]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e230]
              - row "2026-05-18 14:25:47 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e231]:
                - cell "2026-05-18 14:25:47" [ref=f2e232]
                - cell "Connection" [ref=f2e233]
                - cell "install" [ref=f2e234]
                - cell "complete" [ref=f2e235]
                - cell "tl:17278" [ref=f2e236]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e237]
              - 'row "2026-05-18 05:55:38 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e238]':
                - cell "2026-05-18 05:55:38" [ref=f2e239]
                - cell "Webhook" [ref=f2e240]
                - cell "ONCRMDEALUPDATE" [ref=f2e241]
                - cell "processed" [ref=f2e242]
                - cell "bx:1" [ref=f2e243]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e244]'
              - 'row "2026-05-18 05:55:37 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e245]':
                - cell "2026-05-18 05:55:37" [ref=f2e246]
                - cell "Webhook" [ref=f2e247]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e248]
                - cell "processed" [ref=f2e249]
                - cell "bx:1" [ref=f2e250]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e251]'
              - 'row "2026-05-18 05:53:39 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e252]':
                - cell "2026-05-18 05:53:39" [ref=f2e253]
                - cell "Webhook" [ref=f2e254]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e255]
                - cell "processed" [ref=f2e256]
                - cell "bx:1" [ref=f2e257]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e258]'
              - 'row "2026-05-18 05:50:54 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e259]':
                - cell "2026-05-18 05:50:54" [ref=f2e260]
                - cell "Webhook" [ref=f2e261]
                - cell "ONCRMDEALUPDATE" [ref=f2e262]
                - cell "processed" [ref=f2e263]
                - cell "bx:1" [ref=f2e264]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e265]'
              - 'row "2026-05-18 05:50:54 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e266]':
                - cell "2026-05-18 05:50:54" [ref=f2e267]
                - cell "Webhook" [ref=f2e268]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e269]
                - cell "processed" [ref=f2e270]
                - cell "bx:1" [ref=f2e271]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e272]'
              - row "2026-05-17 18:57:16 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e273]:
                - cell "2026-05-17 18:57:16" [ref=f2e274]
                - cell "Connection" [ref=f2e275]
                - cell "install" [ref=f2e276]
                - cell "complete" [ref=f2e277]
                - cell "tl:17278" [ref=f2e278]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e279]
              - 'row "2026-05-17 14:02:54 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e280]':
                - cell "2026-05-17 14:02:54" [ref=f2e281]
                - cell "Webhook" [ref=f2e282]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e283]
                - cell "processed" [ref=f2e284]
                - cell "—" [ref=f2e285]
                - 'cell "{\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e286]'
              - 'row "2026-05-17 10:11:22 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e287]':
                - cell "2026-05-17 10:11:22" [ref=f2e288]
                - cell "Webhook" [ref=f2e289]
                - cell "ONCRMDEALUPDATE" [ref=f2e290]
                - cell "processed" [ref=f2e291]
                - cell "bx:1" [ref=f2e292]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e293]'
              - 'row "2026-05-17 10:11:21 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e294]':
                - cell "2026-05-17 10:11:21" [ref=f2e295]
                - cell "Webhook" [ref=f2e296]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e297]
                - cell "processed" [ref=f2e298]
                - cell "bx:1" [ref=f2e299]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e300]'
              - 'row "2026-05-17 10:11:18 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e301]':
                - cell "2026-05-17 10:11:18" [ref=f2e302]
                - cell "Webhook" [ref=f2e303]
                - cell "ONCRMDEALUPDATE" [ref=f2e304]
                - cell "processed" [ref=f2e305]
                - cell "bx:1" [ref=f2e306]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e307]'
              - 'row "2026-05-17 10:11:18 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e308]':
                - cell "2026-05-17 10:11:18" [ref=f2e309]
                - cell "Webhook" [ref=f2e310]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e311]
                - cell "processed" [ref=f2e312]
                - cell "bx:1" [ref=f2e313]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e314]'
              - 'row "2026-05-17 10:04:42 Webhook ONCRMCONTACTDELETE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e315]':
                - cell "2026-05-17 10:04:42" [ref=f2e316]
                - cell "Webhook" [ref=f2e317]
                - cell "ONCRMCONTACTDELETE" [ref=f2e318]
                - cell "processed" [ref=f2e319]
                - cell "bx:1" [ref=f2e320]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e321]'
              - 'row "2026-05-17 10:04:41 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e322]':
                - cell "2026-05-17 10:04:41" [ref=f2e323]
                - cell "Webhook" [ref=f2e324]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e325]
                - cell "processed" [ref=f2e326]
                - cell "bx:1" [ref=f2e327]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e328]'
              - 'row "2026-05-17 10:04:11 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e329]':
                - cell "2026-05-17 10:04:11" [ref=f2e330]
                - cell "Webhook" [ref=f2e331]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e332]
                - cell "processed" [ref=f2e333]
                - cell "bx:1" [ref=f2e334]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e335]'
              - 'row "2026-05-17 10:04:10 Webhook ONCRMDEALADD processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e336]':
                - cell "2026-05-17 10:04:10" [ref=f2e337]
                - cell "Webhook" [ref=f2e338]
                - cell "ONCRMDEALADD" [ref=f2e339]
                - cell "processed" [ref=f2e340]
                - cell "bx:1" [ref=f2e341]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e342]'
              - 'row "2026-05-17 10:04:10 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e343]':
                - cell "2026-05-17 10:04:10" [ref=f2e344]
                - cell "Webhook" [ref=f2e345]
                - cell "ONCRMDEALUPDATE" [ref=f2e346]
                - cell "processed" [ref=f2e347]
                - cell "bx:1" [ref=f2e348]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e349]'
              - 'row "2026-05-17 10:04:10 Webhook ONCRMCONTACTADD processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e350]':
                - cell "2026-05-17 10:04:10" [ref=f2e351]
                - cell "Webhook" [ref=f2e352]
                - cell "ONCRMCONTACTADD" [ref=f2e353]
                - cell "processed" [ref=f2e354]
                - cell "bx:1" [ref=f2e355]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"7\"}" [ref=f2e356]'
              - 'row "2026-05-17 10:04:08 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e357]':
                - cell "2026-05-17 10:04:08" [ref=f2e358]
                - cell "Webhook" [ref=f2e359]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e360]
                - cell "processed" [ref=f2e361]
                - cell "bx:1" [ref=f2e362]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e363]'
              - 'row "2026-05-17 09:52:36 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e364]':
                - cell "2026-05-17 09:52:36" [ref=f2e365]
                - cell "Webhook" [ref=f2e366]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e367]
                - cell "processed" [ref=f2e368]
                - cell "—" [ref=f2e369]
                - 'cell "{\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e370]'
              - 'row "2026-05-17 09:49:48 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e371]':
                - cell "2026-05-17 09:49:48" [ref=f2e372]
                - cell "Webhook" [ref=f2e373]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e374]
                - cell "processed" [ref=f2e375]
                - cell "—" [ref=f2e376]
                - 'cell "{\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e377]'
              - 'row "2026-05-17 09:45:18 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e378]':
                - cell "2026-05-17 09:45:18" [ref=f2e379]
                - cell "Webhook" [ref=f2e380]
                - cell "ONCRMDEALUPDATE" [ref=f2e381]
                - cell "processed" [ref=f2e382]
                - cell "bx:1" [ref=f2e383]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e384]'
              - 'row "2026-05-17 09:45:18 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e385]':
                - cell "2026-05-17 09:45:18" [ref=f2e386]
                - cell "Webhook" [ref=f2e387]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e388]
                - cell "processed" [ref=f2e389]
                - cell "bx:1" [ref=f2e390]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e391]'
              - 'row "2026-05-17 09:41:42 Webhook ONCRMACTIVITYDELETE processed — {\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"88888\"}" [ref=f2e392]':
                - cell "2026-05-17 09:41:42" [ref=f2e393]
                - cell "Webhook" [ref=f2e394]
                - cell "ONCRMACTIVITYDELETE" [ref=f2e395]
                - cell "processed" [ref=f2e396]
                - cell "—" [ref=f2e397]
                - 'cell "{\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"88888\"}" [ref=f2e398]'
              - 'row "2026-05-17 09:41:42 Webhook ONCRMACTIVITYDELETE processed — {\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"99999\"}" [ref=f2e399]':
                - cell "2026-05-17 09:41:42" [ref=f2e400]
                - cell "Webhook" [ref=f2e401]
                - cell "ONCRMACTIVITYDELETE" [ref=f2e402]
                - cell "processed" [ref=f2e403]
                - cell "—" [ref=f2e404]
                - 'cell "{\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"99999\"}" [ref=f2e405]'
              - 'row "2026-05-16 21:14:27 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e406]':
                - cell "2026-05-16 21:14:27" [ref=f2e407]
                - cell "Webhook" [ref=f2e408]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e409]
                - cell "processed" [ref=f2e410]
                - cell "—" [ref=f2e411]
                - 'cell "{\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e412]'
              - 'row "2026-05-16 21:14:26 Webhook ONCRMACTIVITYDELETE processed — {\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"21\"}" [ref=f2e413]':
                - cell "2026-05-16 21:14:26" [ref=f2e414]
                - cell "Webhook" [ref=f2e415]
                - cell "ONCRMACTIVITYDELETE" [ref=f2e416]
                - cell "processed" [ref=f2e417]
                - cell "—" [ref=f2e418]
                - 'cell "{\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"21\"}" [ref=f2e419]'
              - 'row "2026-05-16 21:14:26 Webhook ONCRMDEALUPDATE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e420]':
                - cell "2026-05-16 21:14:26" [ref=f2e421]
                - cell "Webhook" [ref=f2e422]
                - cell "ONCRMDEALUPDATE" [ref=f2e423]
                - cell "processed" [ref=f2e424]
                - cell "—" [ref=f2e425]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e426]'
              - 'row "2026-05-16 21:14:25 Webhook ONCRMCONTACTDELETE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"99999\"}" [ref=f2e427]':
                - cell "2026-05-16 21:14:25" [ref=f2e428]
                - cell "Webhook" [ref=f2e429]
                - cell "ONCRMCONTACTDELETE" [ref=f2e430]
                - cell "processed" [ref=f2e431]
                - cell "—" [ref=f2e432]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"99999\"}" [ref=f2e433]'
              - 'row "2026-05-16 21:14:25 Webhook ONCRMCONTACTUPDATE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e434]':
                - cell "2026-05-16 21:14:25" [ref=f2e435]
                - cell "Webhook" [ref=f2e436]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e437]
                - cell "processed" [ref=f2e438]
                - cell "—" [ref=f2e439]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e440]'
              - 'row "2026-05-16 20:57:35 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e441]':
                - cell "2026-05-16 20:57:35" [ref=f2e442]
                - cell "Webhook" [ref=f2e443]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e444]
                - cell "processed" [ref=f2e445]
                - cell "—" [ref=f2e446]
                - 'cell "{\"note\":\"relayed_1_messages\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e447]'
              - 'row "2026-05-16 19:05:38 Webhook ONIMCONNECTORMESSAGEADD failed bx:1 {\"note\":\"no_recipient_phone\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e448]':
                - cell "2026-05-16 19:05:38" [ref=f2e449]
                - cell "Webhook" [ref=f2e450]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e451]
                - cell "failed" [ref=f2e452]
                - cell "bx:1" [ref=f2e453]
                - 'cell "{\"note\":\"no_recipient_phone\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e454]'
              - 'row "2026-05-16 19:03:59 Webhook ONIMCONNECTORMESSAGEADD failed bx:1 {\"note\":\"no_recipient_phone\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e455]':
                - cell "2026-05-16 19:03:59" [ref=f2e456]
                - cell "Webhook" [ref=f2e457]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e458]
                - cell "failed" [ref=f2e459]
                - cell "bx:1" [ref=f2e460]
                - 'cell "{\"note\":\"no_recipient_phone\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e461]'
              - 'row "2026-05-16 18:37:07 Webhook ONIMCONNECTORMESSAGEADD processed bx:1 {\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e462]':
                - cell "2026-05-16 18:37:07" [ref=f2e463]
                - cell "Webhook" [ref=f2e464]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e465]
                - cell "processed" [ref=f2e466]
                - cell "bx:1" [ref=f2e467]
                - 'cell "{\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e468]'
              - 'row "2026-05-16 16:58:28 Webhook ONIMCONNECTORMESSAGEADD processed — {\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e469]':
                - cell "2026-05-16 16:58:28" [ref=f2e470]
                - cell "Webhook" [ref=f2e471]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e472]
                - cell "processed" [ref=f2e473]
                - cell "—" [ref=f2e474]
                - 'cell "{\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e475]'
              - 'row "2026-05-16 16:58:28 Webhook ONCRMACTIVITYDELETE processed — {\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e476]':
                - cell "2026-05-16 16:58:28" [ref=f2e477]
                - cell "Webhook" [ref=f2e478]
                - cell "ONCRMACTIVITYDELETE" [ref=f2e479]
                - cell "processed" [ref=f2e480]
                - cell "—" [ref=f2e481]
                - 'cell "{\"note\":\"activity_aggr_recovery_on_next_message\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e482]'
              - 'row "2026-05-16 16:58:27 Webhook ONCRMDEALUPDATE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e483]':
                - cell "2026-05-16 16:58:27" [ref=f2e484]
                - cell "Webhook" [ref=f2e485]
                - cell "ONCRMDEALUPDATE" [ref=f2e486]
                - cell "processed" [ref=f2e487]
                - cell "—" [ref=f2e488]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e489]'
              - 'row "2026-05-16 16:58:27 Webhook ONCRMCONTACTDELETE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e490]':
                - cell "2026-05-16 16:58:27" [ref=f2e491]
                - cell "Webhook" [ref=f2e492]
                - cell "ONCRMCONTACTDELETE" [ref=f2e493]
                - cell "processed" [ref=f2e494]
                - cell "—" [ref=f2e495]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e496]'
              - 'row "2026-05-16 16:57:55 Webhook ONCRMCONTACTUPDATE processed — {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e497]':
                - cell "2026-05-16 16:57:55" [ref=f2e498]
                - cell "Webhook" [ref=f2e499]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e500]
                - cell "processed" [ref=f2e501]
                - cell "—" [ref=f2e502]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e503]'
              - 'row "2026-05-16 09:26:31 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e504]':
                - cell "2026-05-16 09:26:31" [ref=f2e505]
                - cell "Webhook" [ref=f2e506]
                - cell "ONCRMDEALUPDATE" [ref=f2e507]
                - cell "processed" [ref=f2e508]
                - cell "bx:1" [ref=f2e509]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e510]'
              - 'row "2026-05-16 09:26:31 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e511]':
                - cell "2026-05-16 09:26:31" [ref=f2e512]
                - cell "Webhook" [ref=f2e513]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e514]
                - cell "processed" [ref=f2e515]
                - cell "bx:1" [ref=f2e516]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e517]'
              - 'row "2026-05-16 06:45:47 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e518]':
                - cell "2026-05-16 06:45:47" [ref=f2e519]
                - cell "Webhook" [ref=f2e520]
                - cell "ONCRMDEALUPDATE" [ref=f2e521]
                - cell "processed" [ref=f2e522]
                - cell "bx:1" [ref=f2e523]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e524]'
              - 'row "2026-05-15 12:23:37 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e525]':
                - cell "2026-05-15 12:23:37" [ref=f2e526]
                - cell "Webhook" [ref=f2e527]
                - cell "ONCRMDEALUPDATE" [ref=f2e528]
                - cell "processed" [ref=f2e529]
                - cell "bx:1" [ref=f2e530]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e531]'
              - 'row "2026-05-14 21:02:07 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e532]':
                - cell "2026-05-14 21:02:07" [ref=f2e533]
                - cell "Webhook" [ref=f2e534]
                - cell "ONCRMDEALUPDATE" [ref=f2e535]
                - cell "processed" [ref=f2e536]
                - cell "bx:1" [ref=f2e537]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e538]'
              - 'row "2026-05-14 21:02:07 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e539]':
                - cell "2026-05-14 21:02:07" [ref=f2e540]
                - cell "Webhook" [ref=f2e541]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e542]
                - cell "processed" [ref=f2e543]
                - cell "bx:1" [ref=f2e544]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e545]'
              - row "2026-05-14 12:50:49 Connection install complete tl:17278 App installed for b24-cclvfg.bitrix24.com" [ref=f2e546]:
                - cell "2026-05-14 12:50:49" [ref=f2e547]
                - cell "Connection" [ref=f2e548]
                - cell "install" [ref=f2e549]
                - cell "complete" [ref=f2e550]
                - cell "tl:17278" [ref=f2e551]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e552]
              - row "2026-05-14 12:43:47 Connection install complete tl:662729 App installed for b24-cclvfg.bitrix24.com" [ref=f2e553]:
                - cell "2026-05-14 12:43:47" [ref=f2e554]
                - cell "Connection" [ref=f2e555]
                - cell "install" [ref=f2e556]
                - cell "complete" [ref=f2e557]
                - cell "tl:662729" [ref=f2e558]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e559]
              - 'row "2026-05-14 12:07:32 Webhook ONCRMDEALUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e560]':
                - cell "2026-05-14 12:07:32" [ref=f2e561]
                - cell "Webhook" [ref=f2e562]
                - cell "ONCRMDEALUPDATE" [ref=f2e563]
                - cell "processed" [ref=f2e564]
                - cell "bx:1" [ref=f2e565]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e566]'
              - 'row "2026-05-14 12:07:31 Webhook ONIMCONNECTORMESSAGEADD processed bx:1 {\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e567]':
                - cell "2026-05-14 12:07:31" [ref=f2e568]
                - cell "Webhook" [ref=f2e569]
                - cell "ONIMCONNECTORMESSAGEADD" [ref=f2e570]
                - cell "processed" [ref=f2e571]
                - cell "bx:1" [ref=f2e572]
                - 'cell "{\"note\":\"phase6a_placeholder_logged\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":null}" [ref=f2e573]'
              - 'row "2026-05-14 12:07:31 Webhook ONCRMCONTACTUPDATE processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e574]':
                - cell "2026-05-14 12:07:31" [ref=f2e575]
                - cell "Webhook" [ref=f2e576]
                - cell "ONCRMCONTACTUPDATE" [ref=f2e577]
                - cell "processed" [ref=f2e578]
                - cell "bx:1" [ref=f2e579]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e580]'
              - 'row "2026-05-14 12:07:31 Webhook ONCRMLEADADD skipped bx:1 {\"note\":\"unknown_event\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e581]':
                - cell "2026-05-14 12:07:31" [ref=f2e582]
                - cell "Webhook" [ref=f2e583]
                - cell "ONCRMLEADADD" [ref=f2e584]
                - cell "skipped" [ref=f2e585]
                - cell "bx:1" [ref=f2e586]
                - 'cell "{\"note\":\"unknown_event\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e587]'
              - 'row "2026-05-14 12:07:31 Webhook ONCRMLEADUPDATE skipped bx:1 {\"note\":\"unknown_event\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e588]':
                - cell "2026-05-14 12:07:31" [ref=f2e589]
                - cell "Webhook" [ref=f2e590]
                - cell "ONCRMLEADUPDATE" [ref=f2e591]
                - cell "skipped" [ref=f2e592]
                - cell "bx:1" [ref=f2e593]
                - 'cell "{\"note\":\"unknown_event\",\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"1\"}" [ref=f2e594]'
              - 'row "2026-05-14 12:07:31 Webhook ONCRMCONTACTADD processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e595]':
                - cell "2026-05-14 12:07:31" [ref=f2e596]
                - cell "Webhook" [ref=f2e597]
                - cell "ONCRMCONTACTADD" [ref=f2e598]
                - cell "processed" [ref=f2e599]
                - cell "bx:1" [ref=f2e600]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e601]'
              - 'row "2026-05-14 12:07:31 Webhook ONCRMDEALADD processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e602]':
                - cell "2026-05-14 12:07:31" [ref=f2e603]
                - cell "Webhook" [ref=f2e604]
                - cell "ONCRMDEALADD" [ref=f2e605]
                - cell "processed" [ref=f2e606]
                - cell "bx:1" [ref=f2e607]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"5\"}" [ref=f2e608]'
              - 'row "2026-05-14 10:50:07 Webhook ONCRMDEALADD processed bx:1 {\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e609]':
                - cell "2026-05-14 10:50:07" [ref=f2e610]
                - cell "Webhook" [ref=f2e611]
                - cell "ONCRMDEALADD" [ref=f2e612]
                - cell "processed" [ref=f2e613]
                - cell "bx:1" [ref=f2e614]
                - 'cell "{\"note\":null,\"domain\":\"b24-cclvfg.bitrix24.com\",\"entity_id\":\"3\"}" [ref=f2e615]'
              - row "2026-05-14 10:32:28 Connection install complete tl:662729 App installed for b24-cclvfg.bitrix24.com" [ref=f2e616]:
                - cell "2026-05-14 10:32:28" [ref=f2e617]
                - cell "Connection" [ref=f2e618]
                - cell "install" [ref=f2e619]
                - cell "complete" [ref=f2e620]
                - cell "tl:662729" [ref=f2e621]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e622]
              - row "2026-05-14 05:45:31 Connection install complete tl:662661 App installed for b24-cclvfg.bitrix24.com" [ref=f2e623]:
                - cell "2026-05-14 05:45:31" [ref=f2e624]
                - cell "Connection" [ref=f2e625]
                - cell "install" [ref=f2e626]
                - cell "complete" [ref=f2e627]
                - cell "tl:662661" [ref=f2e628]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e629]
              - row "2026-05-14 05:15:33 Connection install complete tl:662661 App installed for b24-cclvfg.bitrix24.com" [ref=f2e630]:
                - cell "2026-05-14 05:15:33" [ref=f2e631]
                - cell "Connection" [ref=f2e632]
                - cell "install" [ref=f2e633]
                - cell "complete" [ref=f2e634]
                - cell "tl:662661" [ref=f2e635]
                - cell "App installed for b24-cclvfg.bitrix24.com" [ref=f2e636]
          - paragraph [ref=f2e637]: Showing the most recent 86 events (capped at 200).
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
  97  |   const iframeUrlMatch = opts.iframeUrlMatch ?? 'tl-bitrix-integration.netlify.app';
  98  |   const timeoutMs = opts.timeoutMs ?? 20_000;
  99  | 
  100 |   // [E2E_SLIDER_DIAGNOSTIC] Step 1: pre-click snapshot.
  101 |   diagLog('openLeftMenuPlacement:start', {
  102 |     handlerSlug: item.handlerSlug,
  103 |     iframeUrlMatch,
  104 |     timeoutMs,
  105 |   });
  106 |   await diagOverlays(page, 'pre-dismiss');
  107 | 
  108 |   // 1. One-shot pre-dismiss. If A.1's marketplace install slider is still
  109 |   //    open from a prior step we'd be blocked from clicking the left-menu
  110 |   //    anchor. After this returns we do NOT install an auto-handler — the
  111 |   //    next slider that opens is the placement we want.
  112 |   await dismissSidePanelOverlay(page);
  113 | 
  114 |   // [E2E_SLIDER_DIAGNOSTIC] Step 2: post-dismiss state + click target.
  115 |   await diagOverlays(page, 'post-dismiss');
  116 |   if (diagEnabled()) {
  117 |     const target = page
  118 |       .locator(
  119 |         `a.menu-item-link[href*="${item.handlerSlug}"], a[href*="${item.handlerSlug}"]`,
  120 |       )
  121 |       .first();
  122 |     const targetInfo = await target
  123 |       .evaluate((el: any) => {
  124 |         const rect = el.getBoundingClientRect();
  125 |         return {
  126 |           tag: el.tagName,
  127 |           href: el.getAttribute('href'),
  128 |           text: (el.textContent ?? '').trim().slice(0, 80),
  129 |           box: { x: rect.x, y: rect.y, w: rect.width, h: rect.height },
  130 |         };
  131 |       })
  132 |       .catch((err) => ({ error: String(err) }));
  133 |     diagLog('click-target', targetInfo);
  134 |     await diagScreenshot(page, '01-pre-click');
  135 |   }
  136 | 
  137 |   // 2. Click the left-menu anchor by handler-URL slug (PR #475 locator).
  138 |   const clickStart = Date.now();
  139 |   await clickLeftMenuItem(page, item, { timeoutMs });
  140 |   diagLog('click-done', { elapsedMs: Date.now() - clickStart });
  141 | 
  142 |   // [E2E_SLIDER_DIAGNOSTIC] Step 3: post-click DOM enumeration after 500ms.
  143 |   if (diagEnabled()) {
  144 |     await page.waitForTimeout(500);
  145 |     await diagOverlays(page, 'post-click-500ms');
  146 |     const childTree = await page
  147 |       .evaluate(() => {
  148 |         const d: any = (globalThis as any).document;
  149 |         const root = d.querySelector('#a11y-slider-container');
  150 |         if (!root) return { rootExists: false, children: [] as unknown[] };
  151 |         const children = Array.from(root.children as any[]).map((c: any) => ({
  152 |           tag: c.tagName,
  153 |           dataId: c.getAttribute('data-id'),
  154 |           className: c.getAttribute('class'),
  155 |           iframeSrc:
  156 |             c.querySelector('iframe')?.getAttribute('src') ?? null,
  157 |         }));
  158 |         return { rootExists: true, children };
  159 |       })
  160 |       .catch((err) => ({ error: String(err) }));
  161 |     diagLog('post-click-children', childTree);
  162 |     await diagScreenshot(page, '02-post-click-500ms');
  163 |   }
  164 | 
  165 |   // [E2E_SLIDER_DIAGNOSTIC] Step 4: instrumented iframe attach wait (8s
  166 |   // cap) — runs BEFORE the production waits so we can log timings even
  167 |   // if the production waits then throw.
  168 |   if (diagEnabled()) {
  169 |     const attach = await waitForIframeWithDetail(page, iframeUrlMatch, 8_000);
  170 |     diagLog('iframe-attach', attach);
  171 |     // Detect close-then-reopen / detach-after-attach by re-checking after
  172 |     // a 500ms beat.
  173 |     if (attach.attached) {
  174 |       await page.waitForTimeout(500);
  175 |       const reCheck = await waitForIframeWithDetail(page, iframeUrlMatch, 500);
  176 |       diagLog('iframe-attach-recheck-500ms', reCheck);
  177 |     }
  178 |   }
  179 | 
  180 |   // 3. Wait for the placement slider container to be visible. Bitrix
  181 |   //    animates the `--open` class on after a brief delay; the iframe
  182 |   //    won't be attached until the slider is open.
  183 |   const sliderContainer = page.locator(
  184 |     '#a11y-slider-container .side-panel.--open',
  185 |   ).first();
  186 |   await sliderContainer.waitFor({ state: 'visible', timeout: timeoutMs });
  187 | 
  188 |   // 4. Wait for our iframe inside the slider to attach. Scoping the
  189 |   //    locator to the slider container guards against matching an
  190 |   //    unrelated iframe on the portal (a worker frame, a chat widget,
  191 |   //    etc.) — important because the un-scoped version sometimes
  192 |   //    resolves to the wrong frame when Bitrix mounts background frames
  193 |   //    before the placement.
  194 |   const iframeLocator = sliderContainer.locator(
  195 |     `iframe[src*="${iframeUrlMatch}"]`,
  196 |   ).first();
> 197 |   await iframeLocator.waitFor({ state: 'attached', timeout: timeoutMs });
      |                       ^ TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
  198 | 
  199 |   // [E2E_SLIDER_DIAGNOSTIC] Step 5 + 6: iframe load + body snippet.
  200 |   if (diagEnabled()) {
  201 |     const load = await waitForIframeLoad(page, iframeUrlMatch, 8_000);
  202 |     diagLog('iframe-load', load);
  203 |     const snippet = await captureIframeBodySnippet(page, iframeUrlMatch, 300);
  204 |     diagLog('iframe-body-snippet', { snippet });
  205 |     await diagScreenshot(page, '03-iframe-loaded');
  206 |   }
  207 | 
  208 |   return sliderContainer.frameLocator(`iframe[src*="${iframeUrlMatch}"]`).first();
  209 | }
  210 | 
```