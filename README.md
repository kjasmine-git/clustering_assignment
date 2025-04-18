# clustering_assignment
🔍 Overview
This study aimed to evaluate the impact of various preprocessing techniques on the performance of different clustering algorithms (K-Means, Hierarchical Clustering, and Mean Shift) using three popular evaluation metrics: Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index. The experiments were conducted on a UCI dataset (e.g., Iris dataset) using a range of cluster numbers (c=3, 4, 5) wherever applicable.

📈 Key Observations
Preprocessing Matters:

Preprocessing significantly impacted clustering performance across all algorithms.

The combination of Transformation + Normalization + PCA (T+N+PCA) consistently yielded better Silhouette and Calinski-Harabasz scores, especially with K-Means.

No preprocessing generally resulted in lower performance, indicating the importance of scaling and transformation.

Best Performing Algorithm:

K-Means outperformed other algorithms in most preprocessing scenarios, especially when combined with PCA.

Hierarchical Clustering performed comparably in some cases, particularly with Normalization, but was slightly less consistent.

Mean Shift, although parameter-free, had relatively lower performance and higher Davies-Bouldin scores, indicating less compact and well-separated clusters.

Effect of Cluster Number (c):

For both K-Means and Hierarchical clustering, c=3 gave the highest Silhouette scores in most cases.

Increasing the number of clusters generally led to a decrease in Silhouette Score and increase in Davies-Bouldin Index, suggesting diminishing returns in cluster separation.

🏁 Final Takeaways
Optimal Preprocessing: T+N+PCA led to the most interpretable and high-quality clusters.

Algorithm Choice: K-Means is recommended for balanced performance and interpretability, provided the number of clusters is known.

Evaluation Metrics: Silhouette Score is intuitive, but combining it with Calinski-Harabasz and Davies-Bouldin gives a well-rounded view of cluster quality.

