# M67 Membership Analysis — DBSCAN & GMM

## Objective

Investigate probable M67 star cluster membership using Gaia DR3 astrometric data and unsupervised machine learning.

## Dataset

- Source: Gaia DR3
- Initial sample: 3,655 sources
- Target: M67 (NGC 2682)

## Methodology

### 1. Initial Candidate Selection

Broad parallax and proper-motion constraints were used to construct an initial astrometric candidate sample.

These cuts are exploratory and do not represent definitive membership labels.

### 2. Feature Space Investigation

The following feature spaces were examined:

- PMRA and PMDEC
- PMRA, PMDEC, and Parallax
- Local sky position, Proper Motion, and Parallax

### 3. Feature Scaling

StandardScaler and RobustScaler were investigated.

### 4. DBSCAN

DBSCAN was applied to different feature spaces.

The epsilon parameter was investigated using K-distance plots and parameter sensitivity analysis.

### 5. GMM

Gaussian Mixture Models were used to investigate probabilistic grouping.

The number of Gaussian components was explored using BIC and AIC.

### 6. Model Comparison

DBSCAN cluster labels and GMM component probabilities were compared to identify agreement and disagreement between clustering methods.

## Limitations

- Initial candidate selection may exclude genuine cluster members.
- DBSCAN is sensitive to feature scaling and parameter selection.
- GMM assumes the data can be represented as a mixture of Gaussian distributions.
- The selected GMM component is not automatically equivalent to true cluster membership.
- Astrometric measurement uncertainties are not fully incorporated into the clustering algorithms.
- Cluster membership requires astronomical validation.

## Status

Exploratory clustering is in progress.

The generated clusters and GMM probabilities are considered candidate membership results, not confirmed membership labels.

