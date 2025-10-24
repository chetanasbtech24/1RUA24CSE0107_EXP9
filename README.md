# K-Means Clustering Analysis

This notebook demonstrates K-Means clustering on two different datasets: a synthetic income dataset and the Iris dataset.

## Synthetic Income Dataset Clustering

The first part of the notebook performs K-Means clustering on a synthetic dataset containing Age and Income information.

**Steps:**

1.  **Load Data**: The `income.csv` file is loaded into a pandas DataFrame.
2.  **Visualize Data**: A scatter plot is created to visualize the distribution of Age vs. Income.
3.  **K-Means Clustering (Initial)**: K-Means clustering is applied with an initial assumption of 3 clusters.
4.  **Add Cluster Labels**: The predicted cluster labels are added to the DataFrame.
5.  **Visualize Clusters (Initial)**: The clusters and their centroids are visualized.
6.  **Preprocessing (MinMax Scaling)**: MinMaxScaler is applied to both Age and Income features to scale them between 0 and 1.
7.  **Visualize Scaled Data**: A scatter plot of the scaled data is shown.
8.  **K-Means Clustering (Scaled Data)**: K-Means clustering is applied again with 3 clusters on the scaled data.
9.  **Add Cluster Labels (Scaled Data)**: New cluster labels based on scaled data are added to the DataFrame.
10. **Visualize Clusters (Scaled Data)**: The clusters and their centroids from the scaled data clustering are visualized.
11. **Elbow Plot**: The Elbow method is used to determine a potentially optimal number of clusters by plotting the Sum of Squared Errors (SSE) for different values of k.

## Iris Dataset Clustering Exercise

The second part of the notebook addresses an exercise using the Iris flower dataset. The goal is to cluster flowers based on petal dimensions.

**Steps:**

1.  **Load Data**: The Iris dataset is loaded from `sklearn.datasets`.
2.  **Prepare Data**: A DataFrame is created containing only 'petal length (cm)' and 'petal width (cm)' features.
3.  **Preprocess Data**: MinMaxScaler is applied to the selected petal features.
4.  **Determine Optimal k**: The Elbow method and Silhouette analysis are used to find the optimal number of clusters for the Iris petal data.
5.  **Apply KMeans**: K-Means clustering is applied with the optimal number of clusters determined in the previous step.
6.  **Visualize Clusters**: The resulting clusters and their centroids for the Iris petal data are visualized.

**Key Findings (Iris Dataset):**

*   Clustering was performed on the 'petal length (cm)' and 'petal width (cm)' features.
*   MinMaxScaler was successfully applied to scale the features.
*   Based on silhouette analysis, the optimal number of clusters for the Iris petal data was found to be 2.
*   K-Means clustering with 2 clusters revealed two distinct groups based on petal dimensions.

## Dependencies

*   pandas
*   sklearn
*   matplotlib
*   numpy

To run this notebook, ensure you have these libraries installed.
