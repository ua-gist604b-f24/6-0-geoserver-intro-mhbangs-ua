Q1: What is the URL of the WMS GetCapabilities request?
- https://solid-garbanzo-4jw6wgggjjq7h7x6p-8080.app.github.dev/geoserver/ows?service=WMS&version=1.3.0&request=GetCapabilities

Q2: What is the URL of the WFS GetCapabilities request?

- https://solid-garbanzo-4jw6wgggjjq7h7x6p-8080.app.github.dev/geoserver/ows?service=WFS&acceptversions=2.0.0&request=GetCapabilities


Q3: Submit a screenshot of your updated WFS Layer Preview
<img width="659" alt="WFS Layer Preview" src="https://github.com/user-attachments/assets/d0e31e7d-df26-439e-850c-275053d4bf4c">

Q4: What does drawing order refer to? Which layer goes on top, the first or the last layer in the list?
- This drawing order is the order in which the layers are displayed. The layer that goes on top is layer 1 or the first layer in the list.

Q5: Submit a screenshot of the Layer Preview of the Spearfish Layer Group when sf:sfdem is listed as the 3rd layer.
<img width="1406" alt="screenshot-dem3rd" src="https://github.com/user-attachments/assets/387abef5-cff0-4ee7-8c2d-6f058e5d7a04">

Q6: What is the WMS url for the single-tiled request?
- Single Tile
https://solid-garbanzo-4jw6wgggjjq7h7x6p-8080.app.github.dev/geoserver/wms?SERVICE=WMS&VERSION=1.1.1&REQUEST=GetMap&FORMAT=image%2Fpng&TRANSPARENT=true&STYLES&LAYERS=spearfish&exceptions=application%2Fvnd.ogc.se_inimage&SRS=EPSG%3A26713&WIDTH=1900&HEIGHT=1000&BBOX=589816.6262606113%2C4918085.506452528%2C607946.9169117232%2C4927626.257750212

Q7: What is the WMS url for one of the tiled requests? What is the image size?
- Tiled Image Size 256/256? 
https://solid-garbanzo-4jw6wgggjjq7h7x6p-8080.app.github.dev/geoserver/wms?SERVICE=WMS&VERSION=1.1.1&REQUEST=GetMap&FORMAT=image%2Fpng&TRANSPARENT=true&tiled=true&STYLES&LAYERS=spearfish&exceptions=application%2Fvnd.ogc.se_inimage&tilesOrigin=589425.9342365642%2C4913959.224611808&WIDTH=256&HEIGHT=256&SRS=EPSG%3A26713&BBOX=602260.3237318471%2C4923142.200079817%2C603481.9471065567%2C4924363.823454527

Q8: What is the URL of your coarse resolution sample of a WMTS url? 
https://solid-garbanzo-4jw6wgggjjq7h7x6p-8080.app.github.dev/geoserver/gwc/service/wmts?layer=spearfish&style=&tilematrixset=EPSG%3A4326&Service=WMTS&Request=GetTile&Version=1.0.0&Format=image%2Fpng&TileMatrix=EPSG%3A4326%3A11&TileCol=867&TileRow=518

What level does this tile refer to? I think this url points to the service as a whole instead of a single tile. It is also an image of the service/

What are some of the fields that are unique to this url? This url appears to be a png instead of bound by a bbox. It has something about a TileMatrix, maybe that is how the png is constructed?

Q9: In the zoomed-out URL, what are the TileCol and TileRow?
- I might have be looking at a different service because I have multiple wmts when I zoom in and out. But for the one I am looking at it TileCol=216&TileRow=129

Q10: In the zoomed-in URL, what are the TileCol and TileRow?
- I might have be looking at a different service because I have multiple wmts when I zoom in and out. But for the one I am looking at it TileCol=6936&TileRow=4145

Q11: Why are they so different for the same location in the map?
- They are different because it is a different cache of tiles when zoomed in and zoomed out?

Q12: Is there a difference in the TileMatrix? %3A is an HTML encoding for a colon, :.What does the number after EPSG:4326 mean?
- The numbers after ESPG 4326 is the projection I believe. 
