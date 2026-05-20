# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: ..\auth.setup.ts >> authenticate against Bitrix portal
- Location: tests\e2e-playwright\auth.setup.ts:63:1

# Error details

```
TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
Call log:
  - waiting for locator('input[type="password"]').first() to be visible

```

# Page snapshot

```yaml
- generic [ref=e2]:
  - button "Log in" [ref=e5] [cursor=pointer]:
    - generic [ref=e6]: Log in
  - generic [ref=e8]:
    - link [ref=e10] [cursor=pointer]:
      - /url: https://www.bitrix24.com
    - generic [ref=e11]: Your ultimate workspace
  - generic [ref=e17]:
    - generic [ref=e18]:
      - heading "Recover password" [level=2] [ref=e19]
      - generic [ref=e20]:
        - paragraph [ref=e21]: Password recovery link will be sent to your email.
        - textbox [ref=e24]: patrai.anton@gmail.com
        - iframe [ref=e30]:
          - generic [ref=f1e2]:
            - generic [ref=f1e3]:
              - checkbox "I'm not a robot" [ref=f1e7]
              - generic [ref=f1e11]: I'm not a robot
              - generic [ref=f1e13]:
                - text: This site is exceeding
                - link "reCAPTCHA Enterprise free quota" [ref=f1e14] [cursor=pointer]:
                  - /url: https://cloud.google.com/recaptcha/docs/billing-information
                - text: .
            - generic [ref=f1e18]: reCAPTCHA
        - button "Continue" [ref=e31]:
          - generic [ref=e32]: Continue
    - generic [ref=e34]:
      - generic [ref=e35]: reCAPTCHA protection
      - generic [ref=e36]: ●
      - link "Terms of Service" [ref=e37] [cursor=pointer]:
        - /url: https://policies.google.com/privacy
      - generic [ref=e38]: ●
      - link "Privacy Policy" [ref=e39] [cursor=pointer]:
        - /url: https://policies.google.com/terms
  - generic [ref=e40]:
    - generic [ref=e41]:
      - generic [ref=e43] [cursor=pointer]: English
      - link "Privacy Policy" [ref=e45] [cursor=pointer]:
        - /url: https://www.bitrix24.com/privacy/
    - button "Help" [ref=e47] [cursor=pointer]:
      - generic [ref=e49]: Help
```

# Test source

