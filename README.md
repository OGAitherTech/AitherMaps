# Aither Maps

A fast, mobile-first map web app for iPhone, iPad, and desktop.

## Version

**3.1.0**

## What's new in 3.1

- 🧭 **Built-in navigation** — routes are calculated and drawn directly on the Aither Maps map.
- 📍 Start and destination addresses are geocoded inside the app.
- 🛣️ Route line is displayed directly on the map.
- ⏱️ Distance and estimated travel time are shown in the Directions panel.
- ➤ **Route here** action is available directly from a searched place.
- No redirect to an external directions page is required.

## Features

- Interactive Leaflet world map
- Standard OpenStreetMap map
- Dark map style
- Satellite map style
- Place/address search with Nominatim
- Device location support
- Touch-friendly zoom controls
- Map scale control
- Saved Places
- Recent Searches
- Built-in driving route calculation
- Route distance and ETA
- Route preview on the map
- Settings and themes
- System, light, and dark themes
- Offline application-shell caching
- iPhone safe-area support
- Installable standalone web app

## Navigation

Open **Directions** from the arrow button on the map, enter a starting point and destination, and Aither Maps will geocode both locations and request a driving route. The route is then rendered directly on the map with distance, ETA, and a short preview of route steps.

The routing engine is OSRM and the geocoding service is Nominatim. Both are external services, so routing requires an internet connection and is subject to their availability and usage policies.

## Run it

Open `index.html` in a modern browser or deploy the repository with GitHub Pages.

## Data and services

Map tiles and search/routing data use third-party services including OpenStreetMap, CARTO, Esri, Nominatim, and OSRM. The app does not require a personal API key.

## Changelog

### 3.1.0 — 2026-08-31

- Replaced the external Directions redirect with built-in route calculation.
- Added Nominatim geocoding for route endpoints.
- Added OSRM driving routes.
- Added route rendering directly on the Leaflet map.
- Added route distance and ETA.
- Added a short route-step preview.
- Added Route here from searched place popups.

### 3.0.0 — 2026-08-31

- Added Directions shortcut and panel.
- Added Recent Searches.
- Added Clear Saved Data.
- Improved mobile UI and touch feedback.

### 2.0.0 — 2026-08-31

- Added Saved Places and save-from-popup support.

### 1.0.0 — 2026-08-31

- Initial Aither Maps rebuild.
