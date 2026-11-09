# AEGIS 0.4.0 — private vault development update

Install **AEGIS-vault-S25-0.4.0.apk over AEGIS 0.3.0**, without uninstalling. Same `local.aegis.app` package/signing certificate, higher version code. Existing pins/appearance remain. Keep the separate AEGIS Feasibility app if retaining its test model.

Open **Settings → Open private vault**. Confirm your Android PIN, pattern or password to create/open the encrypted note store. A secure Android screen lock is required. This version uses device credentials, not a biometric-only prompt. The vault is a development implementation: use nonsensitive test notes until native device testing/security review are complete.

New functionality:

* Add/read/delete encrypted notes (up to 100); private data is separate from the public library database.
* Lock immediately when the vault activity pauses/backgrounds, on Lock now, or after two minutes of inactivity.
* Private screen capture/recents protection; note drafts/recovery input are not saved across relock/recreation.
* Export an encrypted backup with a separately generated recovery code; restore it behind device authentication.

For backup, choose **Back up notes**, record the generated 43-character code somewhere separate, acknowledge it, then choose the encrypted file destination. AEGIS does not retain the code. Copy is optional/explicit and uses the Android clipboard. Going to the file picker locks the vault. Keep the code after export; a file without its code is not recoverable on another phone.

For restore, choose **Restore encrypted backup** from the locked screen, select the file, enter its code and confirm replacement. A separate encrypted generation is prepared first; then Android screen-lock confirmation is required before it becomes active. It replaces the active note list, not a merge. Wrong code, invalid file or cancellation before commit leaves the old selection intact. Previous encrypted generations remain stored; automatic cleanup/rollback browsing is not implemented.

No internet/account, location, camera, microphone or nearby-device permission is added. AndroidX has its existing app-scoped signature guard permission. The app remains ARM64, minimum Android 10/API 29, compiled/targeted for Android 17/API 37. Device-native vault authentication and end-to-end SQLCipher/recovery acceptance on the S25 Ultra remain pending; passing host tests is not a security audit. Debug signing remains in use.

The build still does not include operational survival/first-aid content, species guides, real maps, family tracking or the AI assistant. Those follow the content/navigation/AI milestones. No photo recognition is an edibility test.
