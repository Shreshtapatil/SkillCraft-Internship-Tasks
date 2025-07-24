# 📊 SCT_ML_02  
### Internship Task 02 – K-Means Clustering for Retail Customer Segmentation  
💼 SkillCraft Technology | 📅 July 2025

---

## 🧠 Project Overview
As part of my internship at **SkillCraft Technology**, Task ID **SCT_ML_02** involved implementing a **K-Means Clustering algorithm** to analyze and group **customers of a retail store** based on their **purchase behavior**.  
The goal is to identify distinct customer segments that can help the business understand spending patterns and improve targeted marketing strategies.

---

## 🗂 Dataset
The dataset used is `Mall_Customers.csv`, which includes the following features:

- `CustomerID`: Unique customer identifier  
- `Genre`: Gender  
- `Age`: Age of the customer  
- `Annual Income (k$)`: Customer’s yearly income  
- `Spending Score (1-100)`: Score assigned based on purchasing behavior and habits

---

## 📚 Libraries Used
- `pandas` – Data handling and analysis  
- `numpy` – Numerical operations  
- `matplotlib` – Plotting static graphs  
- `seaborn` – Enhanced data visualization  
- `scikit-learn` – Machine learning (KMeans clustering, preprocessing)

---

## ⚙️ Methodology

- Loaded and cleaned the `Mall_Customers.csv` dataset
- Chose relevant features: **Annual Income** and **Spending Score**
- Scaled features using `StandardScaler` for better clustering performance
- Used the **Elbow Method** to determine the optimal number of clusters
- Applied **KMeans Clustering** (with 5 clusters)
- Labeled and visualized segmented customer groups

---

## 📈 Visualizations

### 📌 Elbow Method  
Identifies the optimal number of clusters by plotting the Within-Cluster Sum of Squares (WCSS):  
![Elbow Plot](https://github.com/user-attachments/assets/a9733b32-92d3-4c38-9ed8-2ed482c8fe34)

---

### 📌 Customer Segmentation  
Clusters of customers based on spending behavior and income:  
![Cluster Plot](https://github.com/user-attachments/assets/25597601-3cae-4d99-a0ac-b01ec06bd62a)

---

## ✅ Results Summary

- Customers successfully grouped into **5 unique clusters**
- Each segment reflects different combinations of income and spending behavior
- Cluster insights can be used to:
  - Target high-value customers
  - Improve store layout and promotions
  - Optimize customer relationship strategies
- Clustered data exported to `clustered_customers.csv`

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/SCT_ML_02-Customer-Segmentation.git
