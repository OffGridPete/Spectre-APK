# What's new

Newest first. This is the sideload APK at [OffGridPete/Spectre-APK](https://github.com/OffGridPete/Spectre-APK), not source. Each build below is what Settings shows as the Spectre version.

## 1.2.14 — 15 September 2026

- Android 12–14: Spectre could crash on the first BLE advertisement. Fixed. Android 15 still shows Public / Random from the stack.

## 1.2.13 — 15 September 2026

- The APK is not a debug build. With USB debugging on, adb can no longer read Spectre’s private data folder without root (including full GPS logs that Privacy mode only masks on screen).

## 1.2.12 — 15 September 2026

- At launch, BLE scanning starts about half a second after Wi-Fi and GPS. Workaround for phones that crashed when system Bluetooth and Location were both on.

## 1.2.11 — 15 September 2026

- BLE names come from the advertisement, not this phone’s paired list. A paired gadget with no advertised name shows as unnamed; Save name still labels that MAC.
- A bad scan batch no longer takes the whole scan service down.

This list starts at 1.2.11, when the sideload repository was opened. Older APKs in git history are not itemized here.
