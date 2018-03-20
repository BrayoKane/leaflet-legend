# Leaflet.Legend

This is a simple legend plugin for Leaflet.  It can be used to add a small popup legend to a Leaflet map


### What is this?

This plugin allows you to add a simple popup legend to a Leaflet map.  It extends the Leaflet ```Control``` class: creating and positioning the necessary container elements. The actual legend content is defined separately as a legend element in the html and appended to the legend container (see Usage).

### Demo

An example can be found in [`example.html`](./example.html) or here: [OpenTrailMap](http://michaelskaug.com/projects/OpenTrailMap/)

## Usage

### Dependencies

- Leaflet 1.3.1

optional:
- font-awesome 4.4.0

### Install
Install with npm:
```
npm install leaflet-legend
```
or fork the [github project](https://github.com/mikeskaug/Leaflet.Legend).

### Example

After including ```leaflet-legend.js``` and ```leaflet-legend.css``` in your project, you can add a legend to your map with the following:

```js
var legend = new L.control.legend({
    buttonHtml: '<i class="glyphicon glyphicon-info-sign"></i>',
    items: {
        'red': 'reserved',
        'blue': 'not reserved'
    }
});
legend.addTo(map);
```

## License

[MIT License](http://opensource.org/licenses/MIT)
