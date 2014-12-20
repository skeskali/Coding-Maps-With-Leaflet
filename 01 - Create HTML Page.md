# Coding Maps with Leaflet
## Create Your HTML Page

Open your text editor. For this course, I’ll be using [Brackets](http://brackets.io "Brackets Text Editor"), but you can use whatever text editor you want. A couple of good, multi-platform ones are [Atom](http://atom.io "Atom text editor") and [Sublime Text](http://sublimetext.com "Sublime Text").

Create a new file with this basic structure:

![Basic HTML Page](/images/HTML01.png)

Save the file. You can give it any name you want, as long as it ends with the **.html** extension.

## Setting up Leaflet
To make the web map work, we need to add a link to the [Leaflet CSS ](https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.css)file to the ```<head>``` section of the page. This will load a lot of predefined CSS classes and elements to your HTML page.

````<link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.css" />````

Your page should look like this:

![HTML Step 2 - add Leaflet CSS](images/HTML02.png "HTML Sample 02")

Next, add a link to the [Leaflet JavaScript file](http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.js "Leaflet JavaScript library") to the ```<head>``` of your document, like this:

`<script src="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.js"></script>`

Your document should look like this:

![Coding Maps with Leaflet - Step 3 - Add Leaflet js](images/HTML03.png "Coding Maps with Leaflet - Step 3")

Lastly, we need to add some of our own CSS to make the map as large or as small as we want.

Set the `margin` and `padding` on the document to ```0```. Next, create a declaration for the ID `#map`, and set the `height` to `800px`.

## Add the map to your page
Next we’ll add a `div` element on the page where we want our map to appear.

In the `<body>` section of your page, add the following code:

` <div id="map"></div>`

Next, add another `<script>` tag to your page, immediately following the closing `</div>` tag.

We’ll be making a map of Vancouver, BC using OpenStreetMap. Add this code inside the `<script>` tag:

`var map = L.map('map').setView([49.288, -123.125], 16);`

Your HTML should look like this.


![Coding Maps with Leaflet - Step 4 - Add style declaration](images/HTML04.png)


If you’ve come this far, give yourself a pat on the back! Next, we’ll add some map tiles.
