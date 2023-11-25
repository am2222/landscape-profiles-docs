# Model Card for SPI model

**Slug**: `AggReportModel`

**Description**: `Aggregated Report Model`

**Version**: `0.1`


[//]: # (Provide a quick summary of what the model is/does. [Optional])
This model computes supports the creation of aggregate reports which pull together model results from one or multiple reports. 

# Model Details

## Model Description

[//]: # (Provide a longer summary of what this model is/does.)
Each model provides report output summarizing its results. However, users may want to create a single report which aggregates multiple model runs into a single report. This model simply concatenates previously run model results into a single report.

- **Developed by:** Colin R., Majid H.
- **Model type:** Report model
- **Language:** Javascript
- **License:** 
- **Parent Model:** N/A
- **Resources for more information:** N/A



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