```ts
  5   |  * write here.
  6   |  *
  7   |  * What this spec does:
  8   |  *
  9   |  *   1. Reads BITRIX_PORTAL_URL / BITRIX_EMAIL / BITRIX_PASSWORD from env
  10  |  *      (typically populated by `tests/e2e-playwright/.env.test.local`, which
  11  |  *      is gitignored). Bails loudly if any are missing.
  12  |  *
  13  |  *   2. Logs into the Bitrix portal. Bitrix24's cloud login is a multi-step
  14  |  *      flow: enter email → continue → enter password → continue. Some test
  15  |  *      accounts are linked to a Google / social account, in which case Bitrix
  16  |  *      inserts an extra screen with a social-account picker AND a password
  17  |  *      fallback button — we click that to reveal the password input. After
  18  |  *      login we wait for the portal landing page (presence of the left-side
  19  |  *      navigation `#sidebar` or `.bx-menu`) before considering the session
  20  |  *      established.
  21  |  *
  22  |  *   3. Detects SSO / 2FA prompts and bails with a clear error so Anton knows
  23  |  *      to either disable 2FA on the test account or supply a TOTP secret.
  24  |  *      We DON'T try to be clever here — a 2FA-protected account is not
  25  |  *      compatible with a fully autonomous run, and any "wait and hope"
  26  |  *      behaviour would just waste budget.
  27  |  *
  28  |  *   4. Saves storage state to `.auth/bitrix.json`.
  29  |  *
  30  |  * Only Bitrix portal auth is persisted here. The TimelinesAI login path was
  31  |  * removed because every in-scope spec accesses TL exclusively via the Public
  32  |  * API (`TL_API_TOKEN` Bearer) and the admin-sql endpoint (`lib/adminSql.ts`)
  33  |  * — none of them depend on TL UI cookies, and the old TL login test was
  34  |  * brittle against TL UI redesigns.
  35  |  *
  36  |  * NOTE: this file is in the same dir as playwright.config.ts (not under
  37  |  * `specs/`) so Playwright only picks it up via the `setup` project's
  38  |  * `testMatch`, never as a regular spec.
  39  |  */
  40  | 
  41  | import { test as setup, expect } from '@playwright/test';
  42  | import * as path from 'node:path';
  43  | import * as url from 'node:url';
  44  | import { mkdirSync } from 'node:fs';
  45  | 
  46  | const __dirname = path.dirname(url.fileURLToPath(import.meta.url));
  47  | const AUTH_DIR = path.join(__dirname, '.auth');
  48  | mkdirSync(AUTH_DIR, { recursive: true });
  49  | 
  50  | const BITRIX_AUTH_FILE = path.join(AUTH_DIR, 'bitrix.json');
  51  | 
  52  | function requireEnv(name: string): string {
  53  |   const v = process.env[name];
  54  |   if (!v) {
  55  |     throw new Error(
  56  |       `[auth.setup] Missing required env var ${name}. ` +
  57  |         `Populate tests/e2e-playwright/.env.test.local (see README).`,
  58  |     );
  59  |   }
  60  |   return v;
  61  | }
  62  | 
  63  | setup('authenticate against Bitrix portal', async ({ page }) => {
  64  |   const portal = requireEnv('BITRIX_PORTAL_URL'); // e.g. https://b24-g0r3o2.bitrix24.com
  65  |   const email = requireEnv('BITRIX_EMAIL');
  66  |   const password = requireEnv('BITRIX_PASSWORD');
  67  | 
  68  |   await page.goto(portal, { waitUntil: 'domcontentloaded' });
  69  | 
  70  |   // Bitrix24 cloud login is now a two-step passwordless-style form: the first
  71  |   // screen has an anonymous textbox with placeholder "name@company.com" and a
  72  |   // "Continue" button; the password screen appears only after Continue. Older
  73  |   // single-step portals exposed the legacy `USER_LOGIN` / `USER_PASSWORD`
  74  |   // inputs on the same form — keep those as fallback selectors for
  75  |   // backwards compatibility.
  76  |   const emailInput = page
  77  |     .getByPlaceholder('name@company.com')
  78  |     .or(page.locator('input[type="email"], input[name="USER_LOGIN"], input[name="login"]'))
  79  |     .first();
  80  |   await emailInput.waitFor({ state: 'visible', timeout: 20_000 });
  81  |   await emailInput.fill(email);
  82  | 
  83  |   // Two-step: click Continue to advance to password screen. Legacy single-step
  84  |   // portals don't have this button, so guard with a short-timeout try.
  85  |   const continueBtn = page.getByRole('button', { name: /^Continue$/i });
  86  |   try {
  87  |     await continueBtn.waitFor({ state: 'visible', timeout: 5_000 });
  88  |     await continueBtn.click();
  89  |   } catch {
  90  |     // Single-step portal — password input is already on this page.
  91  |   }
  92  | 
  93  |   // Some accounts are linked to a Google / social account. Bitrix shows an
  94  |   // extra screen with a social-account picker AND a password-fallback button
  95  |   // (labelled per the selector below). Click that to reveal the password input.
  96  |   const passwordPathBtn = page.getByRole('button', { name: /or log in using password/i });
  97  |   try {
  98  |     await passwordPathBtn.waitFor({ state: 'visible', timeout: 5_000 });
  99  |     await passwordPathBtn.click();
  100 |   } catch {
  101 |     // No social-account branch — password field is already exposed.
  102 |   }
  103 | 
  104 |   const pwdInput = page.locator('input[type="password"]').first();
> 105 |   await pwdInput.waitFor({ state: 'visible', timeout: 20_000 });
      |                  ^ TimeoutError: locator.waitFor: Timeout 20000ms exceeded.
  106 |   await pwdInput.fill(password);
  107 | 
  108 |   await page
  109 |     .getByRole('button', { name: /^(Log in|Sign in|Continue)$/i })
  110 |     .first()
  111 |     .click();
  112 | 
  113 |   // Now we're either on the portal, on a 2FA challenge, or staring at an error.
  114 |   // Race the three.
  115 |   const result = await Promise.race([
  116 |     page.waitForSelector('#sidebar, .bx-menu, [data-id="main-buttons-menu"]', { timeout: 30_000 })
  117 |       .then(() => 'ok' as const),
  118 |     page.waitForSelector('text=/two-factor|verification code|authenticator/i', { timeout: 30_000 })
  119 |       .then(() => '2fa' as const),
  120 |     page.waitForSelector('.login-form-error, .error-text, text=/incorrect|invalid/i', { timeout: 30_000 })
  121 |       .then(() => 'error' as const),
  122 |   ]).catch(() => 'timeout' as const);
  123 | 
  124 |   if (result === '2fa') {
  125 |     throw new Error(
  126 |       '[auth.setup] Bitrix presented a 2FA challenge for the test account. ' +
  127 |         'Either disable 2FA on this account, or use an account without 2FA. ' +
  128 |         'TOTP automation is NOT implemented.',
  129 |     );
  130 |   }
  131 |   if (result === 'error') {
  132 |     throw new Error('[auth.setup] Bitrix login form showed an error. Check credentials.');
  133 |   }
  134 |   if (result === 'timeout') {
  135 |     throw new Error(
  136 |       '[auth.setup] Timed out waiting for portal landing page. ' +
  137 |         'Either Bitrix is slow today or the login flow has changed. ' +
  138 |         'Re-run in headed mode (`npm run e2e:headed`) to inspect.',
  139 |     );
  140 |   }
  141 | 
  142 |   await expect(page).toHaveURL(new RegExp(`^${portal.replace(/[.*+?^${}()|[\\]\\\\]/g, '\\\\$&')}`));
  143 | 
  144 |   await page.context().storageState({ path: BITRIX_AUTH_FILE });
  145 | });
  146 | 
```