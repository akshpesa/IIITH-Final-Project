# IIITH-Final-Project

This project uses satellite images and machine learning to map flood-affected areas in Bihar, India. By combining radar (Sentinel-1), optical (Sentinel-2), elevation, and rainfall data, we create accurate flood maps to help disaster response teams.

## Features
Uses cloud-penetrating Sentinel-1 SAR for reliable flood detection.<br>
Combines multiple features: water indices, elevation, slope, SAR ratios, and change detection.<br>
Trains a Random Forest classifier on balanced, labeled samples.<br>
Produces interactive flood maps for validation and visualization.

## Data Sources<br>
Sentinel-1 SAR (VV, VH bands)<br>
Sentinel-2 Optical (for NDWI, MNDWI)<br>
SRTM Elevation & Slope<br>
Rainfall data

## Tools:
Google Earth Engin<br>
Python (Colab/Jupyter): earthengine-api, geemap, scikit-learn, pandas, matplotlib, seaborn

## How to Use
Clone this repo and open the main notebook in Google Colab or Jupyter.<br>
Authenticate with Google Earth Engine.<br>
Run the workflow: data download, feature extraction, model training, and mapping.<br>
Visualize results interactively with geemap.

## Results
Achieved nearly perfect accuracy (ROC-AUC ≈ 0.999) on validation data<br>
Flood maps match official reports and news coverage for July 2019
