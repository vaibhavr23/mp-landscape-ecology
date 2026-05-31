# Spatial Covariate Extraction — Madhya Pradesh

Reproducible R pipeline for extracting landscape-level ecological covariates 
across Madhya Pradesh for use in species distribution and occupancy models.

## Covariates extracted
- Elevation (SRTM DEM)
- Mean annual temperature + precipitation (WorldClim 2.1)
- Temperature and precipitation seasonality (WorldClim 2.1)
- Tree cover % (ESA WorldCover)

## Methods
Raster clipping, projection alignment, and zonal statistics across 52 MP 
districts using `terra`, `sf`, and `exactextractr` in R.

## Outputs
- District-level covariate table (`outputs/tables/mp_district_covariates.csv`)
- Publication-style maps of elevation, tree cover, and climate variables

## Data sources
- [WorldClim 2.1](https://worldclim.org)
- [ESA WorldCover](https://esa-worldcover.org)
- [GADM boundaries](https://gadm.org)

## How to run
Open `mp_landscape_analysis.Rmd` in RStudio and knit to HTML.
