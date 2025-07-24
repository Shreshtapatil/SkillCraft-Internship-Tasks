# SCT_ML_01  
**Internship Task 01 – House Price Prediction using Linear Regression**  
💼 SkillCraft Technology | 📅 July 2025

---

## 🏡 House Price Prediction using Linear Regression

This project is part of my internship with **SkillCraft Technology** under the Task ID `SCT_ML_01`. It predicts house sale prices based on features like land area, living area, number of bedrooms, and more using a **Linear Regression model**.

---

## 📚 Libraries Used

- `pandas` – for data manipulation  
- `numpy` – for numerical computations  
- `matplotlib` – for plotting graphs  
- `scikit-learn` – for machine learning algorithms  

---

## 🗂 Dataset

The dataset used was synthetically generated to reflect realistic housing data. It includes:

- `LotArea`: Size of the lot  
- `GrLivArea`: Above-ground living area  
- `OverallQual`: Overall material quality  
- `GarageArea`: Garage size in sq. ft.  
- `Bedroom`: Number of bedrooms  
- `YearBuilt`: Year the house was built  
- `SalePrice`: The target value (price)  

---

## 🧠 Model Used

- Linear Regression (from scikit-learn)  
- Dataset scaled using `StandardScaler`  
- Data split into 80% training and 20% testing  

---

## 📊 Evaluation Metrics

| Metric              | Value (example) |
|---------------------|-----------------|
| Mean Squared Error  | 12,345,678.90   |
| R² Score            | 0.88            |

---

## 📈 Visualizations

### 📌 Actual vs Predicted Prices  
<img src="https://github.com/user-attachments/assets/ae4b7199-fdad-45b7-a569-1950676f240d" width="600"/>

### 📌 Residuals vs Predicted  
<img src="https://github.com/user-attachments/assets/b3c7da95-04d8-496b-856c-bd026b9aa86f" width="600"/>

---

## ✅ Results Summary

- The model performed well with a high R² Score  
- Data was scaled properly  
- Plots indicate good prediction distribution  
- Demonstrates the use of linear regression in real-world pricing models  

---

## ▶️ How to Run

1. Clone this repository  
2. Install required libraries:  
   ```bash
   pip install pandas numpy matplotlib scikit-learn

