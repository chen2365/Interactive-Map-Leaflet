# Developing Data Product: Week 2 Assignment
June 18, 2017  



## Instructions
Create a web page using R Markdown that features a map created with Leaflet.

Host your webpage on either GitHub Pages, RPubs, or NeoCities.

Your webpage must contain the date that you created the document, and it must contain a map created with Leaflet. We would love to see you show off your creativity!


## Interactive Map Leaflet

Some New York points of interest: Empire State Building, New York University, One World Trade Center, Metropolitan Museum of Art


```r
library(leaflet)
mapNYC = leaflet() %>%
 addTiles() %>%
 addMarkers (lat= 40.7484404, lng= -73.9856554, popup="Empire State Building")%>%
 addMarkers (lat= 40.7291475, lng = -73.9959781, popup="New York University")%>%
 addMarkers (lat= 40.7129947, lng = -74.0131609, popup="One World Trade Center")%>%
 addMarkers (lat= 40.7794366, lng= -73.963244, popup="Metropolitan Museum of Art")

mapNYC
```

<!--html_preserve--><div id="htmlwidget-72d334d09da52dea2eb9" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-72d334d09da52dea2eb9">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"maxNativeZoom":null,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"continuousWorld":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":null,"unloadInvisibleTiles":null,"updateWhenIdle":null,"detectRetina":false,"reuseTiles":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[40.7484404,-73.9856554,null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"Empire State Building",null,null,null,null,null,null]},{"method":"addMarkers","args":[40.7291475,-73.9959781,null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"New York University",null,null,null,null,null,null]},{"method":"addMarkers","args":[40.7129947,-74.0131609,null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"One World Trade Center",null,null,null,null,null,null]},{"method":"addMarkers","args":[40.7794366,-73.963244,null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"Metropolitan Museum of Art",null,null,null,null,null,null]}],"limits":{"lat":[40.7129947,40.7794366],"lng":[-74.0131609,-73.963244]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
