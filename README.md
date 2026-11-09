# PROJECT AEGIS

Private, offline-first Android survival platform in development. Primary target: Samsung Galaxy S25 Ultra, Android17/API37.

## Current development APK — 0.7.0 local assistant

[Download AEGIS 0.7.0](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-assistant-S25-0.7.0.apk)

**Install over your existing AEGIS without uninstalling.** Same package/development signer, versionCode5. Guides, language packs, bookmarks, pins and appearance remain. The vault remains v2 (migrating from v1 when needed) and retains existing notes; public catalog remains v2. Do not downgrade afterwards. The separate Feasibility app and its imported test model remain separate.

[Assistant/model installation](ASSISTANT-INSTALL.md) · [Field tool workflows](FIELDTOOLS-INSTALL.md) · [Checksums](apk/SHA256SUMS) · [Notices](apk/ASSISTANT-THIRD-PARTY-NOTICES.txt)

### New local guide assistant

Open **Home → Open local guide assistant**. Text search works immediately without a model. The optional model interprets the question and suggests an installed English general reference. Displayed summary/steps/limits/source are taken directly from that captured guide; arbitrary generated text is never rendered as survival advice. Matching may be irrelevant, so check applicability. No reviewed medical/species advice or full conversational RAG is claimed.

For **Ask local AI**, use the screen's **Download model in browser**, then **Import supported model file**. The exact supported Qwen3 0.6B INT4 weights are **347,251,840 bytes (347.3 MB)**, separate from the APK. Downloads need your external browser/network; an independently transferred file imports offline. Existing Downloads copies from the earlier benchmark can be selected, but private files inside the separate Feasibility app are not automatically shared. Allow about 415 MB free plus the original downloaded copy.

Import/removal verifies size/hash and uses staged atomic activation with process-safe model leases. Inference rechecks integrity in a separate nonexported process, using LiteRT-LM0.19.1 CPU/two threads. It needs ≥2 GiB currently available RAM, a cool phone, battery saver off and sufficient battery. Resource/timeout/cancellation guards stop work; the independent guide reader remains available. Questions/matches are not saved as conversation history and are discarded on backgrounding. Only one lightweight profile is supported; other models are rejected, and the new AI matching flow still needs physical S25 verification.

### Retained working features

- **Kit inventory:** encrypted supplies with quantity/unit, category, storage, expiry/replacement, priority and notes. Create/edit/delete, search and review-due filter. Exact quantities to three decimal places; no recommended medical doses or supply amounts.
- **Household checklists:** 11 scenario categories, custom editable tasks, completion state and optional organizing prompts. Planning records, not emergency response procedures.
- **Private waypoints:** named WGS84 coordinates, edit/delete and straight-line distance/initial true bearing. User-entered destinations are unverified.
- **Foreground GPS/GNSS:** explicit Start GPS and runtime location consent; actual fix/accuracy/age/time and available speed/ellipsoidal altitude. No Google Play services or internet requirement.
- **Magnetic compass:** native accelerometer/magnetometer readings, rotation correction and visible stale/unreliable/missing readings. Magnetic north differs from the separately labelled true target bearing; declination correction is not implemented.
- **Foreground tracks:** up to 1,000 recent points reporting ≤50m horizontal accuracy, relative sketch and first-point return target. No geographic map or safe route is implied.
- **GPX export:** explicit warning and user-selected file. GPX contains unencrypted location/time data. Live subscriptions and positions stop/clear when leaving; export before leaving if you need a file. No background or remote tracking.
- **Recovery:** encrypted v2 backup covers notes, inventory, tasks and waypoints with a separately generated recovery key. Reads legacy v1 notes-only backups. Restore replaces ALL active record types, not a merge; the app warns about older backups.
- **Offline library:** eight illustrated, source-checked general planning/map-reading guides, full-text search, bookmarks and optional signed guide-language packs. No vault unlock or model is needed to read them.

Open **Home → Open kit and household plans**, or **Home → Open GPS and compass**. Private records require Android screen-lock authentication. GPS requests precise location only when started; permission refusal does not block the library/inventory. Hardware is optional. The app has no INTERNET, camera, microphone, nearby, background-location or storage permission. Navigation is nonexported and uses a secure window.

### Downloadable guide languages

Library → Guide packs shows edition, measured file/payload size, coverage, review status and installation state. Download through the external browser, then import the signed `.aegispack` file. Installed guides work offline. App controls and original sources remain English.

| Content language | Guides | Download | Uncompressed payload | Status |
| --- | ---: | ---: | ---: | --- |
| [English](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-1.aegispack) | 8 | 33,635 bytes | 50,429 bytes | Included, general reference |
| [Filipino](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-fil-1.aegispack) | 8 | 33,709 bytes | 51,459 bytes | Optional draft translation |
| [Czech / Čeština](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-cs-1.aegispack) | 8 | 34,083 bytes | 51,037 bytes | Optional draft translation |

Database/index/temporary files add overhead to payload size. These are concise starter guides, not full encyclopedias. English lacks specialist review; translations also lack independent language review. Older guides retain their dated 0.5 examples; current live tools are separate native features.

### Validation and limits

**94 automated host tests pass; build/lint have zero errors.** Checks cover v1 database migrations with retained records, full backup and legacy compatibility/tampering, inventory/plan/waypoint CRUD, decimal/date/coordinate edge cases, public/private separation, UI entry/task/return-target actions, permission refusal/subscription cleanup, GPX content and earlier guide/vault behavior. APK signer continuity, merged permissions/nonexported components, signed pack integrity and 16KiB native/ZIP alignment were audited. Retained warnings concern dependency/tooling updates, x86/ChromeOS omission, two incompatible custom lifecycle lint checks and version-catalog placement.

Native GPS/compass accuracy, Keystore/SQLCipher upgrades and One UI behavior still require physical S25 verification. Host tests are not device, security, clinical or translation approval. Use nonsensitive private test records until those checks are complete. Minimum Android10/API29, target Android17/API37, ARM64, development signing.

**This does not complete the master specification.** Reviewed first aid, plant/mushroom/animal edibility references, geographic maps/routing, persistent/background tracks, private-group communications, country/radio datasets, broader conversational/embedding RAG, signed multi-model catalogs and production hardening remain unfinished. No unsupported emergency instructions or edibility verdicts are supplied.

APK: 59,454,640 bytes. SHA-256:

```text
4732a3a9782098448235385c0f97388d5ef44e671ae7b98250e8a0325d8ebffe
```

Earlier artifacts: [0.6 field tools APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-fieldtools-S25-0.6.0.apk), [0.5 guide APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-guides-S25-0.5.0.apk), [0.4 vault APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-vault-S25-0.4.0.apk), [0.3 foundation APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-foundation-S25-0.3.0.apk). Prefer the current version; do not downgrade a populated database. [Separate 0.2 feasibility APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.2.0.apk) and [benchmark instructions](LOCAL-AI-BENCHMARK.md) remain historical diagnostics. No repeat of those earlier tests is required to install this update.
