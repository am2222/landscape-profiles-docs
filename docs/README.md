# landscape-profiles-docs

Landscape Profile is a conservation planning tool for helping planners analyze prospective developments from the perspective of cumulative impacts on the landscape and landscape connectivity. The tool has been developed in collaboration with planners in British Columbia, and is currently in the beta testing phase of development. The Conservation Planning Tool (CPT) is an initiative led by the [Okanagan Collaborative Conservation Program (OCCP)](https://okcp.ca/).

## Design Goals

The CPT has been developed with the following Design Goals in mind:

1. **Scalability**: Want a tool that can scale to new and more complex models for assessing connectivity and cumulative impacts and new datasets 
2. **Transparency**:  Clear documentation of data and models and how computations are performed
3. **Open Source**: Use open source libraries as much as possible, allow for extendibility with a flexible modelling framework
4. **Use-Case Driven**: Maintain a narrow focus on a clear target use case, supporting evaluation of metrics in relation to development proposals
5. **Iterative Feedback**: Work with planners and stakeholders early and often to incorporate feedback into tool design and approach


## Core Concepts

![Core Concept Overview](https://github.com/am2222/landscape-profiles-docs/blob/main/img/concepts.png?raw=true "Overview of core concepts")

There are a few core concepts modelled in the project. 

- Plan Polygons - these are geospatial data uploaded by the user representing a proposed development. Often these files are described as limit of disturbance polygons. Currently, shapefile format as a zipped folder is supported, with data projected in BC Albers coordinate system.

- Base Layers - these are system-managed datasets which describe features of the environment which will be analyzed in relation to a Plan Polygon. Layers such as Sensitive Ecosystem Invetory (SEI) are available as well as many others. Users can also upload a user-specific base layer (e.g., ESA polygons) using the plan upload feature and designating the layer as a Base Layer. The number and scope of available Base Layers will grow over time.

- Reference Zones - these are the scales over which analysis are reported, which currently include Plan, Parcel, Regional District and Watershed.

- Models - models are the analysis that is being run. The architecture is designed to support adoption of new and more complex models for cumulative impacts and connectivity analysis. Currently, models are limited Spatial intersection model, a model implementing landscape pattern indices, and a model incorporating human footpring layers. Models may be unique analytical models or unique combinations of other models and base layers (e.g., pre-configured models).

- Reports - these are the visual outputs of models, which can be viewed online or downloaded as a PDF report.


## Tutorials

A [tutorial is available here](docs/intro.md) demonstrating key functionality of the CPT.

## More information

## Sponsors

The CPT was sponsored by the following organizations:

![Sponsors](/img/sponsors.png "Sponsors of the Conservation Planning Tool")
