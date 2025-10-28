# Earthquake-Visualizer

A single-file, zero-build web app that shows every earthquake recorded by USGS in the past 24 h.

## Features
- Interactive world map (pan, zoom, wheel-zoom)
- Markers sized by magnitude (color coded via default Leaflet icon)
- Popup with magnitude, location, timestamp
- Auto-fits map to show all events
- Graceful error + loading states
- Responsive (works on phone, tablet, desktop)

## Tech choices
- React 18 (UMD, no build)
- react-leaflet 4.x (UMD)
- Tailwind via CDN for quick styling
- USGS GeoJSON endpoint (no key required)

## Run locally
1. Clone repo
2. Serve folder with any static server  
   `npx serve .`  or  `python -m http.server 3000`
3. Open http://localhost:3000

## Deploy
Push to GitHub → import repo in CodeSandbox or StackBlitz → automatic deploy.

## Extending
- Replace markers with CircleMarker radius = magnitude * 3  
- Add layer control to toggle “Past hour”, “Past week” feeds  
- Color markers by depth instead of magnitude  
- Add sidebar list that scrolls to marker on click

## License
MIT
