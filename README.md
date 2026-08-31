# Aither Weather

Aither Weather is a fast, responsive weather web app designed for iPhone, iPad, and desktop. It uses Open-Meteo for current conditions and forecasts and requires no API key.

## Version

**1.0.0**

## Features

- Current temperature and conditions
- Feels-like temperature
- Humidity, wind, pressure, and UV index
- 12-hour scrolling forecast
- 7-day forecast
- Search for cities and ZIP codes
- Use device location
- Fahrenheit and Celsius
- System, light, and dark themes
- Settings panel
- Working Force Update button that clears cached app data and reloads
- Offline fallback using the most recently loaded forecast
- Mobile-first layout with iPhone safe-area support
- Installable as a standalone web app through the included web manifest

## Run it

This is a static web app. Open `index.html` in a modern browser or deploy the repository with GitHub Pages.

## Weather provider

Weather data is provided by Open-Meteo. The app calls its public forecast and geocoding endpoints directly from the browser, so no personal API key is stored in this repository.

## Files

- `index.html` — application UI
- `style.css` — responsive styling and themes
- `app.js` — weather API, search, location, settings, caching, and update logic
- `manifest.webmanifest` — mobile install metadata

## Changelog

### 1.0.0 — 2026-08-31

- Created Aither Weather from the AitherMaps repository.
- Added responsive weather dashboard.
- Added search and device-location weather lookup.
- Added hourly and seven-day forecasts.
- Added settings, unit switching, themes, offline cache, and Force Update.
- Added mobile web app manifest.
