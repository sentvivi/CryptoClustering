# CryptoClustering

Introduction

In this project, we will leverage Python and unsupervised learning techniques to predict whether cryptocurrencies are affected by 24-hour or 7-day price changes. The primary tool we'll use is the K-means clustering algorithm.

Instructions

1. Rename the Notebook
Rename the Crypto_Clustering_starter_code.ipynb file as Crypto_Clustering.ipynb.

2. Load and Explore the Data
* Load the crypto_market_data.csv into a DataFrame.
* Get the summary statistics and plot the data to understand its structure.

3. Prepare the Data
* Use StandardScaler() from scikit-learn to normalize the data.
* Create a DataFrame with the scaled data, setting "coin_id" as the index.

4. Find the Best Value for k Using Original Scaled Data
* Implement the elbow method to find the optimal value for k.
* Visualize the inertia values for different k values.
* The best value for K in this case is 4.

5. Cluster Cryptocurrencies with K-means Using Original Scaled Data
* Initialize the K-means model with the best k value.
* Fit the model using the original scaled DataFrame.
* Predict the clusters and add a new column with the predicted clusters.
* Create a scatter plot using hvPlot to visualize the clustering.

6. Optimize Clusters with Principal Component Analysis (PCA)
* Perform PCA on the original scaled DataFrame to reduce features to three principal components.
* Retrieve the explained variance and answer: What is the total explained variance of the three principal components?
* Create a new DataFrame with PCA data, setting "coin_id" as the index.

7. Find the Best Value for k Using PCA Data
* Apply the elbow method on PCA data to find the best k value.
* Visualize the inertia values for different k values.
* The best value for k with PCA data is also 4.

8. Cluster Cryptocurrencies with K-means Using PCA Data
* Initialize the K-means model with the best k value from PCA.
* Fit the model using the PCA data.
* Predict the clusters and add a new column with the predicted clusters.
* Create a scatter plot using hvPlot to visualize the clustering.

9. Analyze Results
The impact of using fewer features to cluster the data with K-Means makes the visualization much clearer and easier to analyze