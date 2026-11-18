# MR91 Journal 1.2.1 — visual pass and independent review

## Applied
- Added MR91 launcher artwork derived from the supplied logo, including legacy density icons and Android adaptive icon resources.
- Added dark navy launcher background with high-contrast white/cyan logo foreground.
- Added rounded elevated surfaces, gradient app shell, subtle entrance animations, and tactile press feedback.
- Applied Persian RTL / English LTR layout direction to the main screen and scroll content.
- Added app icon and round icon references to AndroidManifest.

## Independent review findings still open
- No Android SDK/Gradle executable was available in the build container, so APK compilation and runtime installation could not be performed.
- No automated instrumentation or unit tests are present yet.
- Trade outcome amount is stored as user-entered text; it is not yet a verified P/L calculation.
- Trade editing, robust numeric validation, image backup/restore, export/import, and database migrations remain unimplemented.
- Full RTL review of dialogs, spinners, and system document picker needs a real-device pass.

## Honest test status
Resource paths, manifest references, XML well-formedness, Java source structure, and ZIP integrity can be statically checked. This review does not claim an APK build, emulator run, or physical-device test.
