XCSoar Map Repository
=====================

## Purpose
This repo maintains the source data for the maps in the official XCSoar data repository. 

The maps are regenerated if: 
 * Once a week on Thursday (github actions cron schedule)
 * On push to this repository (github actions)

## Usage 
 * edit maps.config.js and add the coordinates:
```javascript
"CAN_S_SK_MA": [-110.0, 48.6, -94.8, 53.9],
```

## TODO:
 * Upload maps.config.js to download.xcsoar.org/maps for website https://xcsoar.org/download/maps/ 
 * Upload maps.config.js to mapgen-data.sigkill.ch/ and update checksums
 * currently we upload to maps-test, move to production when comfortable. 

## Future Plans
 * Regnerate OSM data see https://github.com/lordfolken/mapgen-datagen
 * Deprecate VMAP1 data 
 * New SRTM Data containing the whole planet (https://mapgen-data.sigkill.ch/scripts/SRTM_Data_GeoTIFF/)
