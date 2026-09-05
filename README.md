# Aither Maps

A fast, mobile-first map web app with a desktop application for Windows, macOS, and Linux.

## Version

**3.5.1**

## Shared Aither Account

Aither Maps uses the same AitherBackend account service as the other Aither apps. Use the same email and password to access the same Aither account across the ecosystem.

- `POST /api/auth/register` — create an account
- `POST /api/auth/login` — sign in
- `GET /api/auth/session` — restore the current session
- `POST /api/auth/logout` — sign out
- Shared default backend: `https://aither-backend.onrender.com`
- Credentialed requests use the backend's HttpOnly session cookie
- Passwords are not stored in Aither Maps local storage

## Web Features

- Interactive Leaflet world map
- Standard, Dark, and Satellite map styles
- Place/address search
- Device location
- Saved Places
- Recent Searches
- Built-in driving navigation
- Route line, distance, ETA, and route-step preview
- Shared Aither account creation, sign-in, session restore, and sign-out
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

## Navigation

Aither Maps performs driving-route calculations inside the app. It geocodes the start and destination with Nominatim, requests a driving route from OSRM, draws the returned GeoJSON route on the map, and displays distance, ETA, and route steps.

## Changelog

### 3.5.1 — 2026-09-05

- Standardized Aither Maps on the shared `aither-backend.onrender.com` account service URL.
- Kept registration, login, session restore, and logout on the common AitherBackend API.
- Updated documentation for cross-service accounts.

### 3.5.0 — 2026-09-05

- Added Aither Backend-powered account creation and sign-in.
- Added secure credentialed session restoration and sign-out.
- Added mobile-friendly Aither Account UI.

### 3.4.0 — 2026-09-01

- Rebuilt the navigation experience as a proper in-app route planner.
- Added device-location start selection.
- Added start/destination swapping and route clearing.
- Added route distance, ETA, start/end markers, and step-by-step preview.
- Improved the navigation panel for mobile and desktop layouts.

### 3.3.0 — 2026-09-01

- Hardened and polished the Electron desktop application.
- Added secure preload bridge and disabled renderer Node integration.
- Added controlled geolocation permissions.
- Improved external URL handling.

### 3.2.0 — 2026-08-31

- Added Electron desktop application and cross-platform packaging workflow.
