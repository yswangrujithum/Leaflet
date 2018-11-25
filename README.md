# Geography of Earthquake and the Plate Tectonics
![Earth](Images/earth.jpeg)
This project is focusing on creating a map using Mapbox and Leaflet that will illustrate the location of the earthquake and the plate tectonics. 
## Getting Started
### The following program is required for your local machine 
* D3.js
### The following programs are available for download
* Mapbox (API required)
* Leaflet
### Available Resources
* Earthquake Data 

``` https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson```

* Plate Tectonic Data

```https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json``` 

## Project Breakdown
* Create the HTML webpage for map visualization 
* Create the Javascript workspace
* Create the CSS workspace
### Within the JS Workspace
* use D3 to call for the Data within the provided URLs 

```d3.json(URL, function(data){```

* convert the point feature to the map layer by using Leaflet feature, pointToLayer

```pointToLayer: function(feature, coord){```

* For each data points, create the popup feature to indicate the information about the point

```layer.bindPopup``` 

* Add data to the variable that combine multiple data layers to a single group 

```.addTo(allData);```
``` dataMap(allData); ```

* Create the function, Color that will return specific color depending on the magnitude of the earthquake

```if (magnitude > 5){return 'red'```

* Add the function, dataMap to the map itself. 

```var satellite = L.tileLayer('https://api.tiles.mapbox.com/v4/{id}/{z}/{x}/{y}.png?access_token={accessToken}', {```

* Add the baseMap and overlayMap to the visualization 

## Author
Yanin Swangrujithum 

