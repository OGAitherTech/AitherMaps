# Aither Maps

A fast, mobile-first map web app with a desktop application for Windows, macOS, and Linux.

## Version

**3.3.0**

## What's new in 3.3

- 🖥️ Improved **Aither Maps Desktop** experience
- 🔐 Hardened Electron security with preload/context isolation
- 📍 Controlled desktop geolocation permission handling
- 🔗 Safer external-link handling
- 🔄 Dedicated Reload Map and Force Reload desktop actions
- ⛶ Fullscreen and zoom controls from the desktop menu
- 📦 Pinned Electron and electron-builder versions for more repeatable builds
- 🪟 Windows NSIS + portable targets
- 🍎 macOS DMG target
- 🐧 Linux AppImage target
- ⚙️ Cross-platform GitHub Actions desktop build workflow

## Web Features

- Interactive Leaflet world map
- Standard, Dark, and Satellite map styles
- Place/address search
- Device location
- Saved Places
- Recent Searches
- Built-in driving navigation
- Route line, distance, ETA, and route-step preview
- Settings, themes, and Force Update
- Offline application-shell caching
- iPhone safe-area support
- Installable web app

## Desktop App

The desktop app is in `desktop/` and uses Electron to run the same Aither Maps interface.

### Development

```bash
cd desktop
npm install
npm start
```

### Build

```bash
cd desktop
npm install
npm run build
```

The configured build targets are Windows (`NSIS` and portable), macOS (`DMG`), and Linux (`AppImage`).

GitHub Actions can build the desktop packages from `.github/workflows/desktop.yml` using a `desktop-v*` tag or a manual workflow run.

## Navigation

Aither Maps calculates driving routes inside the app using OSRM and Nominatim. Routing requires an internet connection and is subject to those services' availability and usage policies.

## Changelog

### 3.3.0 — 2026-09-01

- Hardened and polished the Electron desktop application.
- Added secure preload bridge and disabled renderer Node integration.
- Added controlled geolocation permissions.
- Improved external URL handling.
- Added desktop navigation/reload controls.
- Pinned desktop build dependencies.
- Expanded desktop build documentation.

### 3.2.0 — 2026-08-31

- Added Electron desktop application and cross-platform packaging workflow.

### 3.1.0 — 2026-08-31

- Added built-in navigation and route rendering.

### 3.0.0 — 2026-08-31

- Added Directions, Recent Searches, and Clear Saved Data.

### 2.0.0 — 2026-08-31

- Added Saved Places.

### 1.0.0 — 2026-08-31

- Initial Aither Maps rebuild.
