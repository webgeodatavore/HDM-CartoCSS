# HDM-CartoCSS

The HDM rendering is a Carto project, focusing on the [Humanitarian Data Model](http://wiki.openstreetmap.org/wiki/Humanitarian_OSM_Tags).

Preview: http://map.hotosm.org

Compare: http://map.hotosm.org/compare.html


## Install

See the [wiki](https://github.com/hotosm/HDM-CartoCSS/wiki) for instructions.

## Differences with the original project

It's a forked version to accomodate one of our customers

### Replaced zipped files with shp

The replacement files are:

* https://osmdata.openstreetmap.de/download/simplified-water-polygons-split-3857.zip
* https://osmdata.openstreetmap.de/download/water-polygons-split-3857.zip

These zip replaced the previous broken links:

* http://data.openstreetmapdata.com/simplified-land-polygons-complete-3857.zip
* http://data.openstreetmapdata.com/land-polygons-split-3857.zip

### Status changed for some layers

The layers `poi-point` and `poi-poly` have a `status` set to `off` to hide them.

### Recipe to consume the source as mml or xml instead of yml

If you need `project.mml` file instead of `project.yml`, do `npm install -g yamljs` and execute `yaml2json --pretty project.yml > project.mml`

If you need `project.xml`, install `npm install -g carto` and from the previous `project.mml` file, generate the XML with `carto project.mml > project.xml`


## Licence

- stylesheet is licenced under CC0
- Nori icons are licenced under CC0
- [Maki icons](https://www.mapbox.com/maki/) by Mapbox are licenced under CC0
