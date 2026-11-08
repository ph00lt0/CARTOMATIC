# CARTOMATIC


<img width="4961" height="3508" alt="cartomatic-A3-landscape-300dpi" src="https://github.com/user-attachments/assets/4c52d713-e2f0-41b3-a462-833a22a8dd9b" />


Generate and style your GeoJSON to make posters of locations.

CARTOMATIC is a browser-based map poster generator for turning GeoJSON data into stylized travel-poster layouts. Upload a GeoJSON file or paste JSON, choose a basemap, tune colors and overlays, and export a printable poster PNG sized for common paper formats.

## Features

- Upload or paste GeoJSON data
- Render points, lines, and polygons on a map
- Switch between built-in basemaps or a blank poster canvas
- Customize map styling with color controls for land, water, roads, borders, and labels
- Style markers with different symbols, colors, stroke, and optional labels
- Add line and polygon overlays with dashed/dotted styles and curved travel routes
- Adjust crop framing and paper size/orientation for poster export
- Export a poster PNG at print-ready resolution
- Includes a sample GeoJSON trip for quick testing

## Live app

The app runs as a single front-end page:

- `index.html`

## Run locally

Because this project is a static HTML app, you can open it directly in a browser:

1. Clone or download this repository.
2. Open `index.html` in your browser, or serve the folder locally:

```bash
cd CARTOMATIC
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000/
```

## Usage

1. Open the app in a browser.
2. Load GeoJSON via file upload or paste raw JSON.
3. Choose a basemap and adjust layer colors to match your poster aesthetic.
4. Configure marker styles, overlay appearance, and optional vintage effects.
5. Set the paper size, orientation, margin, and title.
6. Use the crop frame to define the print area if needed.
7. Click `Print poster PNG` to export the final image.

## GeoJSON notes

The app expects standard GeoJSON objects such as:

- `FeatureCollection`
- `Feature`
- `Point`
- `LineString`
- `Polygon`
- `MultiPoint`, `MultiLineString`, `MultiPolygon`

Point features become markers, while line and polygon features can be rendered as overlay layers.

## Built with

- HTML
- CSS
- JavaScript
- MapLibre GL JS
- OpenFreeMap vector tiles

## Project structure

```text
CARTOMATIC/
├── index.html
├── .github/
└── README.md
```

## Notes

- There is no build step required.
- The app is designed for browser-based poster generation and export.
- Map tiles come from OpenFreeMap and are rendered with MapLibre GL.

