# 📊 Customer Segmentation using K-Means Clustering

This project uses **K-Means Clustering** (unsupervised learning) to segment customers based on their **Annual Income** and **Spending Score**. The goal is to identify distinct customer groups for targeted business strategies like marketing and personalization.

---

## 🧠 Objective

To perform **unsupervised customer segmentation** using K-Means on the **Mall Customer Segmentation Dataset**, and understand patterns in customer behavior.

---

## 🛠️ Tools & Technologies

- Python 🐍
- Pandas 📊
- Matplotlib & Seaborn 🎨
- Scikit-learn 🤖

---

## 📂 Dataset Info

Used the [Mall Customer Segmentation Data](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python), which contains the following fields:

- **CustomerID**
- **Gender**
- **Age**
- **Annual Income (k$)**
- **Spending Score (1–100)**

---

## 🔍 Steps Performed

### 1️⃣ Load & Visualize Dataset
- Selected features: `Annual Income (k$)` and `Spending Score (1–100)`
- Plotted initial scatter plot to observe customer distribution
  ![image](https://github.com/user-attachments/assets/10143acd-e386-4ecc-8254-a05f71b81e4f)


### 2️⃣ Apply K-Means Clustering
- Used `KMeans` from `sklearn.cluster`
- Initially tried `K=5` based on visual intuition
  ![image](https://github.com/user-attachments/assets/5f5e365f-830f-4094-b104-34f3cc72551a)


### 3️⃣ Elbow Method
- Plotted **WCSS** vs **K (1–10)**
- Found optimal `K=5` using the **"elbow point"**
![image](https://github.com/user-attachments/assets/7bc1efcf-d96b-455d-99e4-5afb65be3111)

### 4️⃣ Visualize Clusters
- Color-coded clusters with `viridis` palette
- Plotted **centroids** with red X markers
![image](https://github.com/user-attachments/assets/f9074e2f-ac67-49ee-a222-b6f2a1a1f99e)

### 5️⃣ Evaluate Clustering
- Used **Silhouette Score** to measure quality → `0.5539` ✅
- Plotted **Silhouette Plot** for detailed cluster analysis
  ![image](https://github.com/user-attachments/assets/2e7a4e79-27cc-474d-89b8-a5e62dc3e3f8)


### 6️⃣ Name & Profile Clusters
Analyzed centroids to assign names:

| Cluster | Annual Income | Spending Score | Segment Name        |
|---------|----------------|----------------|---------------------|
| 0       | Medium         | Medium         | Average Segment     |
| 1       | High           | High           | Premium Customers   |
| 2       | Low            | High           | Target Shoppers     |
| 3       | High           | Low            | Careful Rich        |
| 4       | Low            | Low            | Worried Shoppers    |

### 7️⃣ Final Visualization
- Plotted labeled clusters using **segment names**
- Added **cluster centroids** for clarity
  ![image](https://github.com/user-attachments/assets/c151d9e0-0700-4f06-9d82-f5ecbdb71322)


---

## 📈 Results

- Discovered **5 meaningful customer segments**
- **Silhouette Score = 0.5539** → Strong clustering
- Clear visual and logical segmentation supports business insights

---

## 🧠 What I Learned

- Difference between **supervised** and **unsupervised** learning
- How **K-Means** works (centroid update, inertia)
- Using **Elbow Method** to determine K
- Importance of **Silhouette Score** for evaluation
- How to **profile clusters** using centroids
- Creating clear, business-friendly **data visualizations**

---

## File Description
| 📁 File Name                   | 📘 Description                                                                 |
|-------------------------------|---------------------------------------------------------------------------------|
| `supervised-Unsupervised-model.md` | Contains conceptual explanation of **Supervised vs Unsupervised Learning**.          |
| `k-means-Clustering.ipynb`         | Jupyter notebook with **complete step-by-step K-Means implementation**, including visualizations and evaluation. |
| `interview-questions.md`           | A list of **interview questions** related to clustering, K-Means, and unsupervised learning. |
| `Mall_Customers.csv`               | The **dataset** used for customer segmentation (Annual Income, Spending Score, etc.). |
| `README.md`                        | The **main documentation** of the project containing objective, tools, visuals, results, and insights. |
---

## 🧑‍💻 Author

**Niyati Thacker**  
_Data Science Enthusiast | 3rd Year B.Tech CSE Student_

