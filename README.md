# VectorTileLayer-in-BasemapGallery
Example how to use VectorTileLayer in BasemapGallery widget
#Code
```javascript
      var basemapGallery = new BasemapGallery({
        showArcGISBasemaps: false,
        map: map
      }, "basemapGallery");

      var basemapVector = new Basemap({
        layers: [new BasemapLayer({
          styleUrl: "https://basemaps.arcgis.com/arcgis/rest/services/World_Basemap/VectorTileServer/resources/styles/root.json",
          type: "VectorTileLayer"
        })],
        title: "Vector Street",
        thumbnailUrl: "http://www.arcgis.com/sharing/rest/content/items/04e903465a3e497aa669212e08927cee/info/thumbnail/world_street_map.jpg"
      });

      basemapGallery.add(basemapVector);


      var custombasemapVector = new Basemap({
        layers: [new BasemapLayer({
          styleUrl: "http://gestagua.maps.arcgis.com/sharing/rest/content/items/ee10aa2275ae4a068478b730f3c53332/resources/styles/root.json",
          type: "VectorTileLayer"
        })],
        title: "Custom Vector",
        thumbnailUrl: "http://thumb1.shutterstock.com/display_pic_with_logo/1441490/293601764/stock-vector-vector-cartoon-clip-art-illustration-of-a-mean-angry-monster-soccer-ball-or-football-ripping-293601764.jpg"
      });

      basemapGallery.add(custombasemapVector);


      basemapGallery.startup();
```
#[**View Example**](https://saik003.github.io/VectorTileLayer-in-BasemapGallery/)
