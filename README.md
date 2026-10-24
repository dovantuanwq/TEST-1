# FilmCam 1.7.0 — Offline AI integrated

Install FilmCam-1.7.0-OPPO.apk on Android 10+ ARM64, including OPPO Find X8 Pro.
Same application ID and signing key as the previous cloud installers; install over the old version to preserve imported LUTs.

AI is enabled by default. The AI button is at the top left of the camera screen. Subject/thirds markers, a horizon level and guidance appear over the viewfinder. Alignment becomes green after holding the subject within 5% of view width and device roll within 2 degrees continuously for 800 ms. Shutter remains manual. Toggle AI off/on with the AI button.

Bundled ML Kit object and face models work offline. The APK has no Internet or network-state permissions. JPEG uses CameraX analysis when supported; maximum-resolution/HDR configurations fall back to preview sampling. RAW and LUT video preserve Camera2/MediaCodec and use screen preview sampling. Guidance is never included in saved photos or video.

Validation: 115 JVM tests and Android Lint pass. Six Android core tests pass, including bundled offline models, a real detected face, CameraX frame processing, StateFlow geometry, continuous lock and sensor lifecycle. In the real application, default-on visible controls and successive successful CameraX inferences were observed; disabling AI stopped processing and enabling it resumed processing. The final JPEG/video integration test did not complete: the CPU emulator showed System UI ANR, host graphics-context errors and an ADB timeout. No successful final end-to-end photo/video test is claimed for 1.7.0. Physical OPPO behavior and live sensor accuracy remain unverified. This is a personal testing installer, not a production-certified release.

Version: 1.7.0 (9). This is a debug-signed personal testing build, distributed at the user's request.
