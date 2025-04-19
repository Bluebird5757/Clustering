# 📊 Clustering Assignment: Comparative Analysis of Clustering Algorithms

This project performs a **comparative performance study of clustering algorithms** using various **pre-processing techniques**, **cluster counts**, and **evaluation metrics**.

---

## 📌 Objective

To analyze and compare the performance of different clustering algorithms using:

- Multiple **data preprocessing techniques**
- Varying number of clusters (`k = 3, 4, 5`)
- Multiple **evaluation parameters**:
  - Silhouette Score
  - Calinski-Harabasz Index
  - Davies-Bouldin Index

---

## 📚 Dataset

- Sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/).
- (Replace with the dataset name you used, e.g., **Iris**, **Wine**, etc.)
- Number of rows: **`XXX`**
- Number of features: **`YYY`**

---

## 🛠️ Clustering Techniques Used

1. **K-Means Clustering**
2. **Hierarchical Clustering**
3. **Mean Shift Clustering**

---

## ⚙️ Preprocessing Techniques

- No Data Processing
- Normalization
- Data Transformation (e.g., log)
- PCA (Dimensionality Reduction)
- T+N = Transform + Normalize
- T+N+PCA = Transform + Normalize + PCA

---

## 📈 Evaluation Metrics

| Metric              | Ideal Value     |
|---------------------|------------------|
| Silhouette Score    | Closer to 1       |
| Calinski-Harabasz   | Higher is better |
| Davies-Bouldin      | Lower is better  |

---

## 🧪 Sample Results: K-Means Clustering

| Parameters         | No Processing (c=3) | Normalized (c=3) | PCA (c=3) | T+N+PCA (c=3) |
|--------------------|---------------------|-------------------|-----------|---------------|
| Silhouette         | 0.74                | 0.69              | 1.0       | 0.54          |
| Calinski-Harabasz  | 3567                | 6633              | 5294      | 1119          |
| Davies-Bouldin     | 0.34                | 0.59              | 0.41      | 0.62          |

> 📌 Based on metrics, **K-Means with PCA** and **Normalization** show the best overall performance.

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**
2. Install required libraries if not pre-installed:
   ```python
   !pip install scikit-learn pandas matplotlib seaborn
