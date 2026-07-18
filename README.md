# Vlither Enhanced

> **The Arena, Re-Engineered.**  
> A native Android client engineered and maintained by **OM Rajput**.

[![Latest release](https://img.shields.io/github/v/release/disis-om/vlither-enhanced-releases?display_name=tag&style=for-the-badge&label=LATEST&color=10b981)](https://github.com/disis-om/vlither-enhanced-releases/releases/latest)
[![Android](https://img.shields.io/badge/ANDROID-8.0%2B-111827?style=for-the-badge&logo=android&logoColor=10b981)](https://github.com/disis-om/vlither-enhanced-releases/releases/latest)
[![Architecture](https://img.shields.io/badge/ARCH-ARM64--V8A-111827?style=for-the-badge)](https://github.com/disis-om/vlither-enhanced-releases/releases/latest)
[![Signed](https://img.shields.io/badge/APK-PRODUCTION%20SIGNED-111827?style=for-the-badge&logo=letsencrypt&logoColor=10b981)](RELEASE_POLICY.md)

## What is Vlither Enhanced?

Vlither Enhanced is a purpose-built Android interpretation of the Vlither
desktop client: native rendering, real mobile controls, device-aware resource
work and a focused interface designed for touch. It keeps the fast arena
experience at the centre while rebuilding the surrounding client for Android
instead of wrapping a desktop window or shipping a browser shell.

Version **1.1.0** is the first official public release and the new foundation
for every release that follows.

## Download

### [Download Vlither Enhanced v1.1.0](https://github.com/disis-om/vlither-enhanced-releases/releases/download/v1.1.0/Vlither-Enhanced-v1.1.0.apk)

Always download from this repository's **Releases** page. APK files are
attached to immutable versioned releases and are never committed into the Git
history.

## The 1.1.0 experience

| System | What it delivers |
| --- | --- |
| **Native arena** | Vulkan-backed rendering and an arm64 Android build tuned for responsive play. |
| **Mobile control suite** | Left- or right-handed layouts, floating or fixed joystick/boost behavior, draggable control positions, zoom control, size and opacity tuning. |
| **Unified interface** | A graphite-and-emerald visual system across Home, Settings, Controls and Update Center. |
| **Skin workshop** | The renderer-driven snake preview, color palette and accessory workflow preserved inside the refreshed client. |
| **Resource optimization** | Reworked background and atlas assets reduce GPU texture pressure while retaining the visual identity of the arena. |
| **Update Center** | Signed GitHub update architecture, visible progress states and a reserved publisher channel for future expansion. |
| **Backup Vault** | User-owned backups for nickname, skin, gameplay, graphics and control preferences before future updates. |

## Install in four steps

1. Open the [latest release](https://github.com/disis-om/vlither-enhanced-releases/releases/latest).
2. Download `Vlither-Enhanced-v1.1.0.apk`.
3. Allow installation from your browser or file manager when Android asks.
4. Open **Vlither Enhanced**, enter a nickname and server address, then press **Play**.

Android may display an unknown-source warning because Vlither Enhanced is
distributed independently rather than through the Play Store. Verify that the
APK came from `disis-om/vlither-enhanced-releases` before installing it.

## Compatibility

- Android 8.0 / API 26 or newer
- 64-bit ARM device (`arm64-v8a`)
- Vulkan-capable Android graphics stack
- Internet connection for server play and update checks
- Landscape orientation recommended

Device firmware, GPU drivers and vendor-specific Android behavior can affect
compatibility. When reporting an issue, include the phone model, Android
version, GPU name and the exact behavior observed.

## Release integrity

The official v1.1.0 APK is identified by:

```text
Package:      com.vlither.enhanced
Version:      1.1.0
Version code: 10100
APK size:     9,262,081 bytes
SHA-256:      dd006c5d2beeeaa1c5319dcceb427032997f64d8d83b28ff164823c47152fb93
Certificate:  a0d556a4e00c1e8a1949e40cace32f8b13a23c7f354ba1d7ea9c0f95f8a840b5
```

Future updates must preserve the package identity and production signing
certificate. Release tags and APK bytes are immutable; a correction is always
published as a newer version.

## Release archive and documentation

- [Complete v1.1.0 changelog](changelogs/v1.1.0.md)
- [Release policy](RELEASE_POLICY.md)
- [GitHub update architecture](docs/update-system.md)
- [All GitHub Releases](https://github.com/disis-om/vlither-enhanced-releases/releases)

## Road ahead

The **1.1.x** line establishes the Android client, visual system, control
foundation and secure distribution path. Development now moves toward
**Vlither Enhanced 1.2.0**, with future work building on this baseline rather
than fragmenting it into separate experimental editions.

---

### Built with intent by OM Rajput

Vlither Enhanced is developed, signed and maintained by **OM Rajput**. This
repository contains public release material only; private application source,
signing keys and deployment credentials are deliberately excluded.

Vlither Enhanced is an independent community project and is not presented as
an official Slither.io application.
