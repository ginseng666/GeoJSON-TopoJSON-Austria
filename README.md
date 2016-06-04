# GeoJSON/TopoJSON Austria
Geo- and TopoJSON files of municipalities in Austria, as of June 2016

The files are based on [Geoland.at/Land Kärnten](https://www.data.gv.at/katalog/dataset/c33d36b0-f184-4f2a-89cc-839ca7fcf88a) and have been modified in several ways:

1. The files contain only two fields:
  * iso: the 'Gemeindekennziffer', a number to identify region/state (first digit), district (first three digits) and municipality (whole number)
  * name: the name of the municipality
2. Fixed several spelling issues with the names
2. Standardised "Sankt" and "St."
3. Simplified to 95%, 99.5% and 99.9% (using [mapshaper.org](http://www.mapshaper.org))
4. Turned into GeoJSON and TopoJSON format
