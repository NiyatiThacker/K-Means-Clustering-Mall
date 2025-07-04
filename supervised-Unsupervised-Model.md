# **🔷 Supervised Learning**

- 🧠 What:

Supervised learning is a type of machine learning where the model is trained on labeled data — that means for each input, the correct output is already known.

- 📌 Why:

It’s used when the goal is to predict an outcome or classify data based on past examples.

- ⚙️ How:

The model learns the mapping between input features (X) and the known target/output (y).

- After training, it can predict the output for new, unseen inputs.

**🧪 Examples:**
  - Features (Input)	Label (Output)
  - Email text	Spam or Not Spam
  - Tumor measurements	Malignant or Benign
  - House area, location	House Price (in ₹)

**Common Algorithms:**

- Linear Regression

- Logistic Regression

- Decision Trees

- Support Vector Machines (SVM)

- K-Nearest Neighbors (KNN)

# **🔷 Unsupervised Learning**

- 🧠 What:

Unsupervised learning is a type of machine learning where the model works with unlabeled data — only the input features are available, and there’s no output label.

- 📌 Why:

It is useful when you want the model to find hidden patterns or structures in the data, such as grouping, dimensionality reduction, or anomaly detection.

- ⚙️ How:

The algorithm tries to learn the structure or distribution of data on its own.

No right or wrong answers — it’s about discovering relationships in the data.


**🧪 Examples:**

| Features (Input Only)            | Task                     |
| -------------------------------- | ------------------------ |
| Customer income & spending score | Group similar customers  |
| Web user behavior logs           | Segment website visitors |
| Gene expression data             | Discover gene clusters   |


**Common Algorithms:**

- K-Means Clustering

- Hierarchical Clustering

- DBSCAN

- PCA (for dimensionality reduction)

---

# **Key Difference**

| Aspect            | Supervised Learning       | Unsupervised Learning            |
| ----------------- | ------------------------- | -------------------------------- |
| Data              | Labeled (Input + Output)  | Unlabeled (Only Input)           |
| Goal              | Predict or classify       | Find patterns, group data        |
| Example Task      | Spam detection            | Customer segmentation            |
| Evaluation Metric | Accuracy, Precision, etc. | Silhouette Score, Davies-Bouldin |
