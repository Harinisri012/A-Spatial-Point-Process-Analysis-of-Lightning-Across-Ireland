# A-Spatial-Point-Process-Analysis-of-Lightning-Across-Ireland

This project investigates the spatial variability of lightning strikes across Ireland and examines whether the observed spatial patterns can be explained by topographic and meteorological conditions within a spatial point process framework.

## Research Question

> Can the visually observed spatial variability of lightning strikes across Ireland be explained by topographic and meteorological covariates within a spatial point process framework?

## Objectives

- Analyse the spatial distribution and clustering of lightning strikes across Ireland.
- Investigate the influence of topography, particularly elevation, on lightning occurrence.
- Examine the relationships between lightning occurrence and meteorological conditions.
- Develop spatial statistical models to account for environmental and spatial variation.
- Evaluate model performance using appropriate statistical diagnostics and visualisations.

## Data

The analysis combines multiple environmental and spatial datasets:

- **Lightning strike observations** across Ireland.
- **ERA5 reanalysis data** for meteorological variables.
- **Copernicus DEM** data for elevation and topographic information.
- **Geographic boundary data** for Ireland.

## Methodology

The project applies spatial statistical methods to investigate the environmental drivers of lightning occurrence. The analysis includes:

- Exploratory spatial data analysis
- Spatial point pattern analysis
- Inhomogeneous Poisson Point Process (IPP) modelling
- Generalised Additive Models (GAMs)
- Log-Gaussian Cox Processes (LGCP)
- INLA/SPDE-based spatial modelling
- Model diagnostics and visualisation

## Environmental Covariates

The models consider a range of topographic and meteorological variables, including:

- Elevation
- Temperature
- Dew point
- Convective Available Potential Energy (CAPE)
- Convective Inhibition (CIN)
- Mean sea-level pressure
- Total cloud cover
- 10-metre zonal wind component (`u10`)
- 10-metre meridional wind component (`v10`)

## Project Aim

The overall aim of this project is to determine whether topographic and meteorological factors can explain the spatial heterogeneity of lightning occurrence across Ireland while accounting for underlying spatial structure in the observed lightning point pattern.

## Technologies

The project primarily uses:

- **R**
- **Python**
- `spatstat`
- `mgcv`
- `INLA`
- `sf`
- `terra`
- `tidyverse`
- ERA5 NetCDF data
- Copernicus DEM

## Repository Structure

```text
├── data/
│   ├── lightning/
│   ├── meteorological/
│   └── topography/
│
├── scripts/
│   ├── data_processing/
│   ├── exploratory_analysis/
│   ├── point_process/
│   ├── gam/
│   └── inla_spde/
│
├── figures/
│
├── results/
│
└── README.md
