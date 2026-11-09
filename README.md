# PROJECT AEGIS

Private, offline-first Android field companion in development. Primary target: Samsung Galaxy S25 Ultra, Android 17/API 37.

## Current APK: 0.5.0 guides

[Download AEGIS 0.5.0](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-guides-S25-0.5.0.apk)

Install over AEGIS 0.3/0.4 **without uninstalling**. Same package and development signer; pins, appearance and the private vault remain. The separate feasibility app and its imported model stay separate.

[Installation and language packs](GUIDES-INSTALL.md) · [Checksums](apk/SHA256SUMS) · [Notices](apk/GUIDES-THIRD-PARTY-NOTICES.txt)

This release adds eight usable offline planning/map-reading guides, illustrations, source attribution, full-text search and saved bookmarks. Topics: Ten Essentials, trip planning, conditions checks, preparing another app's offline maps, map scale, contours, north references and GPS accuracy limits. Guides work without a model, vault unlock, account or connection.

**Library → Guide packs** shows actual download/payload size, language, coverage, edition, checksum and installation status. Optional downloads open your external browser; return to AEGIS to import the signed `.aegispack` file. Installed packs then work offline. App controls, diagram labels and original source documents remain English.

| Content language | Guides | Download | Uncompressed text/image payload | Status |
| --- | ---: | ---: | ---: | --- |
| [English](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-1.aegispack) | 8 | 33,635 bytes | 50,429 bytes | Included; source-checked general reference |
| [Filipino](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-fil-1.aegispack) | 8 | 33,709 bytes | 51,459 bytes | Optional developer draft translation |
| [Czech / Čeština](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-cs-1.aegispack) | 8 | 34,083 bytes | 51,037 bytes | Optional developer draft translation |

Payload is not total installed database size: indexes, metadata and temporary files add overhead. These are short starter references, mostly text with app-drawn diagrams and one small USGS public-domain image. Geographic maps and AI weights are separate future packages. No proprietary app database was copied.

English has no specialist review; optional translations also lack independent language review. **Reviewed first aid, plants/mushrooms/animal edibility references, real geographic maps, tracking, country/radio data and the in-app AI assistant are not included.** This is a partial development application, not the full survival platform or an operational emergency release.

Existing 0.4 vault features remain: Keystore-protected encrypted notes, Android device-credential confirmation, background/timeout locking, encrypted backup with a separate recovery code, and staged restore. Use nonsensitive test notes until native device authentication/SQLCipher/recovery testing and security review are complete. [Vault instructions](VAULT-INSTALL.md).

No INTERNET, location, camera, microphone, storage or nearby-device permission is added. Only the app-scoped AndroidX receiver guard remains. Only the launcher is exported. ARM64; minimum Android10/API29, target Android17/API37. New-version physical S25 Ultra acceptance remains pending; earlier feasibility results are retained and need not be repeated.

**56 automated host tests pass; build and lint have zero errors.** Tests cover actual v1→v2 migration, retained pins/bookmarks, FTS queries, signature/hash/edition/role rejection, actual JPEG decode, language imports and existing vault regressions. APK permission/component exposure, signer continuity, native/ZIP 16 KiB alignment and embedded/downloadable pack integrity were audited. Retained warnings include newer dependencies/tooling, omitted ChromeOS/x86 support, two incompatible custom lifecycle lint checks and version-catalog placement. This is not independent security, clinical, translation or physical-device certification.

APK: 32,348,740 bytes. SHA-256:

```text
2ecc15740896dca1a0a35134245984237ed278d977f825811f10a81a4dbcf245
```

## Earlier builds

[0.4 vault APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-vault-S25-0.4.0.apk) · [0.3 foundation APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-foundation-S25-0.3.0.apk). Prefer the current version; do not downgrade a populated database.

[Separate 0.2 feasibility APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.2.0.apk) · [Benchmark instructions](LOCAL-AI-BENCHMARK.md). This diagnostic app contains synthetic storage/map/local-model trials, not the real field library.
