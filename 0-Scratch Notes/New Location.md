---
map_height_y: 5882
map_width_x: 5888
scale_pixels: 268
scale_pixels_range: 25
mapCalc1: 10.72
---

```leaflet
id: MapIslandofScreams ### Must be unique with no spaces
image: [[The Island of Screams.jpg]] ### Link to the map image file
bounds: [[0,0], [5882, 5888]] ### Size of the map in px Width_x, Height_y
height: 950px ### Size of the leaflet embed in px on your screen
width: 95% ### Size of the leaflet embed in your note
lat: 2941 ### To center the map, make this half of the map width. 
long: 2944 ### To center the map, make this half of the map height. 
minZoom: -3 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level. 
maxZoom: 0 ### Controls how far towards the map you can zoom in.  Hover over the target icon to see the current level. 
defaultZoom: -2.5 ### Sets the default zoom level when the map loads.  Hover over the target icon to see the current level. 
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out. 
unit: km ### The value displayed when measuring so you know what type of unit is being measure.
scale: 0.09328358208955223 ### Real units/px (resolution) of your map
recenter: false
darkmode: false ### marker
```

[[The Island of Screams.jpg]]


> [!NOTE]- Quick Calculator
> Map Height in Pixels: `INPUT[number:map_height_y]`
Map Width in Pixels: `INPUT[number:map_width_x]`
lat: `VIEW[{map_height_y} / 2][math]` 
long: `VIEW[{map_width_x} / 2][math]` 
How Many Pixels In Scale: `INPUT[number:scale_pixels]`
How Many Units in Scale: `INPUT[number:scale_pixels_range]`
scale: `VIEW[1/{mapCalc1}][math]`