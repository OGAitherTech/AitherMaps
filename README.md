# Aither Maps

Aither Maps is a fast, responsive, mobile-first map web app designed for iPhone, iPad, and desktop.

## Version

**2.0.0**

## What's new in 2.0

- Saved Places with local storage
- Save a searched place directly from its map popup
- Saved Places menu in the sidebar
- Expanded search results
- Improved selected-location handling
- Map style confirmation toast
- Updated mobile UI and version display
- Settings and Force Update retained from v1

## Features

- Interactive world map powered by Leaflet
- Standard OpenStreetMap map
- Dark map style
- Satellite map style
- Place and address search using OpenStreetMap Nominatim
- Device location support
- Touch-friendly zoom controls
- Map scale control
- Saved Places
- Settings panel
- System, light, and dark themes
- Working Force Update button that clears cached app data and reloads
- Offline app-shell caching with a service worker
- Mobile-first layout with iPhone safe-area support
- Installable as a standalone web app

## Run it

This is a static web app. Open `index.html` in a modern browser or deploy the repository with GitHub Pages.

## Map data and services

Map tiles and search data are provided by third-party services including OpenStreetMap, CARTO, Esri, and Nominatim. The app does not require a personal API key.

Please follow the usage policies and attribution requirements of each provider when deploying the app publicly.

## Files

- `index.html` — application UI and mobile metadata
- `style.css` — responsive styling, panels, themes, and mobile layout
- `app.js` — map, search, location, saved places, layers, settings, and update logic
- `manifest.webmanifest` — install metadata
- `sw.js` — offline application-shell service worker

## Changelog

### 2.0.0 — 2026-08-31

- Upgraded Aither Maps from 1.0.0 to 2.0.0.
- Added Saved Places stored locally on the device.
- Added a Save Place action to search-result map popups.
- Added a Saved Places sidebar section.
- Expanded place search results from 6 to 8.
- Improved map marker selection behavior.
- Added layer-change feedback.
- Updated the README and version display.

### 1.0.0 — 2026-08-31

- Rebuilt the repository as Aither Maps.
- Added an interactive Leaflet map.
- Added place and address search.
- Added device-location support.
- Added standard, dark, and satellite map styles.
- Added mobile touch controls and iPhone safe-area support.
- Added settings with theme, map style, scale, and Force Update controls.
- Added offline application-shell caching and a service worker.
- Added installable web-app metadata.
