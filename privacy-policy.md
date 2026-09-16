# Privacy Policy — Money Coach

_Last updated: 2026-09-16_

**TL;DR** — Your financial ledger stays on your phone. No ads and no product-analytics SDK. Production builds use *Sentry* crash and performance monitoring; financial ledger content is redacted and not uploaded. Optional Premium uses *Google Play Billing* and *RevenueCat* only to verify purchases — not to upload your money history. Resetting app data does **not** cancel Google Play subscriptions.

---

## 1. Who runs Money Coach

Money Coach is a personal-finance education app made by an independent developer. Privacy questions and deletion requests: **supfincoach@gmail.com** (also on the Google Play Store listing and in-app under About & Legal → Email support).

---

## 2. The short version

| What you might worry about | What actually happens |
|---|---|
| Does the app collect my financial ledger? | **No.** Accounts, transactions, goals, and balances stay on your phone. |
| Does it send my money data to a Money Coach server? | **No.** There is no ledger backend. |
| Do I need to create an account? | **No.** No sign-up for the core app. |
| Are there ads or product-analytics trackers? | **No.** No advertising SDK and no product-analytics SDK. Crash and performance diagnostics go to **Sentry**. |
| Do you send crash reports? | **Yes.** Production builds use **Sentry** crash and performance monitoring. Financial ledger content is redacted and not uploaded. |
| What about Premium? | Purchases go through **Google Play Billing**. **RevenueCat** verifies entitlements using billing identifiers — not your transaction history. |
| Does a local data reset cancel Premium? | **No.** Resetting app data or a local wipe does **not** cancel Google Play subscriptions. Manage subscriptions in Google Play. |

---

## 3. What stays on your device

- Accounts, transactions, goals, budget rules, gamification, preferences
- App PIN — stored as a salted hash verifier in secure device storage (not plaintext)
- Optional Premium cache flag synced with Google Play / RevenueCat when online

**Android Auto Backup** is disabled for app data so your finance ledger is not included in automatic Google device backups. You can still export a backup from Settings.

---

## 4. Permissions

**Notifications** — local reminders only (no push server).

**Camera** — optional receipt photos; stay on-device.

**Photos** — optional goal covers / receipts. On Android the app uses the **system Photo Picker** and does not request broad `READ_MEDIA_IMAGES`.

---

## 5. Sentry (crash and performance monitoring)

Production builds use **Sentry** crash and performance monitoring (`@sentry/react-native`) so we can diagnose crashes and fix stability issues.

Financial ledger content is **redacted and not uploaded**. Sensitive financial content is redacted on the device before a report is sent. This does **not** upload your accounts, transactions, goals, balances, notes, PIN codes, or backup file contents.

Sentry may receive crash logs, diagnostic information (error type, file names, line numbers), performance traces, and app or device identifiers used to group crashes. Traffic uses HTTPS. This is not advertising and not a product-analytics SDK.

---

## 6. Google Play Billing

Optional **Money Coach Premium** is sold through **Google Play Billing** (Google’s store checkout). Google Play processes payment and manages subscriptions.

Resetting app data, erasing local data, or uninstalling the app does **not** cancel Google Play subscriptions. Subscriptions must be managed through Google Play (Google Play account settings / subscriptions).

---

## 7. RevenueCat

The app uses **RevenueCat** (`react-native-purchases`) to configure the purchase SDK, fetch offerings, and verify purchase entitlements with Google Play.

For billing verification, RevenueCat / Google Play may process purchase tokens, subscription status, subscription-related events, and device or app identifiers needed to confirm that Premium is valid on this install. This is **not** a copy of your accounts, transactions, goals, or balances. Your financial ledger is not uploaded.

---

## 8. Audience

This app is **not directed to children under 13**.

Money Coach is intended for **adults 18 and over** (Play Store target audience: **18+**). We do not knowingly collect children’s personal data for the core offline ledger. Premium billing, if used, is subject to Google Play’s policies.

---

## 9. Educational disclaimer

Money Coach is an educational and personal-tracking tool — not financial, investment, tax, or legal advice.

---

## 10. Your rights / deletion

**Local app data** (ledger, PIN, photos, settings): export from Settings, or use Settings → Erase all local data (Reset all data), or uninstall.

**Resetting app data or a local wipe does NOT cancel Google Play subscriptions. Subscriptions must be managed through Google Play.** Uninstall also does not cancel a Google Play subscription.

Reset and uninstall also do not delete crash or billing records already sent to Sentry, Google Play, or RevenueCat.

To request deletion of that third-party service data, email **supfincoach@gmail.com** and ask for a privacy deletion request. The same address is listed in-app under About & Legal → Email support.

---

## 11. Contact

Privacy questions and third-party deletion requests: **supfincoach@gmail.com** (Play listing and in-app Email support).
