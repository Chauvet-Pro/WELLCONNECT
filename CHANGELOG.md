# Changelog

All notable changes to this project will be documented in this file.

---

## [4.1.10] 2026-03-30 Box Firmware Update

### New Features

- **Custom Chase Effect** *(App)* — Design custom chase sequences with multiple color positions, speed, spread, and direction controls.
- **Auto Program Effect** *(App)* — Automated lighting effects with less manual setup. Blue glow indicates active fixtures.
- **Favorite Colors** *(App)* — Save up to 12 colors for quick access from the color picker. Saved per project.
- **Freedom Profiles** *(App)* — Added Freedom series fixture profile support.
- **Scene Recording & Playback** *(App & Device)* — Record live DMX at 44 fps with Normal, Loop, and Delay modes. Manage recordings from app, device menu, or Web UI. Recorded scenes are clearly marked and non-editable in the app.
- **REST API** *(Device)* — Local API server on port 3002 for scenes, dimmer, status, and recorded scene control. Off by default; local network only.
- **Web UI** *(Device)* — Redesigned browser-based control panel with scene control, firmware updates, API docs, and time zone settings. Auto-detects product branding.
- **sACN Improvements** *(Device)* — Improved sending/receiving with 40 Hz rate limiting and hot reconfiguration.
- **Facebook Community & Spain Contact** *(App)* — Direct link to the Facebook User Group and Spain contact info in Help.

### Improvements

- **Bluetooth Stability** *(App & Device)* — Device auto-configures connection parameters on first boot. App fixes stale commands on reconnect, duplicate listeners, and Bluetooth queue flooding during color picking.
- **Smarter Profile Selection** *(App)* — WDMX/D-Fi toggle auto-matches the selected profile type.
- **Group Deletion Protection** *(App)* — Can't delete groups used in saved scenes. New options menu for groups.
- **Scene Naming** *(App)* — Limited to 20 characters with auto-focus and cleaner UI.
- **Scene Start Throttle** *(App)* — Cooldown prevents accidental double-taps.
- **Faster Pop-Ups & Better Android Keyboard** *(App)* — Instant modals; proper keyboard resize on Android.
- **Fixture Shape Glow Effects** *(App)* — All shapes support white/blue glow halos.
- **Branding Update** *(App)* — "WELL CONNECT" renamed to "CONNECT Box" throughout.
- **On-Screen Display** *(Device)* — Home screen shows current scene; factory reset renamed "Delete Data & Restart"; recording status indicators added.
- **Network & Connectivity** *(Device)* — Fixed subnet mask alias bug, added Art-Net broadcast IP config, async DMX alias setup.
- **Reliability** *(Device)* — Improved shutdown handling, Art-Net stability, and general crash resilience.
- **Settings Migration & Time Sync** *(Device)* — Auto-migrates settings on update; clock syncs over network.
- **Updated Fixture Library** *(App & Device)* — Profiles updated to v2.2.7.

### Bug Fixes

- **Amber & UV Channel Data** *(App)* — All seven color channels (RGBWAUD) now saved correctly.
- **Scene Recording Sync** *(App)* — Local recordings protected during CONNECT Box sync.
- **YouTube Tutorials & Offline Banner** *(App)* — Video playback and banner sizing fixed.
- **Scene Start Timing & Auto Program Blocking** *(App)* — Scheduling and mode-lock bugs resolved.
- **Recorder Settings** *(Device)* — Duration/mode changes now apply correctly.
- **Scene Playback Display** *(Device)* — OLED now shows the correct playing scene.
- **Network & Boot Fixes** *(Device)* — Alias reconfiguration and DMX boot blocking resolved.
- **General Crash Fixes** *(Device)* — Multiple stability issues resolved.

### Platform & Compatibility *(App)*

- Android 15+ support (16KB memory pages), locked dependency versions, updated iOS & Android builds.

### Easter Egg *(Device)*

- A hidden mini-game in the Web UI. Can you find it?
