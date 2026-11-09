# PROJECT AEGIS

Private, local-AI, offline-first Android survival platform in development.

## Download the feasibility APK — 0.1.1

[Download AEGIS-feasibility-S25-0.1.1.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.1.1.apk)

[SHA-256 checksum](apk/SHA256SUMS) · [Third-party notices](apk/THIRD-PARTY-NOTICES.txt)

This test build is a **debug-signed diagnostic probe using synthetic data only**, not the survival application. It targets Android 17/API 37, supports Android 10/API 29 and newer, and contains ARM64 native libraries for the Galaxy S25 Ultra test target. The owner-run 0.1 storage checks passed; repaired offline rendering in 0.1.1 still needs device confirmation.

After installing, run the synthetic encryption/migration checks and open the offline map fixture. The probe contains no AI model, emergency instructions, personal-data input, live location or remote coordination. It has no INTERNET, location, camera or microphone permission.

Build, lint, signer continuity, permissions, map-process declaration and 16 KB APK-alignment checks passed. The map correction passes nine Android host failure-path tests, alongside the earlier 76 M1 host/JVM checks. These do not establish native GPU, on-device or clinical reliability.

## Map startup update

Install 0.1.1 over the existing probe; it uses the same package/signing certificate and a higher version code. Confirm the screen shows `0.1.1-feasibility`, then try the map with airplane mode enabled and Wi-Fi off.

The map SDK now retains read-only network-status permission and is explicitly forced offline. INTERNET remains absent. Map startup/lifecycle errors and a 20-second foreground timeout are displayed with Stage/Error details. The map runs in its own process, and the storage screen reads retained diagnostics on return. A loaded style alone is not claimed as a rendered map.

If it still fails, share the Stage/Error text, or the map status/Android exit reason shown on the main screen. No personal information is entered or transmitted automatically.

SHA-256 of the APK:

```text
b90cd1206f4af451039536b5e85f3c7d3cdba5976787ac98c4490fda2b15f7d8
```
