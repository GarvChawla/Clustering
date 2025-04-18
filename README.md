# Clustering Algorithm Evaluation

This repository includes the comparative analysis of different clustering algorithms using various evaluation metrics. The performance of clustering algorithms, including KMeans, Agglomerative Clustering, DBSCAN, MeanShift, and Gaussian Mixture, has been evaluated using the following metrics:

- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Index**


### Evaluation Tables

Below are the tables displaying the clustering results for each algorithm:

#### 1. **KMeans Clustering** Results

![KMeans Clustering Table](./images/kmeans_table.png)

#### 2. **Agglomerative Clustering** Results

![Agglomerative Clustering Table](./images/agglomerative_table.png)

#### 3. **DBSCAN Clustering** Results

![DBSCAN Clustering Table](./images/dbscan_table.png)

#### 4. **MeanShift Clustering** Results

![MeanShift Clustering Table](./images/meanshift_table.png)

The results are visualized in boxplots, and tables are included for detailed metrics across different cluster counts and preprocessing techniques.

#### 5. **GaussianMixture Clustering** Results

![GaussianMixture Clustering Table](./images/gaussian_mixture_table.png)

## Comparative Boxplots

Below are the comparative boxplots for the clustering algorithms based on the evaluation metrics:

### 1. Silhouette Score across Clustering Algorithms

![Silhouette Score](./images/graph_silhouette.png)

### 2. Calinski-Harabasz Score across Clustering Algorithms

![Calinski-Harabasz Score](./images/graph_calinski_harabasz.png)

### 3. Davies-Bouldin Score across Clustering Algorithms

![Davies-Bouldin Score](./images/graph_davies_bouldin.png)

## Conclusion

From the boxplots, the following inferences can be made:

- **KMeans** and **Agglomerative Clustering** generally perform well across all three metrics, with KMeans showing a slightly better performance in the Silhouette and Calinski-Harabasz scores. These algorithms are reliable for producing well-separated and well-defined clusters.
  
- **DBSCAN** performs well in the Davies-Bouldin score, but its performance on Silhouette and Calinski-Harabasz scores is inconsistent. It struggles to create meaningful clusters in some cases, especially at lower cluster counts.

- **MeanShift** shows poor performance overall, especially in the Calinski-Harabasz and Davies-Bouldin metrics, indicating that it does not form well-separated clusters in most cases.

- **Gaussian Mixture** tends to show moderate performance, with some variation in results depending on the preprocessing method.

