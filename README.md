# API Weather App (PWA)

## 🚀 Overview
A lightweight Progressive Web App (PWA) that provides real-time weather updates and forecasts. Built with vanilla JavaScript and the OpenWeatherMap One Call 3.0 API, it offers a seamless experience across devices with offline capabilities.

## 🧠 Tech Stack
- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **API:** OpenWeatherMap (One Call 3.0 & Geocoding)
- **PWA:** Service Workers, Web App Manifest

## 📊 Features
- **City Search:** Instantly find weather data for any city worldwide.
- **Geolocation:** Auto-detect current location for local weather updates.
- **Unit Conversion:** Toggle between Metric (°C) and Imperial (°F) units.
- **Offline Support:** Caches assets and API responses for offline access.
- **Detailed Forecast:** Displays current conditions, temperature, and forecast data.

## 📈 Results
- **Performance:** Fast load times due to minimal dependencies and efficient caching.
- **Accessibility:** Semantic HTML and ARIA labels for better accessibility.
- **Reliability:** Works offline or on slow networks via Service Worker caching strategies.

## 🧪 How to Run
1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd weather-app
   ```

2. **Serve the application:**
   Because this project uses Service Workers, it must be served over HTTPS or `localhost`. You can use a simple HTTP server like Python's `http.server` or Node's `http-server`.

   **Using Python:**
   ```bash
   python3 -m http.server
   ```

   **Using Node.js (http-server):**
   ```bash
   npx http-server .
   ```

3. **Open in Browser:**
   Navigate to `http://localhost:8000` (or the port shown in your terminal).

4. **(Optional) API Key:**
   The project currently uses an embedded API key in `app.js`. For production use, replace `OWM_KEY` in `app.js` with your own key from [OpenWeatherMap](https://openweathermap.org/).
