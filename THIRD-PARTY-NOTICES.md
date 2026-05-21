# Third-Party Notices

This project uses third-party open-source libraries and external map tile providers.

The app processes GPS files locally in the browser. These notices apply to the JavaScript libraries and map/background services used by the app, not to the user's uploaded GPS files.

## JavaScript libraries

### Leaflet

Website: https://leafletjs.com/  
Repository: https://github.com/Leaflet/Leaflet  
License: BSD 2-Clause License

Leaflet is used for the interactive map display.

Leaflet 1.9.4 is listed with a BSD-2-Clause license, and its published license text identifies the BSD 2-Clause License.  
Sources: Leaflet package/license information and license text.  

### Leaflet.heat

Repository: https://github.com/Leaflet/Leaflet.heat  
License: see the Leaflet.heat repository license

Leaflet.heat is used for rendering the heatmap layer on top of the Leaflet map.

### fit-file-parser

Package: https://www.jsdelivr.com/package/npm/fit-file-parser  
License: MIT

fit-file-parser is used to parse `.fit` and `.fit.gz` files in the browser.

The project currently loads version `3.0.0` dynamically from an ES module CDN when the first FIT file is imported.

## Map tile providers

This project uses external map tile providers by default. Map tiles are not part of this project's MIT license. Each provider's own terms, attribution requirements, usage policies and availability apply.

### OpenStreetMap Standard tiles

Used for the light map style.

Attribution shown in the map:
`© OpenStreetMap contributors`

OpenStreetMap public tile servers have usage policies and capacity limits. For heavy public use, use an appropriate tile provider or host your own tiles.

### CARTO Dark Matter

Used for the dark map style.

Attribution shown in the map:
`© OpenStreetMap contributors © CARTO`

CARTO requires visible attribution for CARTO basemap styles.

### Esri World Imagery

Used for the satellite map style.

Attribution shown in the map:
`Tiles © Esri — Source: Esri, Maxar, Earthstar Geographics, and the GIS User Community`

Esri map services and imagery are subject to Esri's own terms and attribution requirements.

## Notes

- This project does not claim ownership of third-party libraries or map tiles.
- Third-party libraries and map providers may change their licenses, terms or availability.
- For production or high-traffic public deployments, review each provider's current terms directly.
- For a more self-contained/offline version, bundle the JavaScript libraries locally and use offline/self-hosted map tiles.
