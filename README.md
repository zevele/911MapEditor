# NineOneOneMapEditor
## Overview
A map editor for [911Operator](http://jutsugames.com/911/).<br>
A more detailed tutorial can be found on <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2461288197">Steam</a>.<br>
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


## Tutorial
Follow the following steps to download custom maps from OpenStreetMap.org. *Please read carefully the notes section before using the tool.*

1. Open The NineOneOneMapEditor. Its main screen presents all the available maps in 911Operator.
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Capture1.PNG"></p>

2. Right click anywhere on the screen.<br>
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193314.png"></p>

3. In the popup menu click on "*Download OSM...*". The "*Download OSM Data*" dialog will open.
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193410.png"></p>

4. Now you need to get the region you wish to download from <a href="OpenStreetMap.org">OpenStreetMap.org</a><br>
In any browser navigate to OpenStreetMap.org. Find the area you wish to download (in this example I choose <a href="https://www.openstreetmap.org/#map=14/36.8581/28.2764">Marmaris</a> area).
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193628.png"></p>

5. Click on the "*Export*" button to show the export tools.
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193649.png"></p>

6. After finding the region you wish to import, right-click on the "Overpass API" (in the export tools) and copy it's link. Paste the copied link back in the "Download OSM Data" dialog and press the "OK" button
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20205746.png"></p>

7. NineOneOneMapEditor will start downloading the data and processing it.

8. After downloading is completed a list places will popup for you to choose from. This will identify the region you are downloading. Then press "OK".
In this case I chose "Marmaris" (the first choice).
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193759.png"></p>

9. NineOneOneMapEditor will continue processing the data,
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20193827.png"></p>

10. When it finishes the map editor will open.
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20194606.png"></p>

11. The map editor can be zoomed using the mouse wheel, and panned by holding the middle mouse button and dragging the view. Items in the map can be selected by left clicking them, or by holding the left mouse button and dragging a selection region. You can hold "CTRL" to add items to the previously selected items.

12. For the map to work properly in 911Operator, we need to do several things: a. make sure all roads are reachable; and b. that there is at least one police station, one hospital and one fire station.
Police stations are marked by a blue rectangles, hospitals with white rectangles and fire stations with red rectangles. 

13. You can add a POI (Point of Interest) to the map through the popup menu. You can also use the keyboard shortcuts displayed in the popup menu.
<p align="center"><img src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20203200.png"></p>

14. Next we need to make sure all roads are accessible. We do this by removing those that are not accessible from the "main" group. To do this, right-click anywhere and select the "Highlight roads by connection" menu item. This will color each road group with different colors. In the bottom right corner of the screen the number of disconnected groups will appear. 
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20194711.png"></p>
Pressing the "TAB" key or "SHIFT-TAB" will select the next or previous road group. Pressing "Z" will zoom on the selected item and Pressing "DEL" will delete it.
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20194907.png"></p>
We need to repeat this process until we have only single group. In case there are POIs on the selected roads - make sure you delete those as well.

15. Press "Ctrl-S" to save the map.
16. Now if everything was done properly, the map will appear in the game, and will load properly. 
<p align="center"><img width="90%" src="https://github.com/zevele/911MapEditor/blob/main/Guide/Screenshot%202021-04-18%20213109.png"></p>
