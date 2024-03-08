# Introduction to the Conservation Planning Tool

## Getting Started
The purpose of this tutorial is to provide a clear guide to overview the core functionality of the CPT. The analyses and reporting documented here is for demonstration purposes only.

### The Dashboard View
The first view of the CPT is a dashboard view which is essentially a map with available base layers. The map view should be set to the general area of interest you will be working in, which currently is limited to the Okanagan Region.

Not all base layers are viewable in the dashboard. Note that the map view can be maximized with the `Enter Fullscreen`  button in the top right corner. As well, the map view can be tilted to reveal a 3D landscape view using a right click and pan operation with the mouse. 

![Dasboard Map View](https://github.com/am2222/landscape-profiles-docs/blob/main/img/dashboard_view.png?raw=true)

### Creating a User 
To run an analysis in the CPT you must be logged in as a registered user. A user can be created by clicking the top right button `Login/Register`  and users can use an existing account (Google or Microsoft) or an email to create a user account in the system.

![User Registration](https://github.com/am2222/landscape-profiles-docs/blob/main/img/screenshot_registerbutton.png?raw=true)

### Workspaces
Workspaces can be thought of as distinct folders where collections of plans and models are stored. It may be useful to store all analyses associated with a particular development or project or season in a specific workspace. Using workspaces is optional, and if a new workspace is not created, the default workspace will be used automatically. 

Creating a new workspace is straightforward - just provide a name and description and whether you want this to be activated as the workspace that will be used for storing results.

![Add a  new workspace](https://github.com/am2222/landscape-profiles-docs/blob/main/img/add_workspace.png?raw=true)


### Data and Models Documentation
Detailed data and model documentation is available on the left panel of the CPT.

### Data Upload to the CPT
Currently the tool supports upload of geospatial data in shapefile format, zipped up as a single zip file. The data should have a coordinate reference system defined in the `prj` file associated with the shapefile. The operational coordinate reference system for the CPT is the [BC Albers Projection](https://epsg.io/3005) - data that are represented in other projections will be reprojected to BC Albers. 

For plan polygons, each polygon should ideally be the disturbance footprint of the development, with internal divisions merged into a single polygon. For base layer polygons, ensure that the baselayers overlap the plan polygon you are working with. In general, uncompressed shapefiles should not exceed 10 mb.

***

## A Sample Workflow
Assuming you have familiarized yourself with the basic interface and have a logged in registered user with the CPT, we can walk through a simple analysis to demonstrate the workflow. Here we will use some sample data from the City of Kelowna for demonstration purposes.

To complete the workflow below, first [download the sample data](https://github.com/am2222/landscape-profiles-docs/blob/main/files/limit_of_disturbance.zip?raw=true)

### Plan Upload
`Click` on the `Plan Upload` link on the left panel. Enter in details associated with this plan (which is development proposal in the City of Kelowna, B.C.). `Click` on the `Drag file here to upload` button and navigate to the sample dataset downloaded above. `Click submit` to upload the plan polygon zip file to the system. You should get a notification that a process has started.



![Upload Plan](https://github.com/am2222/landscape-profiles-docs/blob/main/img/submit_plan.png?raw=true)



After a successful upload has run, you can view the uploaded plan in the `Plan List` section. Here you can inspect the geometry of the plan by clicking on the row, which will update the map view to visualize the plan in relation to the local area. As well, details of the plan - description, workspace, file name, upload time, etc. are available in the table. 



![Plan List](https://github.com/am2222/landscape-profiles-docs/blob/main/img/plan_list.png?raw=true)



The Map View in the Plan List interface can be expanded to full screen. As well, base layers can be turned on to examine their relation to the plan polygon. This may inform what layers to use in a subsequent model analysis. Note also that by right clicking on the map and panning, the perspective of the map view can be rotated to reveal topographyof the area. For example here is the view of the plan with SEI layer turned on and rortated to look westward across Okanagan Lake.



![Plan List Map View](https://github.com/am2222/landscape-profiles-docs/blob/main/img/view_west.png?raw=true)



The next step is to run a landscape model on the data.

### Running a Landscape Model
`Click` on `Landscape Models` on the left panel. Here you can access tools to run a lanscape model with the uploaded data and available base layers. Also, there is a model history, showing previous records of model runs. You will likely see a single entry for your upload plan, which triggers a background model for uploading and storing data and associating it with your user account. 

Details of what each model does can be examined in the documentation for each model. We will examine the `SPI Model- 0.1` which does spatial intersection analyses (i.e., GIS overlay) with a selected plan polygon and one or several base layers.

`Click` on `SPI Model - 0.1` to bring up the interface for running the model. The documentation for the model is automatically loaded along with the model's parameters. Enter some details into the `Model Name` and `Model Description` text boxes. Select the Plan data that you uploaded previously, and in the list of layers, delete any layers other than `Sensitive Ecosystem Inventory` leaving the field as `SNSTVCSST3` which has the SEI codes that we want to summarize for the development plan.



![Running the SPI model](https://github.com/am2222/landscape-profiles-docs/blob/main/img/model_run.png?raw=true)



When you `click  Run Model` you will be brought back to `Model History` and see that the model run is currently in progress. After a few seconds that `Status` should change to `Success`.



![Seeing Model Status](https://github.com/am2222/landscape-profiles-docs/blob/main/img/model_result.png?raw=true)



`Clicking on the last button` in the row will launch the report to view the results of the SPI model analysis.

### Viewing the Report
The report launches a summary of the intersection analyses. The top part of the report provides a tabular summary of model. Results are grouped by `Base Layer` which in this analysis is just one layer. Within that one layer we get values for distinct values of the variable selected when we ran the model (i.e., `SNSTVCSST3`), we have values of `NA` which means not sensitive, and `WD:co` which is a code for Woodland Coniferous in the SEI classification system. For each row we can see the total area and the proportion of area that intersects the `plan` polygon we uploaded, the `parcel` that the plan is associated with, and the regional district polygon that the plan is in. 



![SPI Result](https://github.com/am2222/landscape-profiles-docs/blob/main/img/spi_result.png?raw=true)

***

## Advanced Topics

### User-uploaded Base Layers

### Modifying Reference Zones

### Aggregation Fields

### Adding New Landscape Models

### Adding New Core Base Layers