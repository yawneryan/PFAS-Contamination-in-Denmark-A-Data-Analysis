# PFAS-Contamination-in-Denmark-A-Data-Analysis

This project analyzes PFAS (Per- and Polyfluoroalkyl Substances) contamination sites across Europe, with a focus on **Denmark**. The dataset originates from publicly reported and verified PFAS monitoring records. The goal is to summarize, filter, and visualize contamination patterns to better understand spatial distribution and severity.

## Objectives
- Load and clean PFAS contamination data
- Summarize contamination levels by country
- Filter PFAS sites located in Denmark
- Visualize Denmark on a map and plot contamination sites
- Highlight high-contamination areas using threshold-based mapping
- Explore how contamination varies between different PFAS chemical types

## Key Steps (R)
- `read_csv()` / `read.csv()` to import data  
- `dplyr::filter()`, `group_by()`, `summarise()` for analysis  
- `pivot_longer()` to restructure PFAS chemical columns  
- `ggplot2` for maps and spatial visualization  
- `scale_color_viridis_c()` to display contamination intensity

## Visual Outputs
- Map of Denmark with all known PFAS sites
- Cities added as reference points
- PFAS sites colored by contamination level
- Optional log-scale color gradient to emphasize differences

## Requirements
- R (version ≥ 4.0)
- R packages:
  - `tidyverse`
  - `ggplot2`
  - `viridis`
  - `maps` or `rnaturalearth` (depending on setup)
  - `knitr` / `rmarkdown` for rendering

## Dataset
The dataset includes:
- Latitude / Longitude coordinates
- Site location and country information
- PFAS chemical concentration values
- Computed total PFAS contamination (`pfas_sum`)
