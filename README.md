# Clustering Analysis with Wine Dataset

This repo compares KMeans, Hierarchical Clustering, and MeanShift on the Wine dataset using six preprocessing techniques.

## Preprocessing Techniques
1. No Processing  
2. Normalized  
3. Transformed  
4. PCA  
5. T+N (Transformed + Normalized)  
6. T+N+PCA  

## Results

### KMeans Clustering

#### Silhouette Score  
![KMeans Silhouette]( images/kmeans.png)

#### Calinski–Harabasz Score  
![KMeans Calinski-Harabasz](images/kmeans-c.png)

#### Davies–Bouldin Score  
![KMeans Davies-Bouldin](images/kmeansdavid.png)

**Observation:** Best separation and compactness with PCA or T+N+PCA.

---

### Hierarchical Clustering

#### Silhouette Score  
![Hierarchical Silhouette](images/hierarchicalsilhouette.png)

#### Calinski–Harabasz Score  
![Hierarchical Calinski-Harabasz](images/hierarchicalcalinski.png)

#### Davies–Bouldin Score  
![Hierarchical Davies-Bouldin](images/hierarchicaldavid.png)

**Observation:** Stable overall but higher Davies–Bouldin with raw/transformed data.

---

### MeanShift Clustering

#### Silhouette Score  
![MeanShift Silhouette](images/meanshift.png)

#### Calinski–Harabasz Score  
![MeanShift Calinski-Harabasz](images/meanshiftcalinski.png)

#### Davies–Bouldin Score  
![MeanShift Davies-Bouldin](images/meansshiftdavies.png)

**Observation:** Consistent across preprocessings; benefits from normalization and PCA.

---

### Best Clustering Configuration Based on TOPSIS
**Algorithm:** kmeans
**Preprocessing:** PCA
**Number of Clusters:** 5
**TOPSIS Score:** 0.9662
