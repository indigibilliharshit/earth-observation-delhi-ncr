# Earth Observation Assignment - Land Cover Classification

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-1.9+-red.svg)](https://pytorch.org)
[![Geospatial](https://img.shields.io/badge/Geospatial-GDAL%20%7C%20Rasterio-green.svg)](https://gdal.org)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A comprehensive geospatial machine learning project for automated land cover classification in the Delhi-NCR region using satellite imagery and deep learning techniques. This project implements spatial analysis, dataset preparation, and CNN-based classification for Earth observation data.

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Visualizations](#visualizations)
- [Contributing](#contributing)
- [License](#license)

## 🌍 Overview

This project addresses **Scenario 1: Spatial Analysis and Land Cover Classification** as part of an Earth observation assignment. The system analyzes satellite imagery of the Delhi-NCR region to classify different land cover types using deep learning.

### Key Objectives

- **Spatial Filtering**: Filter satellite images using 60×60 km grid overlay
- **Land Cover Classification**: Classify 11 ESA WorldCover land cover types
- **Deep Learning**: Implement ResNet18 CNN for automated classification
- **Geospatial Analysis**: Comprehensive analysis of Delhi airshed region

### Key Features

- ✅ Spatial reasoning with grid-based filtering
- ✅ ESA WorldCover 2021 data integration
- ✅ ResNet18 CNN with transfer learning
- ✅ Interactive mapping with satellite basemaps
- ✅ Comprehensive evaluation metrics and confusion matrix analysis
- ✅ Delhi airshed land cover composition analysis

## 📊 Dataset

### Satellite Imagery
- **Total Images**: 9,216 RGB satellite images
- **Filtered Images**: 3,087 (after spatial filtering)
- **Image Size**: 128×128 pixels per patch
- **Coverage**: Delhi-NCR region

### Land Cover Classes (ESA WorldCover 2021)
- **Tree cover**: Forest and woodland areas
- **Shrubland**: Shrub-dominated areas
- **Grassland**: Natural grasslands
- **Cropland**: Agricultural areas (53.5% of Delhi airshed)
- **Built-up**: Urban and developed areas (23.3% of Delhi airshed)
- **Bare/sparse**: Bare soil and sparse vegetation
- **Water**: Permanent water bodies
- **Wetland**: Herbaceous wetlands

### Geographic Data
- **Delhi-NCR Region**: Administrative boundary shapefile
- **Delhi Airshed**: Air quality monitoring region boundary
- **Grid System**: 60×60 km uniform spatial grid

## 📁 Project Structure

```
Earth-Observation-Assignment/
├── data/                                    # Geospatial data files
│   ├── delhi_airshed.geojson               # Delhi airshed boundary
│   ├── delhi_ncr_region.geojson            # Delhi-NCR region boundary
│   └── worldcover_bbox_delhi_ncr_202...    # ESA WorldCover raster data
├── output_plots/                           # Generated visualizations
│   ├── airshed_landcover.png              # Delhi airshed land cover map
│   ├── class_distribution.png             # Class distribution chart
│   ├── confusion_matrix.png               # Model confusion matrix
│   ├── grid_overlay.png                   # Spatial grid visualization
│   ├── interactive_map.png                # Interactive satellite map
│   ├── landcover_distribution.png         # Land cover distribution
│   ├── prediction_examples.png            # Model prediction examples
│   └── training_curves.png                # Training/validation curves
├── earth_observation_landcover_classification.ipynb      # Main analysis script
├── earth_observation_report.pdf           # Comprehensive project report
├── requirements.txt                        # Python dependencies
├── LICENSE                                 # MIT License
└── README.md                              # This file
```

## 🚀 Installation

### Prerequisites
- Python 
- CUDA-compatible GPU (recommended for training)
- GDAL/OGR libraries for geospatial processing

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/indigibilliharshit/earth-observation-delhi-ncr.git
cd earth-observation-delhi-ncr
