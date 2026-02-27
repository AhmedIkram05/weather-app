# Weather App

**Offline-capable PWA for real-time weather data — city search, geolocation, unit toggle, and service worker caching.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20App-blue?style=for-the-badge)](https://ahmedikram05.github.io/weather-app/)

---

## What It Does

A lightweight weather PWA built with vanilla JavaScript and the OpenWeatherMap One Call 3.0 API. Search any city worldwide or use your device's geolocation for instant local conditions. Toggle between Celsius and Fahrenheit. Works offline via service worker caching.

**[→ Live Demo](https://ahmedikram05.github.io/weather-app/)**

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| API | OpenWeatherMap One Call 3.0 + Geocoding |
| PWA | Service Worker + Web App Manifest |

---

## Features

- **City search** — find current conditions and forecasts for any city worldwide
- **Geolocation** — auto-detect location for instant local weather
- **Unit toggle** — switch between Metric (°C) and Imperial (°F)
- **Offline support** — service worker caches assets and recent API responses
- **Responsive** — works on mobile, tablet, and desktop
- **Installable** — add to home screen on any device

---

## How to Run Locally

Service workers require HTTPS or `localhost` — you can't just open `index.html` directly.

**Python:**
```bash
git clone https://github.com/AhmedIkram05/weather-app.git
cd weather-app
python3 -m http.server 8000
```

**Node:**
```bash
npx http-server .
```

Then open `http://localhost:8000`.

### API Key

The app uses an embedded OpenWeatherMap key in `app.js`. To use your own:

1. Sign up at [openweathermap.org](https://openweathermap.org/)
2. Get a free API key (One Call 3.0 requires a free account)
3. Replace `OWM_KEY` in `app.js` with your key

---

## Project Structure

```
weather-app/
├── index.html          # App shell
├── app.js              # Core logic — API calls, geolocation, UI updates
├── style.css           # Styles
├── service-worker.js   # Caching + offline support
├── manifest.json       # PWA manifest
└── weather-icon.png    # App icon
```
