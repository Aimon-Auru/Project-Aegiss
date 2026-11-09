# AEGIS — first app foundation, 0.3.0

Install **AEGIS-foundation-S25-0.3.0.apk** as a separate app. It appears as **AEGIS**; the older **AEGIS Feasibility** test app and its imported model stay intact. No uninstall is needed.

This is a **development build**, not a completed emergency application. Target: Galaxy S25 Ultra / ARM64 / Android 17 (API 37), with Android 10/API 29 as the minimum OS. The new UI has host test coverage; launch and layout on the physical phone remain to be checked.

Included:

* Native Compose dashboard and Home/Library/Device/Settings navigation.
* Find a planned section, read its status and pin/unpin it. Pins remain saved locally after reopening.
* System/dark/light appearance saved on this phone.
* Device RAM/storage/API and sensor-presence snapshot with Refresh; no location reading.

Survival/medical/country content, real maps, navigation, AI assistant, private vault and group communications are **not implemented in this build**. The Library's entries describe planned features; no instruction, frequency, emergency number or safe route is fabricated. The test model remains usable only inside the older feasibility app.

The app has no INTERNET, location, camera, microphone or nearby-device permission. It saves only appearance and pinned section IDs; it has no family/medical/location input. The public Room catalog is initially empty and is not an encrypted private vault. Backup/automatic device transfer are excluded. Uninstalling or clearing this app's storage removes these display choices.

Install the downloaded APK using Android's chosen browser/file-manager installation flow. It is debug-signed; final production signing/custody and security review remain pending. Verify the downloaded file against `apk/SHA256SUMS`. Do not uninstall the feasibility app to make room unless you intend to remove its imported model and test data.
