# GeoJSON/TopoJSON Austria (2016-2021)
Geo- and TopoJSON files of municipalities, districts and states in Austria, as of January 2021. Older versions can be found in the folders '2016' and '2017' - they include the borders as of June 2016 and January 2017. If really old versions are needed (like 2013, before the major 'Styrian update'), see [here](https://wahlen.strategieanalysen.at/geojson/).

The files for 2021 are based on [Statistik Austria - data.statistik.gv.at](https://data.statistik.gv.at/web/meta.jsp?dataset=OGDEXT_GEM_1) and have been modified in several ways:

1. The files contain only two fields:
  * iso (string): the 'Gemeindekennziffer', a number to identify region/state (first digit), district (first three digits) and municipality (whole number) - accordingly the iso in district and state files is only three or one character long
  * name (string): the name of the municipality
2. Simplified to 95%, 99.5% and 99.9% (using [mapshaper.org](http://www.mapshaper.org))
3. Turned into GeoJSON and TopoJSON format
4. Created district and state files for easier use

The municipality and district file both contain two versions of Vienna: One as single feature, one divided into its 23 districts. The features are placed on top of each other and can be filtered using the iso field ('900'/'90001' being the single feature).


2021 also contains a shp/geojson/topojson of "Siedlungseinheiten" per district, used to symbolise districts (see [here](https://www.statistik.at/web_de/klassifikationen/regionale_gliederungen/siedlungseinheiten/index.html) for an explanation, and [here](https://www.drawingdata.net/cov_bezirke/) for a use case):

1. It follows the structure of the other files, containing 'iso' and 'name' as fields. 
2. A simplified version is provided with a simplification of 75% - too much details disappears if using a higher rate.
3. Note that while the map is based on data from 2011, the district data is from 2020.

<br/><br/>
The older versions are based on Geoland.at/Land Kärnten (no longer online). They can be used if one needs for instance the border of the district 'Wien Umgebung'. Additionally to the changes above:

1. Fixed several spelling issues with the names and - as far as possible - changed them to the official name used by Statistik Austria
2. Added two special maps:
* District map of Vienna hovering enlarged over Bavaria
* Municipality map with Vienna being divided into districts

<br/><br/>
All files CC BY 4.0, Flooh Perlot (https://creativecommons.org/licenses/by/4.0/)

Original file 2021: CC BY 4.0 Statistik Austria - data.statistik.gv.at

Original file Siedlungseinheiten 2021: CC BY 4.0 Statistik Austria - data.statistik.gv.at

Original file: CC BY 3.0 Geoland Kärnten
