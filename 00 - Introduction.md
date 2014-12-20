# Coding Maps with Leaflet
## Introduction
### What is a Web Map?
A web map lives on the World Wide Web. This means you can embed it/serve it as an HTML page.

A web map is made up of many small, square images called tiles. The tiles are usually 256 x 256 pixels in size, and are placed side-by-side to create the illusion of a large, seamless image.

Every time you zoom in, each zoom level has its own set of tiles.

Zoom Level 0: 1 tile of the whole world. The with each zoom level, the number of tiles increases exponentially; Zoom Level 1: 4 tiles, Zoom Level 2: 16 tiles, Zoom Level 3: 64 tiles, etc.

Map tiles are just individual images on the web, so you can link to them individually.

Web maps allow you to zoom in and out at different levels, display tool tips, and pan across an entire map. This is made possible with JavaScript.

It helps if you are familiar with JavaScript, but there are many different mapping libraries available that can make this much easier. Today we’re going to use one such mapping library - Leaflet - to build a web map using OpenStreetMap.

This exercise is very similar to the [Leaflet Quick Start Guide](http://leafletjs.com/examples/quick-start.html) (and a fair amount of it is taken from there). It’s also similar to the [Mozilla Thimble tutorial](http://leafletjs.com/examples/quick-start.html).

### Feature Layers
Feature layers are map tiles that live on top of your base tiles. They’re mostly used to introduce interactive elements on a map (like a pop-up).

Feature layers are often vectors layers (shapes), like polygons, a line, or a point on a map.
