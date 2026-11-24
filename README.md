# Claude Local — updates

This repository holds only the **signed releases** of Claude Local:
- the desktop app (Windows),
- the Android app.

The source code is kept elsewhere.

Every installation checks the latest release on its own:
- every 30 minutes, and right away when another computer in the owner's network announces a new version;
- it verifies the ed25519 signature of `manifest.json` and the sha256 of each file;
- it updates automatically, or on a click (setting: auto / on demand / off).

Each release contains:
- `manifest.json`: version, build, sha256 and size of each file, and the signature;
- `claude-local-app-<build>.zip`: the app code;
- `claude-local-<build>.apk`: the Android app, delivered to phones through their own computer.
