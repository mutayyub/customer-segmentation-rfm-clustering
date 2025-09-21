# Who Are Your Best Customers?

## RFM Segmentation with Clustering

This project applies **RFM (Recency, Frequency, Monetary) analysis** and **K-Means clustering** on the [Online Retail II dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II) to segment customers into meaningful groups. The goal is to uncover **high-value, mid-value, and low-value customers** to help businesses improve **marketing, targeting, and retention strategies**.

---

## Objectives

* Preprocess the dataset.
* Perform **RFM analysis** to quantify customer behavior.
* Use **K-Means clustering** to segment customers into groups.
* Visualize clusters with PCA and interactive bubble charts.

---

## Dataset

* **Name:** Online Retail II
* **Content:** Transactions from a UK-based online retail store between 2009–2011.
* **Key features used:**

  * **Recency** → Days since last purchase
  * **Frequency** → Number of purchases
  * **Monetary** → Total spend

---

## Methodology

1. **Data Cleaning & Preprocessing**

   * Removed missing values & irrelevant rows (e.g., test products).
   * Handled outliers and duplicates.
   * Created RFM features.

2. **Feature Scaling**

   * Applied StandardScaler for balanced clustering.

3. **Clustering**

   * Applied K-Means with `k=3`.
   * Evaluated with **Silhouette Score**.

4. **Dimensionality Reduction**

   * PCA (2D) for cluster visualization.

5. **Visualization**

   * PCA scatter plot with cluster colors.
   * Bubble chart (Recency vs Frequency, bubble size = Monetary).

---

## 🔍 Results & Insights

* **Cluster 0 – Low Value Customers**

  * Purchased long ago, low frequency, low spend.

* **Cluster 1 – Mid Value Customers**

  * Recent purchases, moderate frequency, average spend.

* **Cluster 2 – High Value Customers (includes wholesalers)**

  * Very frequent, very recent, extremely high spend.

📌 Businesses should focus on **retaining high-value customers**, re-engaging **mid-value customers**, and running win-back campaigns for **low-value customers**.

---

## 📈 Visualizations

* **PCA 2D Plot** showing customer segments.
* **Interactive Bubble Chart** for identifying bulk buyers.

---
