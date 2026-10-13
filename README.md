# CineFlow

Modern, ad-free multimedia player and streaming media center for Android & Android TV.

[![Build CineFlow APK](https://github.com/jahru23/cineflow-app/actions/workflows/build-apk.yml/badge.svg)](https://github.com/jahru23/cineflow-app/actions/workflows/build-apk.yml)
[![Latest Release](https://img.shields.io/github/v/release/jahru23/cineflow-app?include_prereleases&label=release)](https://github.com/jahru23/cineflow-app/releases/latest)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)

---

## Overview

**CineFlow** is an open-source media player designed with complete freedom, zero advertisements, and robust privacy. The app separates player architecture from content sources using a modular plugin engine.

### Key Features

* **Ad-Free & Privacy First:** Zero trackers, zero analytics, zero banner or pop-up advertisements.
* **Pre-seeded Extension Ecosystem:** Connected out-of-the-box with [CineFlow Extensions](https://github.com/jahru23/cineflow-extensions).
* **Bypass ISP Filtering:** DNS-over-HTTPS (DoH via Cloudflare 1.1.1.1) enabled by default to prevent connection dropouts.
* **Intelligent Subtitles:** Automatic detection and prioritization for Indonesian (`id`) and multi-language subtitles.
* **Material You Dynamic Theming:** Adaptive color palettes (Monet engine) for Android 12+ alongside pure AMOLED dark mode.
* **Modern Media Player:** Integrated ExoPlayer engine supporting Picture-in-Picture (PiP), gesture controls, subtitle customization, and Chromecast.
* **Cross-Device Support:** Built for standard Android smartphones, tablets, and Android TV (leanback UI with remote D-Pad navigation).

---

## Download & Installation

Get the latest installable APKs directly from GitHub Releases:

* **[Download Latest CineFlow APK](https://github.com/jahru23/cineflow-app/releases/latest)**

Available packages per architecture:
* `CineFlow-1.0.0-arm64.apk` (Recommended for modern smartphones and Android TV)
* `CineFlow-1.0.0-universal.apk` (Compatible with all supported ABIs)

---

## Extension Repository

CineFlow utilizes dynamic modular plugins (`.cs3` packages):
* Repository URL: `https://raw.githubusercontent.com/jahru23/cineflow-extensions/builds/repo.json`
* Source Code: [jahru23/cineflow-extensions](https://github.com/jahru23/cineflow-extensions)

---

## Building from Source

### Prerequisites
* JDK 17 (Temurin recommended)
* Android SDK Platform 36/37
* Gradle 8.x

### Build Commands
```bash
git clone https://github.com/jahru23/cineflow-app.git
cd cineflow-app
chmod +x gradlew

# Build release APK
./gradlew assembleStableRelease
```

Compiled APKs will be located in `app/build/outputs/apk/stable/release/`.

---

## License

This project is licensed under the GNU General Public License v3.0 (GPL-3.0). See [LICENSE](LICENSE) for details.
