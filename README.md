# NineOneOneMapEditor
## Overview
A map editor for [911Operator](http://jutsugames.com/911/),
The following features are supported:
* Downloading maps from [OpenStreetMap.com](https://www.openstreetmap.org/)
  * to use this feature, either copy the link from the "Overpass API" (in the [export](https://www.openstreetmap.org/export) tab) e.g: https://overpass-api.de/api/map?bbox=28.1571,36.7500,28.4266,36.8756
  * or provide the latitude longitude bounds, e.g: 28.1571,36.7500,28.4266,36.8756
* Adding/removing POIs and Roads.
* Some validation features, such as checking road connectivity and existance of essential POIs
* Converting map names from logical order to visual order (to support RTL languages).

## Some remarks
OSM map rendering is somewhat buggy (especailly with the nasty coastlines).<br>
This is very much work in progress - so expect many bugs.<br>

## Download
<a id="raw-url" href="https://github.com/zevele/911MapEditor/releases/download/20221028/NineOneOneMapViewer.exe">NineOneOneMapViewer.exe</a>
