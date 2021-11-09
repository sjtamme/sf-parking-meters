sf-parking-meters
======

This map showcases geoprocessing with Node. 

## Data used from [DataSF](https://datasf.org/opendata/):
* San Francisco Neighborhood Quadrants - https://data.sfgov.org/Geographic-Locations-and-Boundaries/Planning-Department-Neighborhood-Quadrants/x89n-qawp
* Parking Meters - https://data.sfgov.org/Transportation/Parking-Meters/8vzz-qzz9  

## Colors from https://carto.com/carto-colors/

## Process:
* Inspected data to be used, added data to directory
* Initialized Node and npm 
* Got information on Shapefiles with mapshaper, inspect CRS for each**
* Used ogr2ogr to convert the parks Shapefile to WSG84 (was NAD83)**
* Converted Shapefiles to GeoJSON using ogr2ogr**
* Simplified lines with Mapshaper**
* Used Node to load, read, and write data
* Parsed and processed CSV data with Node
* Created a Leaflet web map using VS Code
* Used D3 to request and draw data to map
* Created a coordinated visualization map/legend
* Used Leaflet.markercluster plugin
* Committed work along the way

**NOTES: Although I did do these processes for files, they are not the files I ended up using in the map. I was unable to get the coordinated viz to work with the orginial files.

## Commands used in Command Line:
* cd - change directory
* mkdir - add new directory
* git status - checking the status of working tree
* git add & git commit - committing changes
* dir - list contents of current directory
* ogrinfo -so - get information about shapefiles (so flag means summary only)
* ogr2ogr - make CRS transformations, also used to convert file formats
* mapshaper -info - get information 
* mapshaper -simplify - removes verticies from polygons or polylines
* npm init - initializes npm/sets up new package
* node - runs scripts
