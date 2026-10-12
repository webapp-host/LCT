# Project LCT static website

A GitHub Pages-ready public information website with a responsive layout, CesiumJS 3D location viewer, video slots, FAQ, contact-form placeholder, careers content, calendar and downloads.

## Preview locally

The simplest option is to open `index.html`. For the most reliable local preview, serve the folder with a local web server, for example VS Code Live Server. The published GitHub Pages version will be served correctly over HTTPS.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload the **contents** of this folder so `index.html` is at the repository root.
3. In the repository, open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.

## Update the site

- Hero image: replace `images/hero-placeholder.svg`, or change the file path in `index.html`.
- Text and section content: edit `index.html`.
- Colors and layout: edit `css/styles.css`.
- Map coordinates, video names and calendar events: edit the arrays at the top of `js/script.js`.
- Videos: add MP4 files to `videos/` using the current names, or change the paths in `js/script.js`.
- Documents: place PDFs in `documents/`, then replace the placeholder links in `index.html`.

## 3D viewer notes

The viewer uses CesiumJS from Cesium's CDN plus OpenStreetMap raster imagery. It does not require ArcGIS or a Cesium ion token. An internet connection is required. If you later want photorealistic 3D Tiles, detailed terrain or hosted project models, configure a Cesium ion token and data source.

## Contact form note

The form is intentionally a front-end demonstration and does not transmit or store submissions. Connect it to your organization's approved form endpoint before launch.
