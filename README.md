# Migration Atlas

**Live Demo:** [garridolecca.github.io/migration-atlas](https://garridolecca.github.io/migration-atlas/)

Interactive 3D globe visualization of global refugee and displacement flows, built with ArcGIS JavaScript API.

![Migration Atlas](https://img.shields.io/badge/ArcGIS_JS_API-4.31-blue) ![Data](https://img.shields.io/badge/Data-UNHCR_2024-red) ![License](https://img.shields.io/badge/License-MIT-green)

## Overview

Migration Atlas visualizes the movement of **123.2 million** forcibly displaced people worldwide using an interactive 3D globe with animated flow particles. Data is sourced from the [UNHCR Global Trends 2024](https://www.unhcr.org/global-trends) report.

### Key Statistics (End of 2024)
| Metric | Count |
|--------|-------|
| Total Displaced | 123.2M |
| Refugees | 42.7M |
| Internally Displaced (IDPs) | 73.5M |
| Asylum Seekers | 8.4M |

## Features

- **3D Interactive Globe** - ArcGIS SceneView with dark basemap, stars, and atmospheric effects
- **Animated Flow Particles** - Moving dots travel along migration arcs from origin to destination, with color morphing (red to white to cyan) and size pulsing
- **Gradient Migration Arcs** - 46+ routes with red-to-cyan color interpolation and elevation curves proportional to geographic distance
- **Country Dot Markers** - Red for outflow origins, cyan for asylum destinations, orange for countries that are both
- **HUD-Style UI** - Futuristic heads-up display panels with Michroma font, corner brackets, scanlines, and blinking indicators
- **Country Filter** - Click any country dot or use the search bar to zoom in and filter migration flows
- **Crisis Profiles** - Detailed information for 8 major crises including trend charts and destination breakdowns
- **KPI Dashboard** - Real-time stats panel with outflow/inflow bar charts
- **Auto-Rotation** - Globe slowly rotates, pausing on user interaction
- **Responsive Design** - Adapts to mobile and tablet screens

## Crises Covered

| Country | Displaced | Type |
|---------|-----------|------|
| Sudan | 14.3M | Largest crisis (2023 war) |
| Syria | 13.5M | Civil war since 2011 |
| Ukraine | 10.0M | Russian invasion 2022 |
| Afghanistan | 8.9M | Decades of conflict |
| DR Congo | 7.3M | M23 offensive, eastern conflict |
| Venezuela | 5.1M | Economic/political collapse |
| Somalia | 4.5M | Conflict + climate |
| Myanmar | 3.5M | Rohingya + military coup |

## Top Refugee Hosting Countries

| Country | Refugees Hosted |
|---------|----------------|
| Iran | 3.8M |
| Turkey | 2.9M |
| Germany | 2.8M |
| Colombia | 1.8M |
| Uganda | 1.8M |
| Pakistan | 1.6M |
| Poland | 1.6M |

## Tech Stack

- **[ArcGIS JavaScript API 4.31](https://developers.arcgis.com/javascript/)** - 3D SceneView, GraphicsLayer, geometry
- **Single HTML file** - No build tools, no dependencies beyond CDN
- **Michroma Font** (Google Fonts) - Futuristic HUD typography
- **Vanilla JavaScript** - No frameworks

## Data Sources

- [UNHCR Global Trends Report 2024](https://www.unhcr.org/global-trends-report-2024) (end of 2024 data)
- [UNHCR Mid-Year Trends 2025](https://www.unhcr.org/us/publications/mid-year-trends)
- [UNHCR Refugee Data Finder](https://www.unhcr.org/refugee-statistics)
- [Frontex Migratory Routes](https://www.frontex.europa.eu/what-we-do/monitoring-and-risk-analysis/migratory-routes/)

## Usage

Simply open `index.html` in a browser. No server or build step required.

```bash
# Clone and open
git clone https://github.com/garridolecca/migration-atlas.git
cd migration-atlas
open index.html
```

## Inspired By

[Migration Track](https://migrationtrack.netlify.app/) by Seoyeon Jun - a Three.js-based migration visualization.

## License

MIT
