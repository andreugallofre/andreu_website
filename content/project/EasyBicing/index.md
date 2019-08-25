---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "EasyBicing"
summary: |
  Web application with node.js, Html and CSS to solve the problems that bicing users usually have
authors: [ Bernat Torres, Victor Sanchez, Andreu Gallofre ]
tags: [ code, website, noode.js ]
categories: [ source ]
date: 2018-11-11T11:23:56+02:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
image:
 caption: ""
 focal_point: ""
 preview_only: false

# Links
url_code: "https://github.com/atsuky/EasyBicing"
url_pdf: ""
url_slides: ""
url_video: ""
links:
- name: GitHub
  url: https://github.com/atsuky/EasyBicing
  icon_pack: fab
  icon: github

# Slides (optional).
slides: ""
---

# EasyBicing

We made a responsive web application with node.js, Html and CSS to solve the problems that bicing users usually have, for that we implemented real-time and history functionality.

## Why we did it

As we told, we based on the main problems that our friends are having when they use bicing, we asked them and their main problems where things like "I have to be pending of the application if i want to know if the station near my home is full ore it has bikes" or "If i go to a place, i don't know if where i want to park my bike has empty slots" so we build a solution for them.

## Main Funcionalities

#### Real Time

* __Find Bike__: Show you a path to the nearest bicing station with bikes
* __Park Bike__: You can chose between two options
  * Near Station: Shows you the path to the nearest bike station with spots to park the bike
  * Search: You can manually search the station that you want to go even if that station is full
  
* __Find Route__: It's a search engine to search a route to the location that you want

The map will show you all the stations of bicing with the actual ocupation showed by color:
  
  * *Green*: More than 50% of bikes of the station are available
  * *Orange to red*: There is at least 1 bike, and it's a gradient, from 49% to 1%
  * *Black*: There is no bikes available
  
  (The inverse if you are looking for parking your bike)
  
 If you click any point in the map, a pop-up will appear with the basic information of that bike station, you will have the available bikes that it has, the number of the slots, and the address of that specific station, also, a "Go" button will appear and if you click on it, the system will generate a route from your location, based on the device position and the station that you selected.
 
 Also we have implemented an alarm system that allows the user to set alarms to know if one station have at least 1 bike, lots of bikes or the station is empty.
 
##### Data Analysis

  Mobility:Lab provided us a dataset with the information of the bicing usage for the last year, we had like 120K rows for each day. We parsed all of the available data, and we made two heat maps of the usage of bicing based on day of the year and time of the day, the main use of this could be help the user to predict the best time for him to do his trips, and his best stations based on time and what they need.
  
# Technologies used

  For the realtime application we used node.js, html, and we used leaflet and graphopper for the map and routes visualization, all of the apis used are based on openmaps and are licensed as open source.
  
  For the data analytics and visualization, we used the dataset of Mobility:Lab and some shell comands like awk to parse it into something that we actually can use, and then used CARTO for the visualization.

# Deploy

``` npm install ```
``` node server.js ```