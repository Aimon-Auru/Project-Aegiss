# PROJECT AEGIS

Private, local-AI, offline-first Android survival platform in development.

## Download the feasibility APK — 0.2.0

[Download AEGIS-feasibility-S25-0.2.0.apk](https://github.com/Aimon-Auru/Project-Aegiss/raw/refs/heads/main/apk/AEGIS-feasibility-S25-0.2.0.apk)

[Local-AI benchmark instructions](LOCAL-AI-BENCHMARK.md) · [APK checksums](apk/SHA256SUMS) · [Third-party notices](apk/THIRD-PARTY-NOTICES.txt)

Install over the existing probe; the package/signing key is unchanged and version code is higher. Confirm `0.2.0-feasibility` is displayed.

This is a **debug-signed feasibility tool**, not the completed survival application. It targets Android 17/API 37, supports Android 10/API 29+, and includes ARM64 native libraries. Earlier owner tests confirmed synthetic storage checks and the 0.1.1 local map fixture. Actual phone AI performance remains to be measured.

## New: local CPU inference benchmark

1. Open **Local AI benchmark**.
2. **Download model in browser**: a public, separate **347 MB** Qwen3 0.6B INT4 no-think file. Offline transfer also works.
3. **Import downloaded model** and wait for exact size/SHA-256 verification.
4. **Run CPU smoke test**, then **Copy last benchmark report** and share it before starting another test.

[Full instructions and pinned model download](LOCAL-AI-BENCHMARK.md). Three-trial and automatic-cancellation controls are also available. The runtime is LiteRT-LM 0.19.1 with two CPU threads; it is an experimental candidate, not a final production selection. Generated output is unverified and comes only from fixed nonmedical synthetic prompts.

The APK has **no INTERNET, location, camera or microphone permission**. The optional browser download is external; inference uses the verified local file. No private prompt/profile, remote AI API, reviewed emergency guidance or family communication is included. Storage/maps remain usable without a model. AI runs in a separate nonexported worker with resource, cancellation and cleanup guards.

Build/lint, original signer continuity, API/ABI/permissions and 16 KB APK alignment passed. **26 Android host regression tests passed**, using fake inference engines for service tests. These do not establish actual phone inference speed, thermal/battery behavior, native cancellation, grounding or clinical reliability. The model download/hash was verified on the build host; no host/cloud model generation was performed.

APK SHA-256:

```text
fefb753fc1417eb504f00f694b14398e1674b1ea888a29cff8915add632a7336
```

Previous probes remain in `apk/`; the current download above is 0.2.0.
