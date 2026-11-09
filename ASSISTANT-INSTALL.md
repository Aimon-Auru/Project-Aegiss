# AEGIS 0.7.0 — on-device guide assistant

Install **AEGIS-assistant-S25-0.7.0.apk over your existing AEGIS without uninstalling**. Same package/signer; existing kit, plans, waypoints, notes, backups, guides, pins and settings remain. Keep the separate Feasibility app if retaining its imported model. No old benchmark rerun is required.

Open **Home → Open local guide assistant** (also Library → Local intelligence). You can use **Text search** immediately, with no model. Try `contour` or `map scale` to find the bundled English references.

For optional local AI:

1. On the assistant screen, scroll to **Optional on-device model**. The supported Qwen3 0.6B INT4 file is **347,251,840 bytes (347.3 MB)**, separate from the APK.
2. Choose **Download model in browser** while connected, or copy that exact model file to the phone independently. AEGIS has no internet permission. If you still have the original 0.2 model file in Downloads, you can select that file; the other app's private imported copy is not shared automatically.
3. Return to AEGIS → **Import supported model file**. Select the file and keep the screen open for integrity verification. Allow about 415 MB free plus space used by the original downloaded copy. Bad size/hash or cancellation retains an existing valid installation. A subsequent import cleans interrupted partials.
4. Enter a question about the installed guides, then **Ask local AI**. Inference is local; no network or account is required after installation. The manager can remove the installed model without deleting guides or private records.

This assistant suggests a guide and displays that installed guide's existing summary, key points, limits and source. It does not display unrestricted generated survival instructions. A suggested match may be irrelevant: check its applicability. Only English general references are supported here; translated packs stay in Library. Medical/species/edibility/water-treatment/radio/evacuation requests show the lack of reviewed content. No reviewed medical or edible-species corpus has been added.

The lightweight CPU model needs at least 2 GiB CURRENTLY AVAILABLE RAM. Warm phones, battery saver and low battery can block inference; low memory/thermal pressure or a timeout stops it. Cancel or leave the screen to stop work. Questions and matches are not saved as history, and are cleared on leaving/backgrounding. The window is protected against normal screenshots/recents capture. Reading/searching the library and field tools remain independent of AI.

The app includes the native adapter and this new matching flow has host coverage, but still needs actual S25 model-quality/resource verification. Earlier CPU probe results do not qualify every new query. Only this specific lightweight profile is supported; other model files are rejected. No fabricated advanced-model compatibility, full conversational RAG, diagnosis, species identification, route safety or emergency service capability is claimed.

All 0.6 tools remain: encrypted kit/checklists/waypoints, foreground GPS/compass/breadcrumbs/GPX and full-content encrypted backups. GPS has its existing optional location permissions; the AI adds no new permissions. Foreground tracks clear when leaving navigation; exported GPX is deliberately unencrypted after confirmation. Native vault/navigation/security acceptance remains pending. This remains a development-signed partial survival application, not the completed master specification.
