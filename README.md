# FilmCam 1.8.0 Pro

Install FilmCam-1.8.0-Pro-OPPO.apk on Android 10+ ARM64, including OPPO Find X8 Pro. Same package/signing key as earlier cloud installers; install over the previous version to retain imported LUTs.

Choose Pro beside Photo and Video. Pro exposes sensor-supported ISO, shutter speed, white-balance presets, manual focus and EV directly over the viewfinder. ISO and shutter lock as a pair; Auto restores automatic exposure. EV is available with automatic exposure. Reset returns the Pro controls to Auto. Parameters outside the current lens capabilities are bounded or explained as unsupported. Maximum shutter is 30 seconds when the sensor supports it. Long-exposure preview stays responsive and may differ in brightness when ISO compensation reaches its limit; the saved still uses the requested full exposure.

The interface now has a champagne accent, reflective translucent glass, a compact header, a three-mode selector and an optical shutter rim. Pro JPEG/RAW use Camera2; ordinary Photo retains CameraX JPEG/HDR and video retains its recorder. Offline AI, bundled film colors, imported LUTs, zoom and output formats remain available. No Internet/network-state permission.

Validation: 130 JVM tests pass; Android Lint has zero errors. The final Pro device test passes on an Android 11 emulator: actual camera ISO 400 / shutter 0.2 seconds match saved JPEG EXIF, preview exposure is bounded, WB and EV reach sensor metadata, reset restores AE/AWB Auto, and Photo returns to CameraX. Three UI regressions and a sensor RAW/DNG test passed in the first integration run. An Android 11 empty-AF-region metadata error discovered after capture was fixed with a non-empty zero-weight region and verified by the final Pro test. The emulator exhibited System UI ANR dialogs; this is not a physical-device or performance certification. OPPO optics, firmware-specific manual controls, long-exposure limits, HDR and 4K60 still require testing on the actual phone.

Version 1.8.0 (10). Debug-signed personal testing build, distributed at the user's request.
