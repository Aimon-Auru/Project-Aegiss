# PROJECT AEGIS

Private, local-AI, offline-first Android survival platform in development.

## Current development APK — 0.4.0 vault

[Download AEGIS-vault-S25-0.4.0.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-vault-S25-0.4.0.apk)

[Install / vault / backup instructions](VAULT-INSTALL.md) · [Checksums](apk/SHA256SUMS) · [Vault notices](apk/VAULT-THIRD-PARTY-NOTICES.txt)

**Install over AEGIS 0.3.0 without uninstalling.** Same application/signing certificate, higher version code; pins and appearance remain. The separate AEGIS Feasibility application and imported model are untouched.

Open **Settings → Open private vault**. New development functionality:

* SQLCipher/Room encrypted notes with Android Keystore-protected keys.
* Android PIN/pattern/password confirmation to create/open the vault.
* Locking when the private activity pauses/backgrounds and after two minutes of inactivity.
* Private window screenshot/recents protection; draft/recovery input cleared on locking.
* Portable AES-256-GCM backup with a separately generated recovery code; staged restore followed by device authentication and atomic activation.

**Use nonsensitive test notes until actual-device vault acceptance and security review are complete.** This debug-signed build is not production-qualified. Host tests do not execute Android Keystore hardware or ARM64 SQLCipher end to end. Previous encrypted generations are retained; cleanup and rollback browsing are not implemented. Backups contain notes only; keep the generated recovery code separately because AEGIS does not retain it.

**33 automated host tests pass**, covering domain limits, backup encryption/tampering/malformed inputs, atomic pointer interruption, public/private schema separation, background/timeout draft clearing, secure-window flag and existing Compose behavior. All affected modules build and lint with zero errors. Retained warnings include newer dependencies/tooling, omitted ChromeOS/x86 support, two incompatible custom lifecycle lint checks and version-catalog placement. APK signature/lineage, permissions, component exposure, ARM64 native/ZIP 16 KB alignment and absent model weights were audited.

No INTERNET, location, camera, microphone or nearby-device permission is added. AndroidX retains only its app-scoped signature guard permission. This version targets Android 17/API 37, minimum Android 10/API 29, ARM64 for the S25 Ultra development target. Biometric-only unlock, family/medical forms, live location sharing and group communication are not implemented.

The native dashboard, Library, Device and Settings remain. **Operational survival/first-aid/species content, real maps and the AI assistant are still pending.** The Library correctly has no installed guide packages. The feasibility model is not integrated into this app yet.

APK: 30,804,745 bytes. SHA-256:

```text
6fc83a1ce98242d67817ef35263eee90b5921faeaa1c049e8ac97f69d315c5af
```

## Previous foundation — 0.3.0

[Download foundation APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-foundation-S25-0.3.0.apk) · [Foundation instructions](FOUNDATION-INSTALL.md)

The initial AEGIS application introduced Home/Library/Device/Settings, saved section pins and appearance, a public Room catalog and permissionless hardware-presence snapshots. Install the current 0.4.0 update over it; do not downgrade a populated vault.

## Separate feasibility application — 0.2.0

[Download feasibility APK](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.2.0.apk) · [Benchmark instructions](LOCAL-AI-BENCHMARK.md) · [Probe notices](apk/THIRD-PARTY-NOTICES.txt)

The diagnostic app retains synthetic storage checks, the local green-dot map fixture and fixed-prompt LiteRT-LM CPU benchmarks with a separately imported model. Its data/model stay separate from AEGIS. No old benchmark rerun is required merely to install the current app update.
