# PROJECT AEGIS

Private, offline-first Android field companion in development. Main target: Samsung Galaxy S25 Ultra SM-S938B, Android 17 / API 37.

## Current APK — 0.9.0 interface redesign

**[Download AEGIS 0.9.0 (93.1 MB)](https://raw.githubusercontent.com/Aimon-Auru/Project-Aegiss/refs/heads/main/apk/AEGIS-redesign-S25-0.9.0.apk)**

Open the link in Chrome outside ChatGPT if its in-app download gets stuck. The complete file is 93,078,636 bytes. Install **over your existing AEGIS without uninstalling**; keep your records and saved guides. Same package/development signer, versionCode 7. No database reset or migration is introduced. Do not downgrade.

[Everyday use and installation](REDESIGN-INSTALL.md) · [Checksums](apk/SHA256SUMS) · [Licenses](apk/REDESIGN-THIRD-PARTY-NOTICES.txt)

### A clearer everyday interface

- **Home:** picture banner and large First aid, Navigate, My kit and Ask AEGIS cards.
- **Guides:** illustrated cards, search, language filters and familiar bookmark controls. The top bookmark opens saved guides.
- **Tools:** useful functions grouped in one list, with plain descriptions.
- **Settings:** Light/Dark/phone appearance, private notes/backups, privacy, phone details and app information. Hardware readings and developer details stay out of Home.

The reader emphasizes pictures and steps. Sources/review remain available; hashes and full rights are under further details. Kit forms start with name/amount/unit; optional fields are grouped and dates use a calendar. Larger text switches action cards to a single column. Your gold-A/compass launcher icon is retained. The new home landscape is labelled in provenance as original AI-generated fictional decoration, not geographic evidence.

### Existing functions remain

Offline planning/map-reading guides, search/bookmarks, signed language packs, encrypted supplies/checklists/places/notes, foreground location/compass/walks/GPX, coarse country map and optional local guide matching remain connected to their existing implementations. Public catalog and vault stay v2; encrypted backup v2 retains legacy v1 reads. Existing settings, shortcuts, records and imported model files remain. The separate Feasibility app stays separate; no repeat of those earlier diagnostics is required to install.

**Navigate** starts GPS only on request. Its compass uses magnetic north; target bearings use true north. Return to start is a straight-line target, not a checked safe route. Walks clear when you leave; saving GPX explicitly warns about unencrypted coordinates/times. No background or remote tracking is supplied. The world map is a generalized Natural Earth country overview, approximately 85°S–85°N, without local roads/trails, elevation, live position or routes.

**First aid** opens the original ERC illustrated handbook through an explicit browser download and your chosen local PDF viewer. The PDF is separate, copyrighted and not redistributed or clinically certified by AEGIS. Save it and check it opens after disconnecting. Reviewed in-app medical procedures remain unfinished.

**Ask AEGIS** finds existing English guides without a model. Optional setup adds the exact supported 347.3 MB Qwen file for local matching. Its AI selects an existing reference; unrestricted generated survival instructions are not displayed. Questions clear on leaving. Weights, resource guards and exact-hash installation are unchanged; no weights are bundled in the APK.

### Illustrated language packs

English edition 2 is included. Guide downloads shows measured sizes and installed status. Get a pack through the external browser, return and choose Add downloaded pack. App controls remain English; Filipino/Czech guides are draft translations without independent language review.

| Pack | Guides | Download size |
| --- | ---: | ---: |
| [English](https://raw.githubusercontent.com/Aimon-Auru/Project-Aegiss/refs/heads/main/apk/AEGIS-field-basics-2.aegispack) | 8 | 15,299,971 bytes |
| [Filipino](https://raw.githubusercontent.com/Aimon-Auru/Project-Aegiss/refs/heads/main/apk/AEGIS-field-basics-fil-2.aegispack) | 8 | 15,299,980 bytes |
| [Czech](https://raw.githubusercontent.com/Aimon-Auru/Project-Aegiss/refs/heads/main/apk/AEGIS-field-basics-cs-2.aegispack) | 8 | 15,300,467 bytes |

These unchanged edition-2 packs are concise general references, not complete survival encyclopedias. Source, applicability and general/draft review status remain in each guide. A publisher signature is not clinical or botanical approval.

### Verification and limits

111 host tests pass; final build/lint have zero errors. Checks include actual Home destinations, search/saved guides, theme/shortcut retention, large-text access, optional inventory-value retention, large pictures, source disclosures, signature/pack checks, migrations/recovery, private locking, sensor cleanup and AI boundaries. APK signer continuity, permissions, nonexported components and ARM64 16 KiB ZIP/ELF alignment are audited. INTERNET remains absent; existing optional location and network-state permissions are unchanged.

Host previews/tests use API 35 and are not physical S25 tests or a user study. Device security/sensors/maps/AI qualification remains pending; use nonsensitive private test records until security acceptance. The full master project remains unfinished: reviewed medical/species content, detailed regional maps, country/radio collections, family communication, broader RAG, production hardening and iOS delivery remain open. This is a development-signed build, minimum Android 10 / API 29, target Android 17 / API 37, ARM64.

SHA-256:

```text
7ad5bb3efcac7876a9a5319e960cc89be76a8d6e072d28558a2db96a526f2e39
```

[Previous 0.8 illustrated APK](https://raw.githubusercontent.com/Aimon-Auru/Project-Aegiss/refs/heads/main/apk/AEGIS-illustrated-S25-0.8.0.apk) and older artifacts remain historical. Prefer the current version and do not downgrade a populated app.
