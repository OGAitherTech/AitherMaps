# Aither Maps

Aither Maps is a fast, responsive, mobile-first map web app designed for iPhone, iPad, and desktop.

## Version

**1.0.0**

## Features

- Interactive world map powered by Leaflet
- Standard OpenStreetMap map
- Dark map style
- Satellite map style
- Place and address search using OpenStreetMap Nominatim
- Device location support
- Zoom controls designed for touch screens
- Map scale control
- Settings panel
- System, light, and dark themes
- Working Force Update button that clears cached app data and reloads
- Offline app-shell caching with a service worker
- Mobile-first layout with iPhone safe-area support
- Installable as a standalone web app through the included web manifest

## Run it

This is a static web app. Open `index.html` in a modern browser or deploy the repository with GitHub Pages.

## Map data and services

Map tiles and search data are provided by third-party services including OpenStreetMap, CARTO, Esri, and Nominatim. The app does not require a personal API key.

Please follow the usage policies and attribution requirements of each provider when deploying the app publicly.

## Files

- `index.html` — application UI and mobile metadata
- `style.css` — responsive styling, panels, themes, and mobile layout
- `app.js` — map setup, search, location, layers, settings, caching, and update logic
- `manifest.webmanifest` — install metadata
- `sw.js` — offline application-shell service worker

## Changelog

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
