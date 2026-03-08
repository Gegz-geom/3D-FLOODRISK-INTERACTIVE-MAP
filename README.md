# Makkah Flood Risk — Interactive 3D Web Map

A fully interactive 3D flood risk visualization for Makkah Al-Mukarramah, converting a multi-criteria GIS analysis into a deployable web map built with Mapbox GL JS.

https://3-d-floodrisk-interactive-map.vercel.app/



---

## Features

- **Real flood risk data** — zones derived from actual GIS output (SRTM DEM + LULC + Precipitation weighted overlay)
- **3D terrain** — live SRTM elevation with adjustable exaggeration
- **3D buildings** — extruded at zoom 13+
- **Risk zone filtering** — click any legend class to isolate it on the map
- **Cinematic flythrough** — automated 6-waypoint tour of the study area
- **Basemap switching** — Satellite, Dark, Light
- **Responsive** — full desktop sidebar + mobile full-screen control panel
- **Fly-to presets** — Overview and Al Haram Mosque

---

## Data & Methodology

| Parameter | Details |
|---|---|
| Elevation | SRTM 30m DEM |
| Precipitation | Resampled high-resolution |
| Land Use | 7-class LULC |
| Method | Weighted Overlay MCA |
| Study Area | ~1,400 km² |
| CRS | WGS 84 |

**Risk Classification**

| Class | Coverage |
|---|---|
| Very High | 3% |
| High | 15% |
| Moderate | 29% |
| Low | 35% |
| Very Low | 18% |

---

## Tech Stack

- [Mapbox GL JS v3.3.0](https://docs.mapbox.com/mapbox-gl-js/)
- Vanilla HTML / CSS / JavaScript
- Single-file deployment — no build tools or dependencies

---

## Project Structure

```
├── index.html       # Full application — map, UI, and embedded GIS data
├── README.md        
└── assets/
    └── preview.png  # Repository preview image
```

---

## Author

**Hassan Gegu** — GIS & Web Mapping Developer  
[GitHub](https://github.com/gegz-geom)
