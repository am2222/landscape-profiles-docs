# Dataset Card for Landcover 2019 dataset

**Slug**: `Landcover19`

**Description**: `Landcover data derived from Landsat imagery over all of Canada for the year 1999. High-resolution annual forest land cover maps for Canada's forested ecosystems (1984-2019). `

## Dataset Description

- **Homepage:** https://opendata.nfis.org/mapserver/nfis-change_eng.html
- **Organization:** Canadian Forest Service 
- **Paper:** [National Terrestrial Ecosystem Mapping System (NTEMS): Scientific Publications](https://www.researchgate.net/publication/357889457_National_Terrestrial_Ecosystem_Mapping_System_NTEMS_Scientific_Publications)
- **Point of Contact:** 


# Dataset Details
## Dataset Summary
High-resolution annual forest land cover maps for Canada's forested ecosystems (1984-2019). The annual time series of forest land cover maps are national in scope (entire 650 million hectare forested ecosystem) and represent a wall-to-wall land cover characterization yearly from 1984 to 2019. These time-series land cover maps were produced from annual time-series of Landsat image composites, forest change information, and ancillary topographic and hydrologic data following the framework described in Hermosilla et al. (2022), which builds upon the approach introduced in Hermosilla et al. (2018). The methodological innovations included (i) a refined training pool derived from existing land cover products using airborne and spaceborne measures of forest structure; (ii) selection of training samples proportionally to the land cover distribution using a distance=weighted approach; and (iii) generation of regional classification models using a 150x150 km tiling system. Maps are post-processed using disturbance information to ensure logical class transitions over time using a Hidden Markov Model. Hidden Markov Models assess individual year class likelihoods to reduce variability and possible noise in year-on-year class assignments (for instances when class likelihoods are similar).

### Data quality

### Spatial coverage
All of Canada

### Data Currency 
2019
### Data preprocessing
Clipped to BC study region, projected to BC Albers projection
### Coordinate reference system
BC Albers projection

### Citation
Hermosilla, T., M.A. Wulder, J.C. White, N.C. Coops, G. W. Hobart, (2018). Disturbance-Informed Annual Land Cover Classification Maps of Canada's Forested Ecosystems for a 29-Year Landsat Time Series. Canadian Journal of Remote Sensing. 44(1) 67-87.

Hermosilla, T., Wulder, M.A., White, J.C., Coops, N.C., 2022. Land cover classification in an era of big and open data: Optimizing localized implementation and training data selection to improve mapping outcomes. Remote Sensing of Environment. No. 112780

### Data Card Authors
C. Robertson and M. Hojati


