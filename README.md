# Mapping_Earthquakes

## Project Overview
Maps allow us to explore, understand, and make decisions about our world. In this repository we will use javascript (GeoJSON) to create interactive maps to visualize earthquake data. GeoJSON data can be found in many apps that have a map feature such as ride-sharing, navigation, and food and package delivery services. Even location services on smart phones use GeoSJON format. We can explore points (ie addresses and locations), linestrings (ie boundaries for streets and travel routes), and polygons (ie boundaries zip codes and counties) as well as non-spatial attributes (ie earthquake magnitude).  

### Project Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

### Tasks
To complete this project, we use a URL for GeoJSON earthquake data from the USGS website and retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. Then add the data to a map.

### Approach
Use the JavaScript and the D3.js library to retrieve the coordinates and magnitudes of the earthquakes from the GeoJSON data. Calling the API's will alllow us to traverse and retrieve GeoJSON earthquake data and tectonic plate data in order to populate a map. Use the Leaflet library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data.

## Results
Each earthquake is visually represented by a circle and color, where a higher magnitude will have a larger diameter and will be darker in color. In addition, each earthquake has a popup marker that, when clicked, shows the magnitude of the earthquake and the location of the earthquake.
## Summary
