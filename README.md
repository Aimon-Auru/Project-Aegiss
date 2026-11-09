# PROJECT AEGIS

Private, local-AI, offline-first Android survival platform in development.

## Download the app foundation — 0.3.0

[Download AEGIS-foundation-S25-0.3.0.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-foundation-S25-0.3.0.apk)

[Installation and scope](FOUNDATION-INSTALL.md) · [APK checksums](apk/SHA256SUMS) · [Foundation notices](apk/FOUNDATION-THIRD-PARTY-NOTICES.txt)

Install as a **separate app named AEGIS**. Keep **AEGIS Feasibility** installed to retain its imported test model and diagnostics. The two apps have different application IDs; this does not replace or migrate the test app.

Included in this first development increment:

* Native Kotlin / Compose dashboard, Library, Device and Settings screens.
* Search planned section names, open their status, and save pinned sections locally.
* Saved system/dark/light appearance.
* Refreshable device RAM/storage/API and sensor-presence information without reading location.
* Versioned public Room catalog, initially empty; separate portable contracts/domain modules.

**Emergency content, real maps, GPS navigation, the AI assistant, private vault and group communication are not included yet.** Library entries describe planned features. The existing test model is not automatically available in this separate app. No personal medical/family/location entry is enabled.

This is a **debug-signed development build**, not a completed emergency application. It compiles/targets Android 17/API 37, with Android 10/API 29 minimum and ARM64 native libraries for the S25 Ultra. Launch/layout acceptance on the actual phone remains pending for this new package.

The final cached build succeeded. **11 automated host tests passed**: six domain readiness checks, three Room/storage checks and two Compose UI tests including activity recreation. APK audit verifies permissions, only the launcher exported, disabled backup/cleartext, valid signature, ARM64 native ELF and ZIP alignment for 16 KB pages, bundled notices and absent model weights. Lint has no errors; warnings include newer dependency versions, omitted ChromeOS/x86 support and two incompatible library lifecycle lint checks that are skipped. Host checks do not certify physical-device behavior or production security.

The app has no INTERNET, location, camera, microphone or nearby-device permission. AndroidX adds only its app-scoped signature guard permission for nonexported receivers. No account, telemetry or server is required. Pins and appearance are nonsensitive local data; this public catalog is not an encrypted vault.

APK SHA-256:

```text
1652e21e7b652982d0b07821c34ec196f2891e836d6a36f0cb989f85646e2bfe
```

## Separate feasibility tool — 0.2.0

[Download AEGIS-feasibility-S25-0.2.0.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.2.0.apk) · [Benchmark instructions](LOCAL-AI-BENCHMARK.md) · [Probe notices](apk/THIRD-PARTY-NOTICES.txt)

The older diagnostic application retains synthetic storage checks, the green-dot offline map fixture and optional fixed-prompt LiteRT-LM CPU benchmarks with a separately imported 347 MB model. It remains a test tool. Earlier APKs stay in `apk/`; no new benchmark rerun is required just to install the foundation.
