# azs
> Gasoline availability on stations

**English** | [Русский](./README.ru.md)

# 🗺️ Interactive Map of Gas Stations with Fuel Availability

An interactive web map of gas stations (AZS) displaying fuel availability, prices, and filtering by various parameters.

## 🚀 Demo

The page is available at:  
[https://piterkey.github.io/azs/](https://piterkey.github.io/azs/)

## ✨ Features

- **Interactive Map** — visualization of gas stations on OpenStreetMap with color-coded fuel availability
- **Address Search** — automatic coordinate detection from entered address (city, street, house number)
- **Filtering**:
  - By search radius (with progressive step)
  - By number of nearest stations
  - By fuel type (AI-92, AI-95, AI-98/100, Diesel)
  - By gas station brand
  - By fuel availability status (Available, Unavailable, Likely unavailable, etc.)
- **Sorting** — by distance, address, price, update date
- **Up-to-date Data** — loads data directly from Alfa-Bank API
- **Flexible Data Source** — ability to specify any URL with JSON data
- **Responsive Design** — correct display on mobile devices
- **Dark Theme** — comfortable viewing in any conditions

## 📦 Installation and Launch

### Local Launch

1. Download the `index.html` file using one of the following methods:
   - Click the "Download the latest version of index.html" link at the bottom of the page
   - Use the browser's "Save As" button (Ctrl+S / Cmd+S)
2. Open the downloaded file in any modern browser (Chrome, Firefox, Safari, Edge)
3. The page will automatically load data from the Alfa-Bank API

## 📥 Download the Latest Version

**The always-fresh `index.html` file can be downloaded from:**  
[⬇️ Download index.html](https://raw.githubusercontent.com/piterkey/azs/main/index.html)

Or use the direct link to the file in the repository:  
[https://github.com/piterkey/azs/blob/main/index.html](https://github.com/piterkey/azs/blob/main/index.html)

> **For local use:** download the file and open it in your browser. If a `stations.json` file is present in the same folder, the page will load data from it. (ℹ️ `stations.json` size > 20 MB)

## 🔧 Usage

### Main Controls

1. **Address** — enter an address to quickly navigate to the point
2. **Coordinates** — manual coordinate entry (latitude, longitude)
3. **Radius** — slider or numeric input with progressive step
4. **Number of Stations** — limit the number of displayed stations
5. **Fuel Type** — select the fuel type to display
6. **Brand** — filter by gas station brand
7. **Fuel Availability** — multiple status selection

### Map Controls

- **Click** on the map — set a new reference point (in "Set center point on map" mode)
- **Click** on a station marker — view station information and highlight in the table
- **Click** on a table row — highlight the station on the map and open its popup

### Data Loading

- **Refresh** — load data from the current URL
- **Load JSON** — manually upload a JSON file with data
- **Data URL** — ability to specify an alternative data source

## 📊 Data Source

The default data source is the Alfa-Bank API:  
`https://alfabank.ru/api/v1/azs-stations/public/stations`

The data includes:
- Gas station name and brand
- Address and coordinates
- Fuel availability and prices
- Last update time

## 🗺️ Technologies

- **Leaflet.js** — interactive maps library
- **OpenStreetMap** — map tiles
- **Nominatim** — geocoding (address search and reverse geocoding)
- **Vanilla JavaScript** — no additional frameworks
- **CSS Variables** — theme customization

## 📱 Responsiveness

The interface is optimized for:
- Desktop computers
- Tablets
- Mobile phones

## 🔒 Privacy

- All data is loaded directly in the browser
- Data is not stored on the server
- Coordinates and addresses are not transmitted to third parties
- Only public APIs are used (OpenStreetMap, Nominatim)

## 📄 License

This project is distributed under the **MIT** license.

### Why MIT?

- **Simplicity** — short and clear text
- **Freedom** — allows use, modification, distribution
- **Safety** — does not require open-sourcing derivative works
- **Popularity** — the most common license for web projects
- **Compatibility** — allows using the code in any projects

### MIT License Text

MIT License

Copyright (c) 2026 piterkey

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
