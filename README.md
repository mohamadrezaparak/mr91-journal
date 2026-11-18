# MR91 Journal — 1.3.0-alpha
Native Android / Java / SQLite / offline-first.

## Included
- MR91 launcher icon assets (legacy and adaptive launcher icon).
- Persian/English UI foundation and RTL/LTR layout direction.
- Dashboard: total trades, win rate based on closed trades, open trades, wins, losses and net recorded P/L.
- Trade capture: symbol, direction, main entry/exit, Entry 1/2, TP 1/2, SL 1/2, size, currency and leverage.
- WIN/LOSS workflow with sign validation: wins must be positive; losses must be negative.
- Numeric keyboard and basic positive-number validation for entry, size, exit and leverage.
- Local SQLite persistence, trade list and delete confirmation.
- Animated page/card entrances and touch feedback.
- GitHub Actions workflow to build and upload a debug APK artifact.

## Build
JDK 17, Android SDK 35, Gradle 8.9, Android Gradle Plugin 8.7.3.
Open in Android Studio or run `gradle assembleDebug`.

## QA honesty
Source-level review and ZIP integrity checks only. This environment has not run an Android emulator/device build. The app remains alpha.
Known gaps: editing trades, true weighted/partial-entry P/L calculation, export/import and backup, chart image preview, automated tests, full accessibility review and full RTL polish.
