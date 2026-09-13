# Spectre

Receive-only Wi-Fi access-point and Bluetooth LE watcher for Android. No dongle, no account, no backend. Everything lives on the phone.

This repository is **sideload files only** (APK, instruction card, user manual). It does not contain source.

Copyright (c) 2026 Off Grid Pete LLC. All rights reserved. Licensed under the [SPECTRE LICENSE](LICENSE).

## Put it on a phone

| File | What it is |
|---|---|
| `Spectre.apk` | Sideload APK |
| `instruction.txt` | Permissions, first launch, Samsung / One UI |
| `Spectre_User_Manual.pdf` | User manual |
| `LICENSE` | SPECTRE LICENSE |

Android 10+. Copy `Spectre.apk` onto the phone (USB, Drive, or Files) and open it. Allow install from the app you used to open the APK. Play Protect may warn that it is not from Play — expected. Full steps are in `instruction.txt`.

```bash
adb install -r Spectre.apk
```

SHA-256 of `Spectre.apk`:

```
bb3fe9e0e97718e26af280f7d954af768dec3993b04d58fb1940bfc600304bb5
```

## What Spectre is not

- Not Wi-Fi clients, probe-only stations, or 802.11 monitor mode
- Not Bluetooth Classic inquiry (HC-05 / HC-06 will not appear)
- Not cellular
- Not direction finding

If you spot an error in the docs, get in touch (Instagram @OffGridPete, X @OGridPete).
