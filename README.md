# CryptoClustering
Module 19 Challenge
Cryptocurrency Clustering with K-Means and PCA

# Overview

This project applies K-Means Clustering and Principal Component Analysis (PCA) to cluster cryptocurrencies based on their market performance. The goal is to analyze patterns in cryptocurrency price changes and optimize clustering using dimensionality reduction.

# Features

Data Normalization: Uses StandardScaler() to normalize the dataset.

Elbow Method: Determines the optimal number of clusters for K-Means.

K-Means Clustering: Groups cryptocurrencies based on scaled data.

PCA Optimization: Reduces dimensionality for improved clustering.

Data Visualization: Uses hvPlot to create interactive scatter plots.

# Steps

1. Data Preparation

Load and normalize data using StandardScaler().

Create a DataFrame with scaled values, maintaining coin_id as the index.

2. Finding the Best k for Clustering

Implement the Elbow Method to find the optimal number of clusters (k).

Plot the elbow curve to visualize inertia values.

3. Clustering Cryptocurrencies (Original Data)

Apply K-Means clustering on the scaled DataFrame.

Predict clusters and add them to the dataset.

Create an hvPlot scatter plot to visualize the clusters.

4. Optimizing with PCA

Reduce features to three principal components using PCA.

Retrieve explained variance to assess retained information.

Create a new PCA-transformed DataFrame.

5. Finding the Best k for PCA Data

Reapply the Elbow Method to the PCA-reduced DataFrame.

Compare optimal k values between original and PCA-transformed data.

6. Clustering Cryptocurrencies (PCA Data)

Run K-Means clustering on the PCA-transformed DataFrame.

Predict clusters and add them to the dataset.

Create an hvPlot scatter plot using PCA components.

7. Results Comparison

Compare elbow curves from both original and PCA data.

Analyze differences in clustering performance.

Visualization & Interpretation

Compare elbow curves from original vs. PCA-transformed data.

Overlay cluster results from both methods for evaluation.

Interpret the impact of feature reduction on clustering accuracy.

# Requirements

Python Libraries: pandas, sklearn, hvPlot, matplotlib

Data Source: Cryptocurrency market data

# Deployment

Commit changes to a GitHub repository.

Include clear commit messages and proper documentation.

# Conclusion

This project demonstrates the effectiveness of K-Means Clustering and PCA in analyzing cryptocurrency data. Using fewer features can enhance clustering efficiency while maintaining valuable insights.