# ❓ Interview Questions – K-Means Clustering & Unsupervised Learning






### 1. How does K-Means clustering work?

K-Means is an **unsupervised machine learning algorithm** used to group similar data points into **K clusters**. It works in the following steps:
1. Randomly initialize `K` centroids.
2. Assign each data point to the **nearest centroid** (using Euclidean distance).
3. Recalculate the centroid of each cluster based on the new points.
4. Repeat steps 2 and 3 until the centroids stop changing significantly (i.e., convergence).

---

### 2. What is the Elbow Method?

The Elbow Method is a technique used to **find the optimal number of clusters (K)** in K-Means.
- We calculate **WCSS** (Within-Cluster Sum of Squares) for different K values.
- Plot K vs WCSS.
- Look for the **"elbow point"** — where the rate of WCSS decrease slows down. That point is considered the optimal number of clusters.

---

### 3. What are the limitations of K-Means?

- **Requires predefined K** (number of clusters).
- **Sensitive to outliers** and noise.
- Assumes clusters are **spherical and equally sized**, which may not match real-world data.
- Can get stuck in **local minima** depending on initial centroids.
- Not ideal for **non-linear or irregular shaped clusters**.

---

### 4. How does initialization affect results?

The **initial placement of centroids** can impact the final clusters. Poor initialization can:
- Lead to **different results** on different runs.
- Cause the algorithm to **converge to a suboptimal solution**.

To solve this, KMeans uses the **`k-means++`** initialization method to spread out the starting points and improve consistency.

---

### 5. What is Inertia in K-Means?

Inertia is the **sum of squared distances** between each data point and its assigned cluster centroid.
- It measures how **tight** the clusters are.
- **Lower inertia** means better clustering (data points are closer to their centroids).
- Used as a metric for the **Elbow Method**.

---

### 6. What is Silhouette Score?

Silhouette Score is a metric that evaluates how well each data point fits into its assigned cluster:
- Ranges from **-1 to 1**:
  - **~1** → Point is well-matched to its own cluster and far from others.
  - **0** → On or near the decision boundary between clusters.
  - **Negative** → Possibly misclassified.
- A **higher score** indicates **better-defined clusters**.

---

### 7. How do you choose the right number of clusters?

You can determine the optimal number of clusters using:
- **Elbow Method**: Choose K at the “elbow” of the WCSS plot.
- **Silhouette Score**: Choose the K with the **highest average silhouette score**.
- **Domain knowledge**: Sometimes the number of customer types or categories is known.
- **Trial & error**: Run experiments with different K values.

---

### 8. What’s the difference between clustering and classification?

| Feature         | Clustering                  | Classification             |
|------------------|-----------------------------|-----------------------------|
| Type             | Unsupervised learning       | Supervised learning         |
| Input Data       | No labeled output           | Has labeled output (target) |
| Goal             | Group similar data          | Predict categories/labels   |
| Example          | Segmenting customers        | Predicting spam vs not spam |

---

