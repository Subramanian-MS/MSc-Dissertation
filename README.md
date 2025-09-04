# MSc-Dissertation

# Comparison of Clustering Methods in High-Dimensional Data

This project compares popular clustering algorithms on synthetic high-dimensional datasets and on the UCI Human Activity Recognition (HAR) dataset. We evaluate performance with external and internal metrics and study the effect of dimensionality reduction with PCA.

## Project Overview

- **Datasets**
  - Synthetic Gaussian blobs with controllable properties (cluster separation, outliers, feature noise)
  - UCI HAR (smartphone sensors, 561 features)

- **Experiments**
  - Vary cluster separation
  - Add outliers
  - Add feature noise
  - Assess PCA impact (raw vs PCA with selected dimensions)

- **Algorithms**
  - K-means
  - Hierarchical clustering (Ward linkage)
  - Gaussian Mixture Models (GMM)
  - DBSCAN

- **Metrics**
  - External: Adjusted Rand Index (ARI)
  - Internal: Silhouette, Calinski–Harabasz (CH), Davies–Bouldin (DB)
  - Runtime

## Key Findings

Classical clustering methods performed strongly when clusters were compact and well separated, with K-means, Ward, and GMM showing high agreement with ground truth. DBSCAN was more resilient to boundary outliers and irregular shapes by labelling ambiguous points as noise, which preserved inlier quality when contamination increased. Across both synthetic data and HAR, applying PCA before clustering improved stability and reduced runtime while retaining most structure; PCA-50 was effective for analysis, while PCA-2 was used only for visualisation. Overall, there is no single best algorithm in all settings: centroid-based methods excel with spherical, balanced groups, GMM adapts to elliptical structure, and DBSCAN is preferable when robustness to noise and non-convex shapes is required.

## Data & Citation

This repository uses the **UCI Human Activity Recognition (HAR) Using Smartphones** dataset.

Citation:

Reyes-Ortiz, J., Anguita, D., Ghio, A., Oneto, L., & Parra, X. (2013). *Human Activity Recognition Using Smartphones* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C54S4K

