# Spectre

I built Spectre as a personal tool to look at what Wi-Fi access points and Bluetooth LE ads my phone was able to pick up, so that I could better understand what devices were being used around me. It’s passive, it only listens, there’s no dongle, no account, and no backend server. I wanted something that would work offline in the field.

My goals were to have a modern interface that was easy to use, flexible in how information was displayed so I could customize a view based on what I was trying to do, a filtering engine so I do not have to look at everything, an extensible signature library so I can identify as many radio sources as possible and add new ones on the fly, as well as create reports of what was seen.

I have been using it and iterating on it for a while now, and it has been useful enough that I thought I would share it.

This is a hobby — something I do for fun in my spare time. There is no Spectre backend. There are no ads. Everything lives on the phone. This repository is the sideload set: APK, instruction card, and user manual.

If you spot an error, something stupid, or have a feature idea — in the app or the documentation — please [open an issue on this repository](https://github.com/OffGridPete/Spectre-APK/issues). This repository is sideload files only; do not send a pull request. This is how we make it better. I hope you find it as useful as I have. I look forward to hearing how it goes.

## First steps

1. Download `Spectre.apk` from this repo (the file in GitHub, not a copy from chat).
2. Check its SHA-256 against the hash under **Put it on a phone**.
3. Sideload it. Spectre is not on the Play Store. Play Protect may warn that the app is not from Play — expected. Install anyway only if you trust this file. Steps: `instruction.txt`.
4. Read the Notice in `Spectre_User_Manual.pdf` (page after the cover) and the first-run **Disclaimer and license** screen before you scan.

## Safety & disclaimer

This is a hobby project, provided as-is under the SPECTRE LICENSE. A few things to know before you do:

- Use at your own risk. Using Spectre is your responsibility. To the maximum extent permitted by law, Off Grid Pete LLC is not liable for indirect, incidental, special, consequential, or punitive damages arising from its use.
- There is no guarantee that trackers, cameras, tags, access points, or any other device will be found, named, or reported. Radios that are off, cellular-only, asleep, randomized, quiet, or outside what this handset’s OS exposes will not appear. Each phone has its own radios, firmware, scan quotas, and OEM battery policies. Software cannot address those limits.
- Pattern matches, GPS co-travel (“Moving with you” / “possible tail”), Debrief language, and AI Export output are hypotheses — not identity, not a legal finding, and not a complete RF capture. You are solely responsible for how you use this app and this document, and for complying with local law. By using the software or this manual you accept these terms and the SPECTRE LICENSE.
- Location data, if tagging is on, is this phone at hear-time — not the other radio. There is no Spectre server. Stamps stay on the handset until you share them. Logs keep full coordinates even when Privacy mode masks the screen and sit reports. Debrief, Share log, AI Export (sit or one radio), and radio-detail Share as text can take that path off the phone. Online place names use the system geocoder (often the OEM / Google network), not a Spectre cloud. How you store, share, or publish those files is your responsibility.

## Put it on a phone

| File | What it is |
|---|---|
| `Spectre.apk` | Sideload APK |
| `instruction.txt` | Permissions, first launch |
| `Spectre_User_Manual.pdf` | User manual |
| `CHANGELOG.md` | What changed in each build |
| `LICENSE` | SPECTRE LICENSE |

Android 10+. Copy `Spectre.apk` onto the phone (USB, Drive, or Files) and open it. Allow install from the app you used to open the APK. Play Protect may warn that it is not from Play — expected. Full steps are in `instruction.txt`.

```bash
adb install -r Spectre.apk
```

SHA-256 of `Spectre.apk`:

```
ba28c2a9ec3163a22456e803726f0e73a53eafa6543de30259be7a2761e26974
```

What changed in each build: [CHANGELOG.md](CHANGELOG.md).

## What Spectre is not

- Not Wi-Fi clients, probe-only stations, or 802.11 monitor mode
- Not Bluetooth Classic inquiry (HC-05 / HC-06 will not appear)
- Not cellular
- Not direction finding

## Copyright and license

Copyright (c) 2026 Off Grid Pete LLC. All rights reserved.

Spectre is licensed under the [SPECTRE LICENSE](LICENSE). Personal, revocable use of the free edition on devices you own or control. No public redistribution, sale, or representing the software as your own. Full terms in `LICENSE`.
