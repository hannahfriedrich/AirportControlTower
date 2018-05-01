# Airport Control Tower
Made by Hannah Friedrich

## Introduction
This is an interactive map that displays airport density by state and airports that have and do not have airport control
towers - symbolized differently by the color of the telegram icon. By hovering over a state, the information panel in the top right corner
of the map updates with the state and the number of airports in that state. If you click on a state, the map will be zoom
to that state.

## Projection
I decided to use the USA Contiguous Albers Equal Area Conic projection (EPSG:102003) because the United States is predominately
oriented East-West as opposed to North-South and conic projections handle "wide" geogrpahic spans well. While conic projections do not
retain shape or scale exactly, distortion is minimized  between standard parallels.

## Major Functions

There is a variety of functions that are used to allow dynamic user interaction with the webmap.

### Dynamic Label
Supported by the Label Gun library, this function allows the state labels to be displayed based on how cluttered the screen
is with other labels.

### Highlight Feature
Highlight a feature when the mouse hovers on it.

### Reset Highlight
Reset the hightlighted feature when the mouse is out of its region.

### Zoom-To Feature
Zoom to the highlighted feature when the mouse is clicking onto it.

## Libraries
The underlying web map support is from <a href="http://leafletjs.com/">Leaflet</a> js library.

For making dynamic labels, the <a href="https://github.com/Geovation/labelgun">Label Gun</a> and
<a href="https://github.com/mourner/rbush">Rbush</a> js libraries are used.

For creating the graticule, the <a href="https://github.com/cloudybay/leaflet.latlng-graticule">leaflet.latlng-graticule</a>
library is used.

For projecting the map, the <a href="https://github.com/proj4js/proj4js">proj4js</a> and
<a href="https://github.com/kartena/Proj4Leaflet">proj4leaflet</a> js libraries are used.

For adding color to the map, the <a href="https://github.com/gka/chroma.js/">chroma</a> js library is used.

For selecting html elements, the <a href="http://jquery.com/">jQuery</a> js library is used.

## Data Sources
Airport data is from the <a href="https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile">US Government Data Catalog</a>
US States data is from <a href="https://bost.ocks.org/mike/">Mike Bostock</a>.

## Credit
Made by <a href="https://github.com/hannahfriedrich">Hannah Friedrich</a>, Masters Student in Geography, Oregon State University

## Acknowledgement
This webmap was created for <a href="https://github.com/jakobzhao/geog4572">Geovisual Analytics</a> taught by <a href="http://geoviz.ceoas.oregonstate.edu/">Bo Zhao</a>.