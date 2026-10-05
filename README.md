# Kenya Family Safari Map: Samburu, Kalama & Masai Mara Conservancies
 
This is an interactive 3D map of a 7-day family safari through some of Kenya's best private conservancies and reserves. The trip begins in the arid north at **Samburu** and the **Kalama Conservancy**, where visitors can see the "Samburu Special Five." It ends in the **Masai Mara**, with stays in **Mara North Conservancy**, the **Talek** region and the **Mara Triangle**.
 
🗺️ **See the full itinerary and the live map:**
[Safari dla całej rodziny z Kenya Conservancy](https://safarikenia.com.pl/safari-dla-calej-rodziny-z-kenya-conservancy) on **Safari Kenia**
 
---
 
## The route
 
| Day | Destination | Accommodation / Area |
|-----|-------------|----------------------|
| Start | Arrival in Nairobi | Jomo Kenyatta International Airport |
| Day 1 | Samburu | Saruni Samburu |
| Day 2 | Kalama Conservancy | Kalama Conservancy |
| Day 3 | Exploring Samburu | Samburu National Reserve |
| Day 4 | Mara North Conservancy | Saruni Masai Mara |
| Day 5 | Talek region | Talek, Masai Mara |
| Day 6 | Mara Triangle | Mara Triangle |
| Day 7 | Return to Nairobi | Wilson Airport |
 
**Northern Kenya:** Nairobi → Samburu → Kalama Conservancy → Samburu National Reserve
**Masai Mara:** Mara North Conservancy → Talek → Mara Triangle
**Return:** Masai Mara → Wilson Airport, Nairobi
 
The interface labels are in Polish, to match the tour page the map is embedded on.
 
## Features
 
- **Two ecosystems on one map.** The route covers the semi-desert of Samburu in the north and the open savannah of the Masai Mara in the south-west, so visitors see the full scale of the trip across Kenya.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain (1.5× exaggeration) and a tilted camera. This shows the Great Rift Valley between the two regions.
- **Route drawn from the Directions API.** Each leg comes from the Mapbox Directions API and is stitched into one line. If a request fails, that leg falls back to a straight segment.
- **Glowing animated route line.** A golden "marching ants" line uses emissive strength so it stays bright over the satellite imagery.
- **Interactive itinerary panel.** A glassmorphism sidebar lists all seven days. Clicking a card flies the camera to that stop and opens its popup.
- **Custom markers.** Gold SVG pins mark each stop, with popups showing the day and the accommodation.
- **Smart framing.** The initial view adjusts its padding to the container size, so the sidebar doesn't cover the route on desktop or mobile.
- **WordPress-ready.** Styles are scoped to a single container, so the map can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Every entry gets a marker and a sidebar card. Add entries with `isWaypoint: true` to shape the route without adding a marker.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), a Polish-language site offering safari tours and travel guides for Kenya.
 
➡️ [View this family safari itinerary](https://safarikenia.com.pl/safari-dla-calej-rodziny-z-kenya-conservancy)
