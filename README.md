<div align="center">

# Delve

### A native macOS disk-usage visualizer

See exactly what's eating your disk — a cushioned, squarified treemap of every
file and folder, a drill-down tree list, an extensions breakdown, and one-click
cleanup. Built for Apple Silicon.

[![Download][download-badge]][latest]
[![Latest release][release-badge]][latest]
[![macOS 26+][macos-badge]][latest]

[**Download for macOS**][latest-dmg] · [Website][website] · [Release notes][releases]

</div>

---

## Download & install

1. Grab the latest **`Delve.dmg`** from the [releases page][latest].
2. Open the DMG and drag **Delve** into your **Applications** folder.
3. Launch it. Delve is signed and notarized by Apple, so it opens without warnings.

> **Requires macOS 26 or later** on Apple Silicon.

### Automatic updates

Delve updates itself via [Sparkle](https://sparkle-project.org). Once installed,
new versions download and install in the background — no need to come back here.
This repository hosts the Sparkle feed (`appcast.xml`) and the signed release
binaries that power those updates.

## What's in this repo

This is the **public release channel** for Delve — it ships the binaries and the
update feed, not the source.

| File | Purpose |
| --- | --- |
| [`appcast.xml`](appcast.xml) | The Sparkle update feed Delve polls for new versions |
| **Releases** | Each tagged release attaches the notarized, EdDSA-signed `Delve-<version>.dmg` |

Every release is built, signed, notarized, and published through an automated
pipeline; each appcast entry carries an EdDSA signature that the app verifies
before installing an update.

## Links

- 🌐 **Website:** [khaosstudio.com/delve][website]
- 📦 **All releases:** [github.com/snacbot/delve-releases/releases][releases]

## License

Delve is proprietary software. © 2026 Khaos Studios LLC. All rights reserved.

<!-- links -->
[latest]: https://github.com/snacbot/delve-releases/releases/latest
[latest-dmg]: https://github.com/snacbot/delve-releases/releases/latest/download/Delve.dmg
[releases]: https://github.com/snacbot/delve-releases/releases
[website]: https://khaosstudio.com/delve

<!-- badges -->
[download-badge]: https://img.shields.io/badge/Download-Delve.dmg-7c3aed?style=for-the-badge&logo=apple&logoColor=white
[release-badge]: https://img.shields.io/github/v/release/snacbot/delve-releases?style=for-the-badge&color=7c3aed&label=latest
[macos-badge]: https://img.shields.io/badge/macOS-26%2B-7c3aed?style=for-the-badge&logo=apple&logoColor=white
