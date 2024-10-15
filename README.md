# CryptoClustering
Module 19 Challenge

This project applies K-Means clustering to group cryptocurrencies based on their market data. It also uses Principal Component Analysis (PCA) to reduce the dataset's dimensionality and compare the clustering results.

## Project Steps

### 1. Load and Preprocess Data:
    - The cryptocurrency market data is loaded from a CSV file.
    - The data is scaled using StandardScaler for normalization.
### 2. K-Means Clustering:
    - The Elbow Method is used to determine the best number of clusters (k) by plotting the inertia for values of k from 1 to 11.
    - K-Means is applied to the normalized data using the optimal value of k.
### 3. PCA (Principal Component Analysis):
    - The data is reduced to three principal components using PCA to simplify the dataset while retaining most of the variance.
    - K-Means clustering is applied to the PCA-reduced data, and the results are compared with the original clustering.
### 4. Visualizations:
    - Elbow Curves: Elbow plots are generated for both the original and PCA-reduced data to compare optimal values of k.
    - Cluster Scatter Plots: Scatter plots are created to visualize the clusters based on the original and PCA-reduced datasets.
## Key Findings

 - The optimal value for k is 4, determined from the elbow curve for both the original and PCA-reduced data.
 - The clustering results from the original and PCA-reduced data are similar, showing that PCA effectively reduced dimensionality without losing important information.

## Technologies Used

 - Pytchon (with libraries: Pandas, scikit-learn, hvPlot, Matplotlib)
 - K-Means Clustering
 - Principal Component Analysis (PCA)
