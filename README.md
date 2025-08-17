# 🛍️ Mall Customer Segmentation using K-Means

## 📌 Project Overview
This project applies **K-Means clustering** to segment mall customers based on their demographics and spending behavior.  
The goal is to help the mall management understand different customer groups, enabling **targeted marketing strategies**.

---

## 📂 Dataset
- **Source:** Mall Customers dataset  
- **Features:**
  - `CustomerID` → Unique ID of each customer
  - `Gender` → Male/Female
  - `Age` → Age of customer
  - `Annual Income (k$)` → Income of the customer in thousand dollars
  - `Spending Score (1-100)` → Score assigned by the mall based on customer spending patterns

---

## ⚙️ Steps Performed
1. **Data Loading & Exploration**
   - Imported dataset, checked missing values, distributions.
   - Visualized using histograms, scatter plots, and pairplots.

2. **Feature Selection & Preprocessing**
   - Selected key features (`Age`, `Annual Income`, `Spending Score`).
   - Applied scaling where necessary.

3. **K-Means Clustering**
   - Implemented the **Elbow Method** to determine optimal clusters.
   - Chose **K = 5** as the best fit.

4. **Cluster Evaluation**
   - Calculated **Silhouette Score** to validate clustering quality.
   - Achieved score: **0.38** (indicating reasonable cluster separation).

5. **Visualization**
   - Used scatter plots with PCA/2D reduction to visualize clusters.
   - Color-coded customers by their cluster labels.

---

## 📊 Cluster Profile Insights
Based on the K-Means results, the customer segments are:

1. **Cluster 0 – High Income, Low Spending**
   - Customers with high annual income but low spending scores.
   - Likely **savers** or **price-conscious** shoppers.

2. **Cluster 1 – Young, Low Income, High Spending**
   - Customers with low annual income but high spending scores.
   - Likely **impulsive spenders** or **students/youth**.

3. **Cluster 2 – High Income, High Spending**
   - Customers with both high income and high spending scores.
   - Represent the **premium / loyal customers**.

4. **Cluster 3 – Average Income, Average Spending**
   - Middle-income customers with moderate spending.
   - Represent **general mall visitors**.

5. **Cluster 4 – Low Income, Low Spending**
   - Customers with low annual income and low spending scores.
   - Represent **budget-conscious** customers.

---

## 🏆 Key Learnings
- K-Means is effective for segmenting mall customers into meaningful groups.
- **Cluster insights** can help businesses design **targeted campaigns**, e.g.:
  - Discounts for savers.
  - Exclusive offers for premium spenders.
  - Student-focused promotions.

---

## 🚀 Technologies Used
- Python 🐍
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 📈 Next Steps
- Apply **Hierarchical Clustering** for comparison.
- Experiment with **DBSCAN** to detect outliers.
- Deploy as a **dashboard (Streamlit/Flask)** for mall managers.

---
