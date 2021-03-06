# Mapping_Earthquakes

## Project Overview
Maps allow us to explore, understand, and make decisions about our world. In this repository we will use javascript (GeoJSON) to create interactive maps to visualize earthquake data. GeoJSON data can be found in many apps that have a map feature such as ride-sharing, navigation, and food and package delivery services. Even location services on smart phones use [GeoSJON format](https://geojson.org/). 

### Project Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

### Tasks
To complete this project, we use a URL for GeoJSON earthquake data from the [USGS website](https://www.usgs.gov/natural-hazards/earthquake-hazards/earthquakes) and retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. Then add the data to a map.

## Results
### The map visualization can be viewed and interacted with in its entirity [here](https://angienoelhaverly.github.io/MajorEarthquakes/).

Each earthquake is visually represented by a circle and color, where a higher magnitude will have a larger diameter and will be darker in color. In addition, each earthquake has a popup marker that, when clicked, shows the magnitude of the earthquake and the location of the earthquake. The map has three views:
* Street View
* Satellite View
* Dark View

<p>
   <img src="https://user-images.githubusercontent.com/73972332/108937898-fc038280-7603-11eb-8b80-b18acc2f419f.png" width="925" height="512" />
</p>
<p>
   <img src="https://user-images.githubusercontent.com/73972332/108937981-1c334180-7604-11eb-8ccc-5df41bf356ad.png" width="925" height="512" />
</p>

The viewer can also toggle between three layers to filter the data. These layers include: 
* All Earthquakes
* Tectonic Plates
* Major Earthquakes (greater than 4.5 magnitude)
<p>
   <img src="https://user-images.githubusercontent.com/73972332/108938037-32410200-7604-11eb-9261-1aeab795ba4d.png" width="925" height="512" />
</p>

## Summary
To create the maps we used the JavaScript and the D3.js library to retrieve the coordinates and magnitudes of the earthquakes from the [GeoJSON data](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson). 

Calling the API's alllowed us to traverse and retrieve [GeoJSON earthquake data](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) and [tectonic plate data](https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json) in order to populate a map. We then used the [Leaflet library](https://leafletjs.com/index.html) to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data. The viewer can toggle between different layers to view either all earthquakes, only major earthquakes (over 4.5 magnitude), and the earth's tectonic plates. 

By viewing this visualization, it's clear that the majority of the major earthquakes in the last week have all occurred near or on the tectonic plates. Smaller earthquakes can occur farther away, but the major earthquakes all fall on or right next to the fault lines. 
