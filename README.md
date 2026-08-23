# 🗺️ Interactive Map of Gas Stations with Fuel Availability

[![GitHub last commit](https://img.shields.io/github/last-commit/piterkey/azs)](https://github.com/piterkey/azs/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> An interactive web map of gas stations (AZS) displaying fuel availability, prices, and filtering by various parameters. The page automatically loads data from the Alfa-Bank API and shows it on an OpenStreetMap.

**🌐 [View Demo](https://piterkey.github.io/azs/)**

**English** | [Русский](#-интерактивная-карта-азс-с-наличием-топлива)

## ✨ Features

*   **Interactive Map** — visualization of gas stations on OpenStreetMap with color-coded fuel availability.
*   **Address Search** — automatic coordinate detection from entered address (city, street, house number).
*   **Filtering**:
    *   By search radius (with progressive step).
    *   By number of nearest stations.
    *   By fuel type (AI-92, AI-95, AI-98/100, Diesel).
    *   By gas station brand.
    *   By fuel availability status (Available, Unavailable, Likely unavailable, etc.).
*   **Sorting** — by distance, address, price, or update date.
*   **Flexible Data Source** — ability to specify any URL with JSON data, load a local `stations.json` file, or use the GitHub repository as a fallback.
*   **Responsive Design** — correct display on desktops, tablets, and mobile devices.
*   **Dark Theme** — comfortable viewing in any conditions.
*   **Internationalization (i18n)** — full interface translation (Russian/English).

## 📦 Installation and Launch

### Local Launch

1.  Download the `index.html` file using one of the following methods:
    *   Click the **"Download the latest version of index.html"** link at the bottom of the page.
    *   Use the browser's **"Save As"** feature (Ctrl+S / Cmd+S).
2.  For the best experience, it's recommended to run a local web server (e.g., with Python: `python3 -m http.server 8000`). This allows the page to load the `stations.json` file if it's placed in the same folder.
3.  You can also open the downloaded file directly in any modern browser (Chrome, Firefox, Safari, Edge).
4.  The page will attempt to load data in the following order:
    1.  **Local file** (`stations.json` in the same folder).
    2.  **Alfa-Bank API** (default source).
    3.  **GitHub repository** (fallback).

### Data File

*   You can place a `stations.json` file next to `index.html`. The page will load data from it first (when running from a web server).
*   The `stations.json` file is **> 20 MB** and is automatically updated in the repository.
*   You can also use the **"Load JSON"** button to manually select any JSON file.

## 🔧 Usage

### Main Controls

1.  **Address** — enter an address to quickly navigate to the point.
2.  **Coordinates** — manual coordinate entry (latitude, longitude).
3.  **Radius** — slider or numeric input with progressive step.
4.  **Number of Stations** — limit the number of displayed stations.
5.  **Fuel Type** — select the fuel type to display.
6.  **Brand** — filter by gas station brand.
7.  **Fuel Availability** — multiple status selection.

### Map Controls

*   **Click** on the map — set a new reference point (in "Set center point on map" mode).
*   **Click** on a station marker — view station information and highlight it in the table.
*   **Click** on a table row — highlight the station on the map and open its popup.

### Data Loading

*   **Refresh** — load data from the current URL.
*   **Load JSON** — manually upload a JSON file with data.
*   **Data URL** — ability to specify an alternative data source.

## 📊 Data Source

The default data source is the Alfa-Bank API:
`https://alfabank.ru/api/v1/azs-stations/public/stations`

The data includes:
*   Gas station name and brand.
*   Address and coordinates.
*   Fuel availability and prices.
*   Last update time.

## 🗺️ Technologies

*   **Leaflet.js** — interactive maps library.
*   **OpenStreetMap** — map tiles.
*   **Nominatim** — geocoding (address search and reverse geocoding).
*   **Vanilla JavaScript** — no additional frameworks.
*   **CSS Variables** — theme customization.

## 📱 Responsiveness

The interface is optimized for:
*   Desktop computers.
*   Tablets.
*   Mobile phones.

## 🔒 Privacy

*   All data is loaded directly in the browser.
*   Data is not stored on the server.
*   Coordinates and addresses are not transmitted to third parties.
*   Only public APIs are used (OpenStreetMap, Nominatim).

## 📄 License

This project is distributed under the **MIT** license. See the [LICENSE](LICENSE) file for details.

### Why MIT?

*   **Simplicity** — short and clear text.
*   **Freedom** — allows use, modification, and distribution.
*   **Safety** — does not require open-sourcing derivative works.
*   **Popularity** — the most common license for web projects.
*   **Compatibility** — allows using the code in any projects.
