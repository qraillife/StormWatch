# StormWatch

A clean, responsive weather dashboard for phones and desktops, built with HTML, CSS and JavaScript. No build tools, accounts or API keys required for non-commercial use.

## Features

- Current conditions, feels-like temperature, wind, humidity, UV estimate and rainfall
- 12-hour overview, 24-hour detailed hourly forecast, seven-day outlook
- City and suburb search worldwide, plus optional device location
- Recent rainfall radar imagery with a time slider and playback
- Links to official Bureau of Meteorology and Queensland emergency warning resources
- Installable progressive web app (PWA), dark design and mobile navigation
- Saves your chosen location locally in your browser

## Publish to GitHub Pages

1. Create a public GitHub repository called `StormWatch` (or any name you like).
2. Choose **Add file → Upload files** in the repository.
3. Upload **all files and folders in this package** to the **root** of the repository: `index.html`, `style.css`, `app.js`, `sw.js`, `manifest.webmanifest`, `README.md`, and the `assets` folder.
4. Commit the files.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, select **Deploy from a branch**, choose **main** and **/(root)**, then save.
7. After GitHub finishes publishing, open `https://YOUR-USERNAME.github.io/StormWatch/` (replace username and repository name as appropriate).

### Installing on iPhone

Open your published site in **Safari**, tap **Share → Add to Home Screen → Add**.

### Installing on desktop

Open the website in Chrome or Edge and use the browser's **Install app** action when available.

## Data and limitations

- Forecasts: [Open-Meteo](https://open-meteo.com/), used with attribution. The public, keyless API is for **non-commercial use** subject to provider terms and limits. Model forecasts are not official BOM observations.
- Rain imagery: [RainViewer](https://www.rainviewer.com/api.html), historical frames only. Its free API is for personal/educational and small-scale community use, limited in 2026 to **past imagery**, with maximum native zoom 7 and rate limits. Radar coverage and availability vary.
- Base maps: [OpenStreetMap](https://www.openstreetmap.org/copyright) via [CARTO](https://carto.com/attributions). [Leaflet](https://leafletjs.com/) displays the maps. Their stylesheet and script are loaded from a CDN, so the radar map requires internet access.
- Official warnings: StormWatch deliberately **does not claim to display or detect active BOM warnings**. The Warnings tab links directly to the government sources. **Do not use this app as an emergency alert service.**
- Geolocation uses browser permission; it is never uploaded to a StormWatch server. Weather and map service providers receive coordinates as needed to provide their services.
- The PWA can open its shell offline after the first successful visit, but fresh weather/radar information requires an internet connection.

## Files

- `index.html` — app layout and sections
- `style.css` — responsive visual design
- `app.js` — weather, search and radar functionality
- `sw.js` — offline shell cache
- `manifest.webmanifest` — installation settings
- `assets/` — app icons

StormWatch is an independent project and is not affiliated with the Australian Bureau of Meteorology.
