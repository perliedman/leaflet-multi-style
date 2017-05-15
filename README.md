Leaflet Multi Style
===================

A plugin to quickly add multiple styles to the same GeoJSON data. [Demo](http://www.liedman.net/leaflet-multi-style).

## Using

As an extra option, you can add an array of `styles` instead of just a single `style`.

```js
var vectorLayer = L.geoJson.multiStyle(geojson, {
    styles: [
        {color: 'black', opacity: 0.15, weight: 10},
        {color: 'white', opacity: 0.8, weight: 8},
        {color: 'red', opacity: 1, weight: 4}
    ],
}).addTo(map);
```

Similarily, there is also an option `filters` that works just like the original option `filter`, but is called for
each style in `styles`.
