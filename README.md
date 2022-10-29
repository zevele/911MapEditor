# NineOneOneMapEditor
This is an empty public repository to share the editor binaries and information about it.
## Overview
A map editor for [911Operator](http://jutsugames.com/911/).<br>
A more detailed tutorial can be found on <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2461288197">Steam</a> or <a href="https://github.com/zevele/911MapEditor/blob/main/Guide/Tutorial.md">here</a><br>
The following features are supported:
* Downloading maps from [OpenStreetMap.com](https://www.openstreetmap.org/)
  * to use this feature, either copy the link from the "Overpass API" (in the [export](https://www.openstreetmap.org/export) tab) e.g: https://overpass-api.de/api/map?bbox=28.1571,36.7500,28.4266,36.8756
  * or provide the latitude longitude bounds, e.g: 28.1571,36.7500,28.4266,36.8756
* Adding/removing POIs
* Removing roads
* Connecting two exiting roads
* Renaming POIs and roads names
* Some validation tools, such as checking road connectivity and existance of essential POIs
* Converting map names from logical order to visual order (to support RTL languages)
* Add the name of the local region (e.g. town or city) before the street name
* Show a list of all POIs in the map

## Some remarks
OSM map rendering is somewhat buggy (especailly with the nasty coastlines).<br>
This is very much work in progress - so expect many bugs.<br>

## Download
<a id="raw-url" href="https://github.com/zevele/911MapEditor/releases/download/20221028/NineOneOneMapViewer.exe">NineOneOneMapViewer.exe</a>


