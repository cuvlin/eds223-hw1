# Hazardous Waste Proximity and Linguistic Isolation in Orange County, CA

## About

This repository contains Homework 1 for EDS 223 (Geospatial Analysis & Remote Sensing) in the UCSB Master of Environmental Data Science program. It uses the EPA's 2023 EJScreen data at the Census Block Group level to map two variables across Orange County, California:

- **Limited English-speaking households** (`LINGISOPCT`)
- **Hazardous waste proximity EJ index** (`D2_PTSDF`)

The maps are compared side by side to look for a possible spatial link between linguistically isolated communities and exposure to hazardous waste.

## Repository Structure

```
eds223-hw1
├── README.md
├── .gitignore
├── ej_screen.qmd        # Quarto document with analysis and maps
├── ej_screen.pdf        # Rendered report
├── ej_screen_files/     # Figures generated when rendering
└── data/                # Not tracked (see Data Access)
    └── ejscreen/
        ├── EJSCREEN_2023_BG_StatePct_with_AS_CNMI_GU_VI.gdb
        ├── EJSCREEN_2023_BG_Columns.xlsx
        └── ejscreen-tech-doc-version-2-2.pdf
```

## Data Access

The data is **not stored in this repository** because `data/` is listed in `.gitignore`. To run the analysis, download the 2023 EJScreen Block Group geodatabase (state percentiles) along with its column descriptions and technical documentation. Then place the files in `data/ejscreen/` following the structure shown above.

## Getting Started

1. Clone the repository.
2. Add the data as described above.
3. Install the required R packages: `tidyverse`, `sf`, `here`, `tmap` (v4), `stars`, `viridisLite`.
4. Open and render `ej_screen.qmd` in the IDE of your choice (I use Positron).

## Author

Calvin Fu ([@cuvlin](https://github.com/cuvlin))

## References

- U.S. Environmental Protection Agency (EPA). (2023). *EJScreen: Environmental Justice Screening and Mapping Tool* (Version 2.2) [Data set].
- U.S. EPA. (2023). *EJScreen Technical Documentation, Version 2.2*.

## Acknowledgements

This assignment was completed as part of EDS 223 at the Bren School of Environmental Science & Management, UC Santa Barbara.
