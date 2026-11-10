# PROJECT AEGIS

Private, offline-first Android survival platform in development. Primary target: Samsung Galaxy S25 Ultra SM-S938B, Android 17 / API 37.

## Current development APK — 0.8.0 illustrated guides

[Download AEGIS 0.8.0](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-illustrated-S25-0.8.0.apk)

**Install over your existing AEGIS without uninstalling.** Same package/development signer, versionCode 6. Existing notes, inventory, plans, waypoints, bookmarks, pins, settings and imported model remain. Public catalog/vault schemas remain v2; encrypted backups retain v2 with legacy v1 reads. Do not downgrade. The separate Feasibility app and its private model remain separate.

[Picture/map/first-aid reference instructions](ILLUSTRATED-INSTALL.md) · [Field tools](FIELDTOOLS-INSTALL.md) · [Local assistant/model](ASSISTANT-INSTALL.md) · [Checksums](apk/SHA256SUMS) · [Notices](apk/ILLUSTRATED-THIRD-PARTY-NOTICES.txt)

The launcher icon now adapts the user-supplied gold-A/compass/forest brand into an Android adaptive icon. Small text and symbols were removed for legibility; regular and round launcher masks share the padded artwork. Native host rendering is checked; physical Samsung launcher appearance remains unverified.

### Pictures and tutorials

Open **Library → Ranger → Leave a useful trip plan** for a detailed three-scene illustration, a completed fictional itinerary and a three-stage walkthrough. **Enlarge illustration** opens pinch/pan/zoom and reset. Packing, conditions and offline-map preparation also have detailed new pictures. All eight general guides have walkthroughs; map-reading topics include labelled numerical examples and the original USGS north-reference picture.

The four original AI-generated illustrations are labelled fictional explanatory examples, not photographs, real routes, medical procedures or species identification. Sources, applicability and lack of specialist review remain visible. The guides work offline without a model, vault unlock or account. A real large-image database-loading failure was fixed; the old pack's bookmarks are retained during the included English edition-2 upgrade.

### Actual offline world overview

Open **Home → Open offline world overview**, or Library → Navigation. The bundled public-domain Natural Earth 5.1.2 country/territory data supports country lookup and pan/zoom in MapLibre OpenGL. It is a **generalized 1:110 million overview**, approximately 85°S–85°N. Detailed regional maps are not installed: no roads, trails, elevation, live-position overlay or routing. Boundaries can be disputed/outdated. Its native rendering on the S25 is still unverified; the earlier green-dot probe was a separate synthetic test.

All geography/style data is bundled; no tile/glyph/sprite requests, key or account are used. ACCESS_NETWORK_STATE is retained for MapLibre initialization. INTERNET and ACCESS_WIFI_STATE are removed from the merged app. The map does not request location; the separate GPS tool retains its explicit-start permission flow.

### First-aid picture reference from its publisher

Open **Home → First aid: illustrated publisher handbook**, or **Library → First aid → Open illustrated publisher reference**. The official European Resuscitation Council 2025 English handbook includes the publisher's illustrations for resuscitation/AED/children/first aid. Choose **Download from ERC in browser**, save the original PDF while connected, then **Open a saved PDF** to select it for your external PDF viewer. Check the complete book opens after disconnecting. Observed publisher file size: **17,446,129 bytes (17.4 MB)**, checked 10 November 2026; the publisher can replace that URL's file.

The handbook is a separate publication: **AEGIS does not bundle, copy, index or clinically certify it**. Copyright requires permission for redistribution, which has not been obtained. AEGIS retains neither the selected PDF nor persistent file access. Offline opening requires your local saved copy and a separate PDF viewer. This does not complete the medically reviewed in-app library or deterministic emergency procedures.

### Illustrated language packs

Library → Guide packs shows measured file/payload sizes, edition, review status and installed state. English edition 2 is included. For optional Filipino/Czech upgrades, download the edition 2 file in an external browser and import it locally. Already transferred files install offline after signature/hash validation. App controls and original source publications remain English.

| Language | Guides | Download bytes | Uncompressed payload | Status |
| --- | ---: | ---: | ---: | --- |
| [English edition 2](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-2.aegispack) | 8 | 15,299,971 | 15,704,421 | Included general references |
| [Filipino edition 2](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-fil-2.aegispack) | 8 | 15,299,980 | 15,705,671 | Optional draft translation |
| [Czech edition 2](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-field-basics-cs-2.aegispack) | 8 | 15,300,467 | 15,705,299 | Optional draft translation |

About 15.3 MB each because the actual artwork is included. Database, indexes and temporary import files add storage overhead. These are eight concise guides, not complete survival encyclopedias. Independent specialist/language review remains pending. Four art images are original generated explanatory illustrations; the unmodified original USGS image has its public-domain attribution.

### Retained tools

- Encrypted kit inventory with quantity/unit, category, location, expiry/replacement, priority and notes; search/due filter.
- Editable household checklists for eleven scenarios and general planning; user-entered private waypoints.
- Foreground native GPS with fix age/accuracy/time, magnetic compass, straight-line target distance/true bearing, bounded breadcrumbs, track-start target and explicit unencrypted GPX export. No background/remote tracking or safe-route claim; live state clears on leaving.
- Credential-gated SQLCipher notes/supplies/tasks/waypoints, automatic background/inactivity lock and encrypted full-content recovery with an independently retained key. Restore replaces all record types explicitly. Native security acceptance remains pending; use nonsensitive private test data.
- Optional on-device guide assistant and model-free full-text search. Exact verified Qwen3 0.6B INT4 weights are a separate 347,251,840-byte import, not part of the APK. CPU inference requires at least 2 GiB currently available RAM and suitable thermal/battery conditions. Closed guide identifiers select existing cited English text; unrestricted generated advice is not displayed. Questions/matches are ephemeral. Full conversational RAG is unfinished.

### Verification and remaining work

**107 automated host tests pass; build/lint have zero errors.** Actual large-PNG reader/zoom/example and old-bookmark upgrade tests run with native Skia on API 35. Other tests cover map style/data closure, explicit publisher/document-picker actions, signed pack validation, migrations/recovery, private tools, AI output/source boundaries, permission refusal and sensor cleanup. APK signer continuity, exact signed packs, nonexported components, absence of INTERNET, ARM64 and 16 KiB ZIP/ELF alignment are audited.

Host results are not S25 driver/sensor, security, clinical or language approval. This update's native world map, vault, sensors and assistant quality/resource behavior still need physical qualification. No repeat of earlier feasibility diagnostics is required to install.

**The master specification remains unfinished.** Qualified in-app first aid and plant/fruit/mushroom/animal-food references, detailed regional maps, country/radio datasets, private-group communications, broader RAG/model catalogs, production hardening and iOS delivery remain open. No species-edibility verdict or fabricated clinical guidance is supplied. Minimum Android 10 / API 29, target Android 17 / API 37, ARM64, development signing.

APK: 96,164,358 bytes (96.2 MB). SHA-256:

```text
7265719791cc28f93bcba4b3f92a53ecc668d764f3ec11340ad3da882e56ffb6
```

Earlier [0.7 assistant APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-assistant-S25-0.7.0.apk), [0.6 field tools APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-fieldtools-S25-0.6.0.apk), older guide/vault/foundation APKs and separate Feasibility artifacts remain historical. Prefer the current version; do not downgrade a populated app.
