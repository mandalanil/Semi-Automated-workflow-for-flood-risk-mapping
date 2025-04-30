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

├── Notebooks/ │ ├── Input_preparation.ipynb │ ├── Risk_impact_assessment.ipynb │ └── Mapping_visualizations.ipynb ├── Documents/ │ ├── Data Management Guide.pdf │ └── README.md ├── SampleData/ │ └── Example_HUC12/ ├── Outputs/ │ └── FloodMaps/