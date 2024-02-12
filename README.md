# Ananlysis of Clustering using Pycaret
## Project Overview
The project involves the analysis of mall customers based on their annual income and spending score. The analysis is conducted using the caret library and clustering techniques to identify distinct customer segments.

## Key Steps
- Dataset: Utilize a dataset containing information about mall customers, including their annual income and spending score.

- Data Exploration and Preprocessing: Explore the dataset, check for missing values, outliers, and preprocess the data, which may include scaling or transforming variables for clustering.

- Caret Library: Leverage the caret library to streamline the machine learning workflow, providing a unified interface for different clustering algorithms.

- Clustering Algorithm: Apply clustering techniques (e.g., K-means, hierarchical clustering, DBSCAN) to group customers based on their annual income and spending score.

- Model Training: Use the caret library to train the clustering model, allowing for hyperparameter tuning if needed.

- Evaluation: Assess the quality of clusters using metrics like silhouette score or within-cluster sum of squares.

- Insights and Visualization: Interpret the results, gain insights into customer segments, and use visualization techniques (e.g., scatter plots, cluster profiles) to illustrate characteristics of each cluster.

## Output
1. KMeans
   ![image](https://github.com/pulkit8690/Clustering/assets/103959073/3a96758a-edc8-4a30-91bd-b53a61102cca)

2. AgglomerativeClustering
   ![image](https://github.com/pulkit8690/Clustering/assets/103959073/7f0c2484-d8f9-4367-82a9-bd035db71717)

3. DbScan
   ![image](https://github.com/pulkit8690/Clustering/assets/103959073/b9e57d2c-efaf-4a3f-a62f-4d2f8ab66aa3)



## Conclusion
Determining the best clustering algorithm depends on various factors, including the specific dataset characteristics, the goals of clustering, and the interpretation of evaluation metrics. However, we can analyze the provided results to make a recommendation based on the performance across different algorithms and processing methods.

Let's break down the performance of each algorithm based on the provided metrics:

1. KMeans:

- Achieves relatively good silhouette scores across different processing methods and subcluster sizes.
- Performs consistently well with PCA (Principal Component Analysis) preprocessing, indicating good feature representation.
- Scores decently on all evaluation metrics.

2. AgglomerativeClustering:

- Shows competitive silhouette scores, especially with PCA preprocessing.
- Performs well in terms of the Calinski-Harabasz score.
- Davies-Bouldin scores indicate moderate clustering quality.

3. DBSCAN:

- Generally lower silhouette scores compared to KMeans and AgglomerativeClustering.
- Performs poorly with transformation and normalization processing methods.
- Shows a slight improvement with PCA preprocessing.

#
Based on the provided results, KMeans with PCA preprocessing seems to be the best-performing algorithm. It consistently achieves good silhouette scores, indicating well-separated clusters, and maintains competitive scores across other evaluation metrics. Additionally, it shows stability across different subcluster sizes, which is desirable for robust clustering.

Therefore, I would recommend KMeans with PCA preprocessing as the best clustering algorithm based on the given results. However, it's important to consider other factors such as computational efficiency, interpretability of clusters, and domain-specific knowledge when selecting the final algorithm for your application.
