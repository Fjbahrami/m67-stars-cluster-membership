# m67-stars-cluster-membership
Gaia DR3 based star cluster membership analysis using DBSCAN and Gaussian Mixture Models
# M67 Star Cluster Membership Analysis

## Overview

This project investigates the identification of probable members of the open star cluster Messier 67 (M67) using astrometric and photometric data from the Gaia Data Release 3.

"Unsupervised machine learning algorithms" are used to distinguish cluster stars from field stars and investigate the distribution of stellar populations.

## Objectives

- Retrieve stellar data from Gaia DR3 using ADQL queries.
- Perform data cleaning and exploratory data analysis.
- Investigate astrometric and photometric properties.
- Apply DBSCAN clustering.
- Explore probabilistic clustering using Gaussian Mixture Models (GMM).
- Compare clustering results and evaluate their limitations.
- Visualize candidate cluster members.

- ## Exploratory Data Analysis (EDA)

The initial exploratory analysis investigates the Gaia DR3 dataset retrieved for the M67 field.

### Data Quality Assessment

- Dataset dimensions and data types were inspected.
- Missing values were investigated.
- Duplicate records and duplicate Gaia source identifiers were checked.
- Descriptive statistics were calculated.
- Measurement uncertainties and astrometric quality indicators were explored.

### Statistical Analysis

- Feature correlation analysis
- Parallax distribution
- Proper motion distributions
- Outlier investigation using the IQR method
- Astrometric uncertainty analysis

### Astronomical Visualization

- Spatial distribution of stars (RA vs DEC)
- Spatial density using hexbin visualization
- Proper motion space (PMRA vs PMDEC)
- Color-magnitude diagram (BP-RP vs G magnitude)
- Parallax-based spatial visualization

### Feature Engineering

The following additional features were investigated:

- Total proper motion magnitude
- Angular separation from the adopted M67 center
- Proper motion signal-to-noise ratios

### Machine Learning Preparation

Initial feature scaling was explored using StandardScaler.

Feature selection and scaling strategies will be evaluated further before applying clustering algorithms such as DBSCAN and Gaussian Mixture Models.

### Current Status

Exploratory analysis and initial feature investigation are in progress. No final cluster membership labels have been assigned.


## Methods

- Data acquisition: Gaia DR3
- Data processing: Python, Pandas, NumPy
- Visualization: Matplotlib, Seaborn
- Clustering: DBSCAN, Gaussian Mixture Models
- Dimensionality reduction: PCA

## Repository Structure

The project is organized into notebooks, source code, datasets, and reports.

## Status

Project in progress.

