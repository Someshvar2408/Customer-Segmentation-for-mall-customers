# Customer Segmentation: K-Means vs. DBSCAN

This project demonstrates customer segmentation of mall customers using clustering algorithms, focusing on comparing **K-Means** and **DBSCAN**. The project evaluates the performance and characteristics of these two algorithms for unsupervised learning tasks.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Algorithms Used](#algorithms-used)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Setup and Installation](#setup-and-installation)
- [Visualization](#visualization)
- [Conclusion](#conclusion)
- [Future Work](#future-work)

## Overview
Customer segmentation is crucial for businesses to understand their customer base, improve marketing strategies, and provide personalized experiences. This project uses clustering techniques to group mall customers based on their attributes and spending patterns.

## Dataset
The dataset used in this project, `mall_customers.csv`, contains the following features:
- **Age**: Age of the customer
- **Gender**: Gender of the customer
- **Annual Income (k$)**: Annual income in thousand dollars
- **Spending Score (1-100)**: Spending score assigned to the customer

## Project Workflow
1. **Data Preprocessing**:
   - Handled missing values by filling with the mean.
   - Standardized features using `StandardScaler` for clustering.
   - One-hot encoded the `Gender` feature.
   - Removed outliers using Z-scores.

2. **Exploratory Data Analysis (EDA)**:
   - Generated a correlation heatmap to identify relationships among features.
   - Performed Principal Component Analysis (PCA) for dimensionality reduction.

3. **Clustering**:
   - Applied **K-Means** to find clusters.
   - Applied **DBSCAN** to find density-based clusters.
   - Visualized clusters using PCA.

4. **Evaluation**:
   - Calculated silhouette scores to evaluate cluster quality.
   - Compared the performance of K-Means and DBSCAN.

## Algorithms Used
- **K-Means**: Partition-based clustering algorithm that minimizes intra-cluster variance.
- **DBSCAN**: Density-based clustering algorithm that identifies clusters based on density connectivity.

## Evaluation Metrics
- **Silhouette Score**: Measures how similar a data point is to its cluster compared to other clusters. A higher silhouette score indicates better-defined clusters.

## Results
- **K-Means**:
  - Produced well-defined clusters with a silhouette score of **X.XX**.
  - Demonstrated clear centroids and good performance with scaled data.

- **DBSCAN**:
  - Found clusters based on density with a silhouette score of **Y.YY** (or did not find meaningful clusters).
  - Sensitive to parameters `eps` and `min_samples`.

## Setup and Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/customer-segmentation.git
   ```
2. Navigate to the project directory:
   ```bash
   cd customer-segmentation
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Python script:
   ```bash
   python customer_segmentation.py
   ```

## Visualization
1. **Heatmap**: Displays feature correlations.
2. **Elbow Method**: Helps determine the optimal number of clusters for K-Means.
3. **Cluster Visualization**:
   - Scatter plots with PCA for K-Means and DBSCAN clusters.
   - Silhouette plots for each clustering method.

## Conclusion
- **K-Means** performed better for this dataset with clearly defined clusters and higher silhouette scores.
- **DBSCAN** struggled with parameter sensitivity and found meaningful clusters only for certain configurations.
- The project highlights the importance of selecting the right clustering algorithm based on data characteristics.

## Future Work
- Experiment with other clustering algorithms like **Agglomerative Clustering**.
- Fine-tune DBSCAN parameters to improve cluster quality.
- Explore additional features or datasets for customer segmentation.

---

Feel free to reach out with suggestions or questions about the project. Contributions are welcome!

