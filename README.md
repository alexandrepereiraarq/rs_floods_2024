# Rio Grande do Sul 2024 Flood Impact Detection Project

## Description
This repo includes the code used in the Rio Grande do Sul 2024 Flood impact detection project.

## Goal
This repo has the following objectives: <br>
a. to access Sentinel 2 data.<br>
b. to delinete the maximum flood area (MFA) from the 2024 flood events.<br>
c. to import buildings and roads from OSM in the MFA.<br>
d. to output the quantification of buildings and the list of roads per municipality in the MFA.<br>

## Usage
Feel free to reuse the code if needed. Data licenses will follow the original providers' ones.

## Support
Reach out to our team: 
- alexandre.santos(at)lmu.de
- c.mirbach(at)lmu.de

## Roadmap
1. Download Sentinel 2a data from https://browser.dataspace.copernicus.eu <br>
In ArcGIS Pro (done!) <br>
2. With de NDWI from Copernicus, explore bands and values to determine flood extent threshold (used 2 Natural Breaks, threshold = 0.662131) <br>
3. Reclassify the raster, to binary values (0, if < 0.55, 1, if >= 0.55) <br>
4. Run Majority Filter (8 neighbours, half rule) <br>
5. Polygonize the raster
6. Remove cloudcover false positives, remove value = 0, remove area < 30 hectares <br>
In Python:
7. Generate individual polygons for each affected municipality <br>
8. Download OSM roads and buildings for each affected municipality <br>
9. Identify OSM road tracts and buildings intersecting with flooded area (outer join) <br>

## Authors and acknowledgment
Dr. Alexandre Pereira Santos
Charlota Mirbach


## Project status
Ongoing.