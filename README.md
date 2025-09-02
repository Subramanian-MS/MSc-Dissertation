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

   git clone https://github.com/Subramanian-MS/MSc-Dissertation.git
   cd MSc-Dissertation
