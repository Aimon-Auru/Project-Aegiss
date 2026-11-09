# PROJECT AEGIS

Private, local-AI, offline-first Android survival platform in development.

## Download the feasibility APK

[Download AEGIS-feasibility-S25-0.1.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.1.apk)

[SHA-256 checksum](apk/SHA256SUMS) · [Third-party notices](apk/THIRD-PARTY-NOTICES.txt)

This test build is a **debug-signed diagnostic probe using synthetic data only**, not the survival application. It targets Android 17/API 37, supports Android 10/API 29 and newer, and contains ARM64 native libraries for the Galaxy S25 Ultra test target. Actual device compatibility remains to be verified.

After installing, run the synthetic encryption/migration checks and open the offline map fixture. The probe contains no AI model, emergency instructions, personal-data input, live location or remote coordination. It has no INTERNET, location, camera or microphone permission.

Build, lint, signature, permissions and 16 KB APK-alignment checks passed. The accompanying Milestone 1 host/JVM experiments passed 76 checks; those checks do not establish on-device or clinical reliability.

SHA-256 of the APK:

```text
f9299587e54e92852e2062495f34d4c046d07256ab3fabbe6900e372d8a73b86
```
