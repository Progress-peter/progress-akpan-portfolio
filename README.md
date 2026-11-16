# Progress Peter Akpan · GIS & Remote Sensing Portfolio

Source of my portfolio website: **[progress-akpan-portfolio.vercel.app](https://progress-akpan-portfolio.vercel.app)**

A static site (plain HTML, CSS and JavaScript, no build step) presenting my GIS and remote sensing projects on Nigeria, each with a full case study, and my publications.

## Contents

| Path | Page |
|---|---|
| `index.html` | Home: projects, about, skills |
| `publications/` | Peer-reviewed publications with APA/BibTeX citations and schema.org metadata |
| `projects/urban-heat-island-lagos/` | Lagos Urban Heat Island, 2019–2029: case study, `map/` Leaflet web map, `code/` notebook and scripts |
| `projects/lagos-in-layers/` | Lagos in Layers: case study (embeds the 3D map) |
| `projects/lagos-filling-station-compliance/` | Filling station siting compliance: case study and `map/` Leaflet web map |
| `projects/eudr-palm-oil-traceability/` | Palm oil EUDR traceability: case study and `map/` Leaflet web map |
| `assets/` | Shared stylesheet and card images |

Each project also has its own repository with the full README and code:
[urban-heat-island-lagos](https://github.com/Progress-peter/urban-heat-island-lagos) ·
[lagos-in-layers](https://github.com/Progress-peter/lagos-in-layers) ·
[lagos-filling-station-compliance](https://github.com/Progress-peter/lagos-filling-station-compliance) ·
[eudr-palm-oil-traceability-dashboard](https://github.com/Progress-peter/eudr-palm-oil-traceability-dashboard)

## Run locally

```bash
python -m http.server 8000
# open http://localhost:8000
```

Pages use root-relative links (`/assets/style.css`), so serve from the repository root.

## Deploy

Hosted on Vercel as a static site (`vercel.json` sets `trailingSlash: true`):

```bash
npx vercel deploy --prod
```

## Credits

Basemaps: Esri (World Light Gray Canvas and reference labels). Leaflet 1.9.4 (BSD-2-Clause) and Chart.js 4.4.1 (MIT) are vendored under `projects/urban-heat-island-lagos/map/vendor/`. Map data sources are credited on each project page.

© 2026 Progress Peter Akpan
