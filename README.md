# Heat My Tracks

Privacy-first local GPS heatmap viewer for GPX, GPX.GZ, FIT and FIT.GZ files.

Heat My Tracks lets you load GPS activity files directly in your browser and generate an interactive heatmap. Your GPS files are processed locally and are not uploaded by the app.

## Important

This is a browser-only app. It does not connect to your Strava (or any other) account and it does not upload your files.

## Features

- Load `.gpx`, `.gpx.gz`, `.fit` and `.fit.gz` files
- Drag-and-drop or file picker import
- Local browser-side processing
- Interactive heatmap
- Optional route display
- Date range filtering
- Day / week / month / year presets
- Timeline playback animation
- Dark, light and satellite map backgrounds
- Heatmap opacity, spread and sensitivity controls

## How to use

1. Open `index.html` in a modern browser.
2. Drag your GPS files into the upload panel, or click **Choose GPS files**.
3. Wait for the import to finish.
4. Use the date range controls at the top to filter your activities.
5. Adjust the heatmap settings in the right panel.
6. Use **Presets** and **Play** to animate through your activity history.

## Supported files

The app supports:

- `.gpx`
- `.gpx.gz`
- `.fit`
- `.fit.gz`

Files ending in `.gz` are decompressed locally in the browser.

## Privacy

Your GPS activity files are not uploaded by this app.

All file parsing and heatmap processing happens locally in your browser.

However, the default version loads some external resources:

- map tiles
- Leaflet
- Leaflet.heat
- FIT parser module

Map tile providers may receive normal map tile requests for the area you view.

## Strava export

You can use files from a Strava bulk export.

Strava exports may contain a mix of `.gpx.gz` and `.fit.gz` files. Both are supported.

## Performance tips

For large imports, keep **Precompute on import** enabled.

This makes importing a bit slower, but makes filtering, playback and heatmap updates much faster afterwards.

For thousands of activities:

- keep **Show routes** disabled unless needed
- keep **Auto-zoom** disabled during playback
- use heatmap mode for best performance

## Map styles

Available map styles:

- Dark — CARTO Dark Matter / OpenStreetMap
- Light — OpenStreetMap Standard
- Satellite — Esri World Imagery

These map providers have their own usage policies and attribution requirements.

## License

This project is licensed under the MIT License.

Third-party libraries and map tile providers have their own licenses and terms.
