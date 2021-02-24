# Mapping_Earthquakes

## Project Overview
Maps allow us to explore, understand, and make decisions about our world. In this repository we will use javascript (GeoJSON) to create interactive maps to visualize earthquake data. GeoJSON data can be found in many apps that have a map feature such as ride-sharing, navigation, and food and package delivery services. Even location services on smart phones use GeoSJON format. 

### Project Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

### Tasks
To complete this project, we use a URL for GeoJSON earthquake data from the USGS website and retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. Then add the data to a map.

## Results
Each earthquake is visually represented by a circle and color, where a higher magnitude will have a larger diameter and will be darker in color. In addition, each earthquake has a popup marker that, when clicked, shows the magnitude of the earthquake and the location of the earthquake. The map has three views:
* Street View
* Satellite View
* Dark View

<p align="center">
   <img src="https://user-images.githubusercontent.com/73972332/108937898-fc038280-7603-11eb-8b80-b18acc2f419f.png" width="720" height="313.125" />
</p>

![2021-02-23_17-03-24](https://user-images.githubusercontent.com/73972332/108937981-1c334180-7604-11eb-8ccc-5df41bf356ad.png)

The viewer can also toggle between three layers to filter the data. These layers include: 
* All Earthquakes
* Tectonic Plates
* Major Earthquakes (greater than 4.5 magnitude)

![2021-02-23_17-04-17](https://user-images.githubusercontent.com/73972332/108938037-32410200-7604-11eb-9261-1aeab795ba4d.png)

## Summary
To create the maps we used the JavaScript and the D3.js library to retrieve the coordinates and magnitudes of the earthquakes from the GeoJSON data. Calling the API's alllowed us to traverse and retrieve GeoJSON earthquake data and tectonic plate data in order to populate a map. We then used the Leaflet library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data. The viewer can toggle between different layers to view either all earthquakes, only major earthquakes (over 4.5 magnitude), and the earth's tectonic plates. 
