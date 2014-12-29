# Coding Maps with Leaflet
## Adding a Map Marker
To place a map marker, you’ll need the latitude and longitude of the exact location. The lat/lon for Vancouver Public Library’s Central Branch is `[49.27970, -123.11549]`. Let’s place our marker here. 

Add this code inside the `<script>` tag: 

    var marker = L.marker([49.27970, -123.11549]).addTo(map);

(add some information here about how to get the lat/lon from OSM)

Reload your HTML page in the browser, and you should see a blue pin on top of Vancouver Public Library. The pin won’t do anything if you click on it, so our next step is to create a popup (or tool tip) that shows some information about the library. The ability to add these popups is built into Leaflet, so creating them will be easy. 

Add this between the `<script>` tags, just after the marker variable: 

    marker.bindPopup("Vancouver Public Library is the third-largest library system in Canada.");

Save your page, reload it in the browser, and click the marker. Your map should now look like this: 

![Map of Vancouver BC](images/MAP01.png)
