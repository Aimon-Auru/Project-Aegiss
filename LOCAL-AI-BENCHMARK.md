# AEGIS local-AI test — 0.2.0

This is an experimental device benchmark, not the completed survival application. Inference runs on the phone. The APK has no INTERNET permission; its download button opens your browser for the public model file.

## Run the first test

1. Install **AEGIS-feasibility-S25-0.2.0.apk** over the existing app. It uses the same package/signing key and a higher version code. Confirm the screen says `0.2.0-feasibility`.
2. Tap **Open local AI benchmark (import model)**.
3. Tap **Download model in browser**. The file is **347 MB**, Apache-2.0, and publicly available without an account. An offline transfer of the exact same file also works.
4. Return to the app, tap **Import downloaded model**, and choose `qwen3_0.6b_nothink_q4_block32_ekv1280.litertlm`. Wait for the size/SHA-256 verification message. A different file, even renamed, is rejected.
5. Tap **Run CPU smoke test**. Network access is unnecessary after download/import. The first engine load may take time; the screen reports its stage.
6. Tap **Copy last benchmark report** and share that report. Copy it before starting another test, because the next run replaces the last report.

Then run **three CPU trials** and **automatic cancellation test**, copying each report separately. **Stop current import / AI trial** cancels current work. Leaving the AI screen also requests cancellation. If native cancellation stalls, only the inference worker is force-stopped after its deadline.

## Exact model

File: `qwen3_0.6b_nothink_q4_block32_ekv1280.litertlm`  
Size: `347251840` bytes  
SHA-256: `2df6821ec12702dafd33915e7a1a1adc7c4b053f3672fd9555dfaf3a114c4139`

[Pinned public model download](https://huggingface.co/litert-community/Qwen3-0.6B-int4/resolve/56621f0115eba5781051ef9714c06e16e6d40c0b/qwen3_0.6b_nothink_q4_block32_ekv1280.litertlm?download=true) · [Publisher model card](https://huggingface.co/litert-community/Qwen3-0.6B-int4)

Runtime candidate: LiteRT-LM 0.19.1, CPU with two threads. This is not a final production runtime/model choice. GPU/NPU are not being tested yet.

## Results and boundaries

The report includes initialization, first text chunk and full generation times; available runtime token metrics; sampled memory; Android thermal status; battery temperature observations; cancellation/cleanup; and failure stage/detail. Engine loading follows an integrity read, so file cache may be warm. A text chunk is not necessarily one token. Short trials are not battery-life or sustained thermal tests.

Only fixed synthetic color/list prompts run. Generated text is unverified, and no medical/survival questions, private profiles, chat history or remote AI API are used. Results stay local until you explicitly copy/share them. Storage and map tests remain accessible without importing a model.

If admission is refused, the report explains the current RAM/battery/thermal condition; nominal total RAM is not the same as currently available memory. If the worker fails, share its retained failure stage and detail. No speed, heat or model compatibility result is assumed from a build/test pass.
