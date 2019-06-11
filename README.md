# Microcoft US Building Footprints by County

This repo contains a notebook that shows one method for taking the [Microsoft USBuildingFootprints dataset](https://github.com/Microsoft/USBuildingFootprints) and subsetting the huge state GeoJSON footprint files by county. This results in more manageable file sizes where the files are zipped CSV files with two columns - the county name and the geometry of the county footprints in [WKT format](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry); each row is a building footprint. Each file has the following naming convention: STATEABBREVIATION_GEOID_footprints.zip where the GEOID is the two digit state FIPS code followed by the 3 digit count FIPS code. You can find the GEOID and county name for each state and county in the `county_fipscode.csv` file in the data folder. While the resultant county files are not in this github repo (they are too big) you can find the files for California in this [Google drive folder](https://drive.google.com/open?id=1-XGvS25tQKKQ3HTqWjAfLJ4PaeXJ9yyY).

Take a look at the notebook to review the process and give it a try.

### Important note

There appear to be missing building footprints in the data that could be artifacts of source imagery tiling. Please review the [issue list](https://github.com/Microsoft/USBuildingFootprints/issues) on the Microsfot Building Footprints github site in general and [issue 42](https://github.com/Microsoft/USBuildingFootprints/issues/42) specifcally about this issue.

## Verion
 
The data referenced by this repo were downloaded from (https://github.com/Microsoft/USBuildingFootprints) on December 16, 2018 and processed on December 20, 2018. Checheck the Microsoft footprints github repo for updates to the data.
