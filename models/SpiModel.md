# Model Card for SPI model

**Slug**: `SpiModel`

**Description**: `Spatial intersection model`

**Version**: `0.1`


[//]: # (Provide a quick summary of what the model is/does. [Optional])
This model computes the intersection of input polygon layers and summarizes intersection results across a variety of spatial scales. 

# Model Details

## Model Description

[//]: # (Provide a longer summary of what this model is/does.)
This model takes a development plan limit of disturbance polygon as input, and computes the spatial intersections with selected base layers. The sum and proportions of intersections of each base layer are reported in the output. Base layers may be vector or raster, and all computations are performed in projected coordinates [BC Albers projection](https://epsg.io/3005).

*Vector base layer*: an agreggation field can be specified if intersections based on a categorical field are required (e.g., SEI polygons using a column with SEI codes).

*Raster base Layer - Discrete*: These are data where values in the raster are categories or codes, for example representing land cover class. Here summaries are reported for each class/unique value.

*Raster base Layer - Continuous*: These are data where values in the raster are measured quantities, for example representing NDVI (normalized differenced vegetation index).

- **Developed by:** Colin R., Majid H.
- **Model type:** Geospatial model
- **Language:** Python
- **License:** 
- **Parent Model:** N/A
- **Resources for more information:** Spatial operations performed using [geopandas](https://geopandas.org/en/stable/) and [shapely](https://shapely.readthedocs.io/en/stable/) libraries



# Uses

[//]: # (Address questions around how the model is intended to be used, including the foreseeable users of the model and those affected by the model.)


 

## Out-of-Scope Use

[//]: # (This section addresses misuse, malicious use, and uses that the model will not work well for. If the user enters content, print that. If not, but they enter a task in the list, use that. )



## Bias, Risks, and Limitations

[//]: # (This section is meant to convey both technical and sociotechnical limitations)

Model results are constrained by the accuracy of input data sources. Error may be introduced through plan polygons or base layers.


## Recommendations

[//]: # (This section is meant to convey recommendations with respect to the bias, risk, and technical limitations.)


# Technical Details


## Preprocessing

More information needed


 
## Evaluation

[//]: # (This section describes the evaluation protocols and provides the results.)


## Technical Specifications

### Model Architecture

File-based input. Geospatial processing in python. Report output in HTML.

### Compute Infrastructure

AWS Cloud compute.


### Citation

[//]: # (If there is a paper or blog post introducing the model, the APA and Bibtex information for that should go in this section.)

### Model Card Authors
C. Robertson and M. Hojati

[//]: # (This section provides another layer of transparency and accountability. Whose views is this model card representing? How many voices were included in its construction? Etc.) 

