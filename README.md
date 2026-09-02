# Aither Maps

A fast, mobile-first map web app with a desktop application for Windows, macOS, and Linux.

## Version

**3.4.0**

## What's new in 3.4

- 🧭 **Built-in driving navigation** now calculates routes directly inside Aither Maps
- 📍 **Use My Location** fills the navigation starting point from the device location
- 🔄 **Swap** start and destination with one tap
- 🗺️ Route line is rendered directly on the Leaflet map
- 📏 Navigation shows route distance and estimated travel time
- 🧾 Full route-step preview with maneuver and distance details
- 🧹 Clear the active route without reloading the app
- 📱 Improved navigation panel for iPhone and small screens
- 🖥️ Desktop app continues to use the same navigation interface

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

Aither Maps performs driving-route calculations inside the app. It geocodes the start and destination with Nominatim, requests a driving route from OSRM, draws the returned GeoJSON route on the map, and displays distance, ETA, and route steps. Routing requires an internet connection and is subject to the OpenStreetMap, Nominatim, and OSRM services' availability and usage policies.

This is route planning and step preview; it is **not** a full live turn-by-turn navigation system with continuous voice guidance.

## Changelog

### 3.4.0 — 2026-09-01

- Rebuilt the navigation experience as a proper in-app route planner.
- Added device-location start selection.
- Added start/destination swapping and route clearing.
- Added route distance, ETA, start/end markers, and step-by-step preview.
- Improved the navigation panel for mobile and desktop layouts.
- Kept README version and feature documentation synchronized.

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

- Added initial built-in navigation and route rendering.

### 3.0.0 — 2026-08-31

- Added Directions, Recent Searches, and Clear Saved Data.

### 2.0.0 — 2026-08-31

- Added Saved Places.

### 1.0.0 — 2026-08-31

- Initial Aither Maps rebuild.
