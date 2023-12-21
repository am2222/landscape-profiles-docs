# Dataset Card for Wetland Classification

**Slug**: `Wetland_class`

**Description**: `Wetland classification in Okanagan region derived from Kristina Deenik MSc Thesis, titled CLASSIFYING WETLANDS USING RANDOM FOREST MACHINE LEARNING, AIRBORNE LIGHT DETECTION AND RANGING AND EARTH OBSERVATION SATELLITE DATA IN THE OKANAGAN BASIN, BRITISH COLUMBIA.`

## Dataset Description
Building on existing wetland inventories that have limited coverage, a random forest probabilistic model was developed to predict, classify and map wetlands in the Okanagan at a 10 m spatial scale. In total, 22 covariates representing multispectral and synthetic aperture radar metrics derived from Sentinel-2 and Sentinel-1; topography and vegetation derived from LiDAR; and ancillary geospatial data were used to classify wetlands. The model was trained using an existing wetland database and provincial datasets to predict the probability of each pixel belonging to the following six-classes: fen, marsh, shallow-water, swamp, upland, and open-water. Model performance was evaluated using a confusion matrix and had an overall accuracy of 84.8%. 

- **Homepage:**  [Earth Observation and Spatial Ecology Lab](https://www.eosel.org/)
- **Organization:** UBC-lab 
- **Paper:** [Associated Thesis Describing Methodology, Deenik 2022](https://open.library.ubc.ca/soa/cIRcle/collections/ubctheses/24/items/1.0413780)
- **Point of Contact:** Dr. Mathieu Bourbonnais


# Dataset Details
## Dataset Summary
The model predicted that 313.9 km² (3.6%) of the 8,635 km² study area represented areas where wetland probability was ≥ 50%. Marshes were the most commonly occurring wetland (159.0 km²) followed by swamp (150.3 km²), shallow-water (3.7 km²), and fen (0.9 km²). The most important predictor variables for wetlands were slope, distance from streams, probability of depression, number of days above five degrees Celsius, topographic position index, seasonal change in the normalized difference vegetation index, standard deviation of vegetation height, and the red band from Sentinel-2.

### Data quality
10 m spatial resolution

### Spatial coverage

### Data Currency 

### Data preprocessing
Original geoTif file was reprojected to BC Albers coordinate system and converted into Cloud Optimized Geotiff format using gdal utility with the following parameters: `gdal_translate -co TILED=YES -co COPY_SRC_OVERVIEWS=YES -co COMPRESS=LZW -co BLOCKXSIZE=256 -co BLOCKYSIZE=256 -co BIGTIFF=YES wetclass_50.tif wetclass_COG.tif`

### Coordinate reference system
BC Albers Projection

### Citation
Deenik, K. (2022). Classifying wetlands using random forest machine learning, airborne light detection and ranging and Earth observation satellite data in the Okanagan basin, British Columbia (T). University of British Columbia. Retrieved from https://open.library.ubc.ca/collections/ubctheses/24/items/1.0413780


### Data Card Authors
C. Robertson and M. Hojati


