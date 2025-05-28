
# Semi-Automated Workflow for Multi-Scenario Flood Risk Mapping

This repository provides the scripts, documentation, and example workflows developed as part of a study titled **"Semi-automated workflow for multi-basin, multi-scenario flood risk modeling, mapping, and impact assessment."** The tools are designed to automate flood modeling and mapping processes using Python in ArcGIS Pro.

## Overview

The workflow was developed to support large-scale flood risk assessments involving multiple watersheds and scenarios. It automates key geoprocessing steps, including:

- Subsetting datasets based on HUC boundaries
- ArcHydro preprocessing and drainage delineation
- Computation of unsaturated zone and soil storage capacity
- Generation of input tables for the Cascade 2001 model
- Probabilistic flood mapping using z-scores
- Flood impact and risk scoring for critical infrastructure
- Automated map creation for scenario outputs

This approach has been tested and applied in several watersheds across Florida to support watershed master planning and flood resilience analysis.

## Key Features

- Reduces manual processing time by over 85%
- Handles 48 flood scenarios per region (rainfall, SLR, tidal events)
- Supports probabilistic flood risk mapping using LiDAR DEMs and Z-score analysis
- Fully compatible with ArcGIS Pro Notebooks
- Designed to work with existing data and output from the Cascade 2001 hydrologic model

## Repository Structure

```
├── Doccuments/
│ ├── Data_Management_Guide.pdf
│ └── Prioritizing Risk Ch 5_for DD comp scores t....
├── Map_templates/
├── Notebooks/
├── Outputs / FloodMaps/
├── SampleData/
├── .gitattributes
├── LICENSE
└── README.md
```

## Getting Started

### Requirements

- ArcGIS Pro with Python Notebook support (ArcPy environment)
- Licensed access to ArcHydro tools within ArcGIS
- Python 3.x (bundled with ArcGIS Pro)
- Familiarity with ArcGIS geoprocessing tools and spatial data structure

### Installation

Clone the repository:

```bash
git clone https://github.com/mandalanil/Semi-Automated-workflow-for-flood-risk-mapping.git
```

Open ArcGIS Pro and navigate to the Notebook tab. You can then run the `.ipynb` files directly, following the folder structure provided in this repository.

### Input Data Requirements

- DEM (LiDAR-based, in feet)
- Water table elevation raster
- Land cover (NLCD)
- Water mask and impervious mask rasters
- Design rainfall rasters for 1-day and 3-day events
- HUC12 boundary shapefiles
- Stormwater infrastructure (optional)

Detailed instructions on data format and folder organization are provided in the [Data Management Guide](https://github.com/mandalanil/Semi-Automated-workflow-for-flood-risk-mapping/blob/main/Doccuments/Data_Management_Guide.pdf).


## Output

- Excel tables of Cascade model inputs
- Raster outputs of soil storage, z-scores, and flood extent
- Feature classes with flood risk and consequence scores
- Map layouts for flood scenarios

## Citation

If you use this workflow in your research or planning project, please cite:

> Mandal, A.K., Thapa Chhetri, M., Bloetscher, F. et al. Semi-automated workflow for multi-basin, multi-scenario flood risk modeling, mapping, and impact assessment. Nat Hazards (2025). https://doi.org/10.1007/s11069-025-07361-6

## License

This project is shared for academic and non-commercial use. Please acknowledge the authors and Florida Atlantic University's Center for Water Resiliency and Risk Reduction (CWR³) in any derived work.

## Contact

For questions, suggestions, or contributions, please contact:

**Anil Kumar Mandal**  
Department of Civil, Environmental, and Geomatics Engineering  
Florida Atlantic University  
Email: kanil2310@gmail.com, amandal2023@fau.edu

**Madan Thapa Chhetri**  
Department of Civil and Environmental Engineering  
Lehigh University  
Email: chhetrim79@gmail.com
