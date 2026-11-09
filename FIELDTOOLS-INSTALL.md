# AEGIS 0.6.0 — kit, plans, waypoints, GPS and compass

Install **AEGIS-fieldtools-S25-0.6.0.apk over AEGIS 0.3/0.4/0.5 without uninstalling**. Same package and development signer. Existing guides, language packs, bookmarks, pins and appearance remain. The encrypted vault upgrades its schema and retains notes. Do not downgrade afterwards. The separate Feasibility app stays separate.

On Home:

- **Open kit and household plans** → confirm Android screen lock → Kit / Plans / Waypoints / Notes. A secure device PIN, pattern or password is required for private records.
- **Kit:** add/edit/delete supplies, quantity/unit, category, storage, expiry/replacement, priority and notes. Search or show records due for review. Dates are YYYY-MM-DD and evaluated against today's UTC date while open; no background notifications.
- **Plans:** choose a scenario, add custom tasks or organizing prompts, edit and mark complete. These are your household planning records, not emergency response procedures.
- **Waypoints:** enter named WGS84 decimal coordinates, edit/delete them, or select Bearing and distance. Destinations are user-entered and unverified.
- **Notes:** existing encrypted notes remain. **Back up everything** / **Back up vault** exports all four record types under a separate generated recovery code. Keep that code separately. Older notes-only backups still restore, but restore replaces the ENTIRE active vault, including kit/tasks/waypoints; confirm the warning carefully.

**Open GPS and compass:** the compass uses actual sensors when available. Tap Start GPS and allow precise location to use the GNSS provider. Go outside with a clear view of the sky if waiting for a fix. GPS does not require internet. No background location permission is requested. Refusal leaves the library and inventory usable.

A received fix shows coordinates, reported accuracy, age/time and available speed/ellipsoidal altitude. The compass indicates magnetic north; target bearing is true and is not corrected for magnetic declination. Sensor presence is not proof of accuracy or calibration. Straight-line bearing/distance is not a navigable or safe route.

**Start new track** records foreground breadcrumbs with a relative sketch, not a geographic map. Keep this screen open. Points clear when leaving the screen, stopping GPS or starting a new track; they are not persistent/background tracks. Use **Set track start as target** for a straight-line bearing back to the first recorded point; this does not supply a route. Export GPX BEFORE leaving if you want a file. Export asks explicitly because GPX contains unencrypted locations/times. The file picker pauses the live session; the captured export can still be saved. A cancelled or failed export may leave no usable file. Do not rely on these development tools as your sole navigation equipment.

New native hardware/vault paths require S25 device verification and security review; use nonsensitive test records meanwhile. No internet/account, cloud AI, camera/microphone or nearby communication is added. Minimum Android10/API29, target Android17/API37, ARM64. Reviewed first aid, edible-species references, geographic maps, remote tracking and integrated AI remain unfinished. Optional draft Filipino/Czech guide packs remain under Library → Guide packs; app controls remain English.
