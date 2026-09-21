# Pest Warning Dashboard

Funder demonstration portal for **SMARTRAPS-2.0** (MNSUAM / PARB): South Punjab fruit-fly GIS map + multi-crop pest knowledge infographics.

## Run on localhost

```bash
cd pest-warning-dashboard
python3 -m http.server 8080
```

Open http://127.0.0.1:8080

- `/` — portal home  
- `/map/` — fruit-fly density map (needs HTTP server for GeoJSON)  
- `/crops/` — mango / cotton / wheat / maize pest charts  

## Data notes

- District polygons: geoBoundaries PAK ADM2 (subset in `map/data/south_punjab_districts.geojson`)
- Trap densities and crop pressure scores are **demo / illustrative**
- Project KPIs (US$200M losses, 92.9% mAP, Rs 49.42 M) follow the PARB concept clearance proforma

## Stack

Static HTML + Leaflet + Chart.js (CDN). No build step.
