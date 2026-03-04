<div align="center">

# Muzic
### Local Audio Architecture

[![Latest Release](https://img.shields.io/github/v/release/officialtechrom/Muzic-Releases?style=for-the-badge&color=7C4DFF&label=Latest%20Release)](https://github.com/officialtechrom/Muzic-Releases/releases/latest)
[![Android](https://img.shields.io/badge/Android-10%2B-brightgreen?style=for-the-badge&logo=android)](https://github.com/officialtechrom/Muzic-Releases/releases/latest)

</div>

## Download

**[Download the latest release APK here](https://github.com/officialtechrom/Muzic-Releases/releases/latest)**

For an archive of all versions, view the **[Releases](https://github.com/officialtechrom/Muzic-Releases/releases)** page.

## System Capabilities

| Capability | Technical Details |
|---------|-------------|
| **Offline Architecture** | Operates fundamentally without network requests or API dependencies. |
| **Clean Distribution** | No advertisement SDKs, telemetry, or third-party wrappers injected. |
| **Format Support** | Lossless (FLAC, WAV, ALAC) & Lossy (OPUS, OGG, AAC, MP3) audio decoding via ExoPlayer. |
| **Material Theming** | AMOLED-optimized dark contrast rendering engineered with Jetpack Compose. |
| **Library Indexing** | Local asynchronous MediaStore parsing (Songs, Albums, Artists, Playlists). |
| **Persistent Playback** | Global MiniPlayer state maintained across UI components via Kotlin Flow. |
| **State Management** | Room database persistence for Playlists and Favorites indexing. |
| **MediaSession Integration** | Hardware Bluetooth event parsing, lock screen, and system notification controls. |

## Requirements

- Android Minimum: API Level 29 (Android 10)
- Architecture Support: ARM64-v8a / ARMEABI-v7a
- Storage Authorization: `READ_MEDIA_AUDIO` / `READ_EXTERNAL_STORAGE`

## Installation Context

1. Acquire the `.apk` from the **[Releases](https://github.com/officialtechrom/Muzic-Releases/releases/latest)** output stream.
2. Execute the file via the Android package manager.
3. If necessary, approve the "Install from Unknown Sources" security constraint in settings.
4. On initialization, grant local storage permission when the system dialogue prompts.

## Development Roadmap

- [x] v1.0.0 — Core engine initialization, MediaStore mapping, base UI components.
- [x] v2.0.0 — Compose UI paradigm shift, Bottom navigation architecture, persistent state.
- [ ] v2.1.0 — Direct system audio hooks (10-band Equalizer, Bass Boost algorithms).
- [ ] v2.2.0 — Relational smart playlist generation based on playback metrics.

## Privacy & Telemetry Statement

Muzic enforces strict local-only data policies at the manifest level:

- **Network Interface Disabled:** The `INTERNET` permission is omitted from the Android Manifest. The binary physically cannot transmit data.
- **Analyzation Tools Removed:** No logging libraries, crash reporters (e.g., Firebase, Sentry), or metric trackers are bundled.
- **Local Sandbox:** All indexing databases reside strictly in the app's local user-secured storage sandbox.

## Issue Tracking

For crash reports or feature proposals, please submit reproducible logs in the **[Issues](https://github.com/officialtechrom/Muzic-Releases/issues)** section.

## License

© 2026 officialtechrom. Maintained for personal application engineering. All rights reserved.

## v2.1.0 - Final UI & UX Improvements
- **Features:** Fully functional Search Screen, Pull-down to dismiss MiniPlayer.
- **Fixes:** Fixed background notifications bug, removed duplicate Developer option, restored Material 3 smooth SeekBar.
- **Refinement:** UI and animation improvements.

