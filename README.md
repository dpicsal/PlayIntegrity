# PlayIntegrity

> Free universal fix for Play Integrity & SafetyNet on Android 10-16

**Author:** Panda
**Telegram:** [@cpanda_app](https://t.me/cpanda_app)

---

## Features

- Fixes **Play Integrity API** (MEETS_BASIC, DEVICE, STRONG)
- Fixes **SafetyNet** (basicIntegrity, ctsProfile)
- Supports **Magisk**, **KernelSU**, and **APatch**
- Auto fetches latest **Pixel Beta fingerprint** via Action button
- Works on Android **10 through 16**
- Spoofs props for Samsung, Realme, OnePlus, Oppo, Xiaomi

## Installation

1. Download the latest zip from [Releases](https://github.com/dpicsal/PlayIntegrity/releases)
2. Flash via Magisk / KernelSU / APatch
3. Reboot
4. (Optional) Tap **Action** button in your module manager to refresh fingerprint

## How It Works

| Layer | What it does |
|---|---|
| Zygisk `.so` | Hooks into GMS process, spoofs attestation |
| `classes.dex` | Intercepts Java-level integrity API calls |
| `post-fs-data.sh` | Spoofs build props at early boot |
| `service.sh` | Hides SELinux/bootloader state at late boot |
| `autopif2.sh` | Fetches fresh Pixel Beta fingerprint on demand |

## Support

- Telegram: [t.me/cpanda_app](https://t.me/cpanda_app)
