# GeoJSON/TopoJSON Austria (2016-2021)
Geo- and TopoJSON files of municipalities, districts and states in Austria, as of January 2017 
(an older version can be found in the folder '2016' - it includes municipalities, districts and states as of June 2016)

The files are based on [Geoland.at/Land Kärnten](https://www.data.gv.at/katalog/dataset/c33d36b0-f184-4f2a-89cc-839ca7fcf88a) and have been modified in several ways:

1. The files contain only two fields:
  * iso (string): the 'Gemeindekennziffer', a number to identify region/state (first digit), district (first three digits) and municipality (whole number) - accordingly the iso in district and state files is only three or one character long
  * name (string): the name of the municipality
2. Fixed several spelling issues with the names
3. Changed the 'Gemeindekennziffer' of municipalities in the former district of 'Wien Umgebung', as it was disbanded 2017
4. Simplified to 95%, 99.5% and 99.9% (using [mapshaper.org](http://www.mapshaper.org))
5. Turned into GeoJSON and TopoJSON format
6. Created district and state files for easier use (no more merging if you only need a certain level)
  * The district files don't contain 'Wien Umgebung' any more - if necessary, use the files from 2016

The folder "2017" contains some special maps:
* district maps with vienna as an enlarged feature, hovering over bavaria
* municipality maps with vienna being divided into districts

The folder "2020" for now only contains a shp of "Siedlungseinheiten" per district, used to symbolise districts. It only contains a field "id" that points to the district. See [here](https://www.statistik.at/web_de/klassifikationen/regionale_gliederungen/siedlungseinheiten/index.html) for an explanation. Note that while the map is based on data from 2011, the district data is from 2020.

The folder "2021" for now only contains GeoJSON and TopoJSON of the Austrian districts in different simplifications.

CC BY 4.0, Flooh Perlot (https://creativecommons.org/licenses/by/4.0/)

Original file: CC BY 3.0 Geoland Kärnten

Original file Siedlungseinheiten: CC BY 4.0 Statistik Austria - data.statistik.gv.at

Original file Districts 2021: CC BY 4.0 Statistik Austria - data.statistik.gv.at
