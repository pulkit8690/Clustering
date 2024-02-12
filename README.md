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
- Kmeans
| Algorithm   | Processing Method   | Subcluster Size   | Silhouette Score   | Calinski-Harabasz Score   | Davies-Bouldin Score   |
|-------------|---------------------|--------------------|---------------------|--------------------------|------------------------|
| KMeans      | No Data Processing | 3                  | 0.384584993         | 2393.003014              | 0.954584401            |
| KMeans      | No Data Processing | 4                  | 0.334764594         | 2183.657053              | 1.066615334            |
| KMeans      | No Data Processing | 5                  | 0.328470753         | 2103.36915               | 1.117386034            |
| KMeans      | Normalization       | 3                  | 0.380850058         | 2379.455299              | 0.992412976            |
| KMeans      | Normalization       | 4                  | 0.331213098         | 2247.854376              | 1.062569644            |
| KMeans      | Normalization       | 5                  | 0.328582671         | 2072.797741              | 1.10759907             |
| KMeans      | Transformation      | 3                  | 0.319812195         | 1719.292632              | 1.148595363            |
| KMeans      | Transformation      | 4                  | 0.288844716         | 1580.674324              | 1.200868319            |
| KMeans      | Transformation      | 5                  | 0.316794819         | 1586.193773              | 1.100592042            |
| KMeans      | PCA                 | 3                  | 0.403316424         | 2730.810679              | 0.895921786            |
| KMeans      | PCA                 | 4                  | 0.3563551           | 2419.444635              | 0.995957707            |
| KMeans      | PCA                 | 5                  | 0.33531913          | 2196.893041              | 1.094142492            |
| KMeans      | T+N                 | 3                  | 0.380850058         | 2379.455299              | 0.992412976            |
| KMeans      | T+N                 | 4                  | 0.331213098         | 2247.854376              | 1.062569644            |
| KMeans      | T+N                 | 5                  | 0.328582671         | 2072.797741              | 1.10759907             |
| KMeans      | T+N+PCA             | 3                  | 0.404421248         | 3047.805359              | 0.901334614            |
| KMeans      | T+N+PCA             | 4                  | 0.38053887          | 2827.314966              | 0.918980934            |
| KMeans      | T+N+PCA             | 5                  | 0.346611058         | 2301.772031              | 1.049831074            |


- AgglomerativeClustering 
| Algorithm                | Processing Method | Subcluster Size | Silhouette Score | Calinski-Harabasz Score | Davies-Bouldin Score |
|--------------------------|-------------------|-----------------|------------------|-------------------------|----------------------|
| AgglomerativeClustering  | No Data Processing | 3               | 0.364784491      | 2137.378707             | 0.961195889          |
| AgglomerativeClustering  | No Data Processing | 4               | 0.299089197      | 1942.205498             | 1.138654965          |
| AgglomerativeClustering  | No Data Processing | 5               | 0.27052387       | 1728.564126             | 1.232901166          |
| AgglomerativeClustering  | Normalization     | 3               | 0.365094136      | 2165.058914             | 1.012228579          |
| AgglomerativeClustering  | Normalization     | 4               | 0.308778371      | 2088.136064             | 1.110064554          |
| AgglomerativeClustering  | Normalization     | 5               | 0.291136101      | 1825.342875             | 1.184240968          |
| AgglomerativeClustering  | Transformation   | 3               | 0.304865715      | 1471.127844             | 1.248150845          |
| AgglomerativeClustering  | Transformation   | 4               | 0.261528618      | 1386.615345             | 1.290494779          |
| AgglomerativeClustering  | Transformation   | 5               | 0.278702908      | 1337.510511             | 1.158304493          |
| AgglomerativeClustering  | PCA               | 3               | 0.392416208      | 2548.953949             | 0.893005557          |
| AgglomerativeClustering  | PCA               | 4               | 0.338359781      | 2185.041295             | 0.998441889          |
| AgglomerativeClustering  | PCA               | 5               | 0.270710711      | 1883.537306             | 1.318368322          |
| AgglomerativeClustering  | T+N               | 3               | 0.365094136      | 2165.058914             | 1.012228579          |
| AgglomerativeClustering  | T+N               | 4               | 0.308778371      | 2088.136064             | 1.110064554          |
| AgglomerativeClustering  | T+N               | 5               | 0.291136101      | 1825.342875             | 1.184240968          |
| AgglomerativeClustering  | T+N+PCA           | 3               | 0.396895024      | 2637.801501             | 0.902163801          |
| AgglomerativeClustering  | T+N+PCA           | 4               | 0.321542911      | 2483.118734             | 0.964616078          |
| AgglomerativeClustering  | T+N+PCA           | 5               | 0.293481475      | 1963.23582              | 1.122494395          |

- DBSCAN
|   | Algorithm | Processing Method | Subcluster Size | Silhouette Score | Calinski-Harabasz Score | Davies-Bouldin Score |
|---|-----------|-------------------|-----------------|------------------|-------------------------|----------------------|
| 0 | DBSCAN    | Normalization     | 3               | 0.337472029      | 15.13964381             | 1.562658807          |
| 1 | DBSCAN    | Normalization     | 4               | 0.337472029      | 15.13964381             | 1.562658807          |
| 2 | DBSCAN    | Normalization     | 5               | 0.337472029      | 15.13964381             | 1.562658807          |
| 3 | DBSCAN    | Transformation    | 3               | -0.281026531     | 23.6408169              | 1.326567986          |
| 4 | DBSCAN    | Transformation    | 4               | -0.281026531     | 23.6408169              | 1.326567986          |
| 5 | DBSCAN    | Transformation    | 5               | -0.281026531     | 23.6408169              | 1.326567986          |
| 6 | DBSCAN    | T+N               | 3               | 0.337472029      | 15.13964381             | 1.562658807          |
| 7 | DBSCAN    | T+N               | 4               | 0.337472029      | 15.13964381             | 1.562658807          |
| 8 | DBSCAN    | T+N               | 5               | 0.337472029      | 15.13964381             | 1.562658807          |
| 9 | DBSCAN    | T+N+PCA           | 4               | 0.356993578      | 6.134362636             | 0.894572694          |
|10 | DBSCAN    | T+N+PCA           | 5               | 0.388823668      | 6.684196067             | 0.890813797          |


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
