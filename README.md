# FilmCam 1.6.0 — AI Core / OPPO ARM64

Android installer for OPPO Find X8 Pro and other ARM64 Android 10+ phones.

Download `FilmCam-1.6.0-AI-Core-OPPO.apk` and install over the previous FilmCam version to keep custom LUTs. This installer uses the same signing certificate.

This build packages the offline smart composition core. The existing UI is unchanged; composition guidance is not bound to the UI yet.

APK size: 29,629,391 bytes.
SHA-256: `6b89fb9f44a326e6c739c3b5224ea9365f39ffd794ff58f06f20fd7697e96a49`.

Validation: 109 JVM tests and 5 headless Android tests passed. The ARM64 installer has identical DEX, model assets and ARM64 native libraries to that validated build; only packaging/ABI selection differs. Physical OPPO testing remains outstanding.
