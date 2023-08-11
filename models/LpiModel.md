# Model Card for LPI model

**Slug**: `LpiModel`

**Description**: `Landscape pattern index model`

**Version**: `0.1`


[//]: # (Provide a quick summary of what the model is/does. [Optional])
This model computes a variety of [landscape pattern indices](https://www.srs.fs.usda.gov/pubs/ja/ja_oneil003.pdf) on categorical landcover data. Outputs can be used to understand degree of landscape fragmentation and when computed at multiple time points - to quantify change in fragmentation over time. 

# Model Details

## Model Description

[//]: # (Provide a longer summary of what this model is/does.)
This model requires a landcover raster as input. A variety of landscape pattern indices are computed. Currently, the model is 



- **Developed by:** Colin R., Majid H.
- **Model type:** Geospatial model
- **Language:** Python
- **License:** 
- **Parent Model:** N/A
- **Resources for more information:** Landscape pattern indices are performed using [pylandstats](https://pylandstats.readthedocs.io/en/latest/) library



# Uses

[//]: # (Address questions around how the model is intended to be used, including the foreseeable users of the model and those affected by the model.)


 

## Out-of-Scope Use

[//]: # (This section addresses misuse, malicious use, and uses that the model will not work well for.)



## Bias, Risks, and Limitations

[//]: # (This section is meant to convey both technical and sociotechnical limitations.)

Model results are constrained by the accuracy of input data sources. 


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

