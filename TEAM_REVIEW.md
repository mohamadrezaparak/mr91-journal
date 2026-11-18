# MR91 Journal — Team Review 1.2.0-alpha

## 1. Senior Android engineer
Created a Java Native Android foundation with SQLite local persistence and a GitHub Actions build workflow.

## 2. Debugger
Reviewed null-safe display helpers, required-field checks, parameterized database update/delete calls, and cursor closure. Runtime compilation and device tests remain outstanding.

## 3. UI/UX designer
Introduced a dark navy/blue MR91 visual foundation, dashboard, journal list, and persistent bottom navigation. Full RTL review and accessibility pass remain outstanding.

## 4. Trader
Included symbol, direction, entry/exit, Entry 1/2, TP 1/2, SL 1/2, position size/currency, leverage, win/loss, P/L, reason, lesson, and chart attachment.

## 5. Adversarial reviewer — findings
- Alpha does not yet calculate realized P/L or risk automatically; user-entered P/L is stored as text.
- Editing a trade is not implemented.
- Image URI is stored, but backup/restore of image files is not implemented.
- SQLite schema migration strategy is not yet implemented.
- Locale switch refreshes the dashboard; deeper screen state restoration needs testing.
- Android 13+ photo picker/document URI permission behavior requires device testing.
- Text inputs currently accept free-form numbers; decimal and range validation must be added.
- No automated unit/UI tests are included yet.

## 6. Fix team
The current build includes basic validation for required symbol, entry and size, database cursor cleanup, parameterized SQL, and null-safe UI display. Remaining findings are explicitly tracked for the next alpha.

## 7. QA
Static source/manifest/workflow review only. No claim of successful APK compilation, emulator launch, or physical-device testing.

## 8. Publisher
Project layout and GitHub Actions workflow included. Release ZIP is an alpha source package, not a signed production APK.
