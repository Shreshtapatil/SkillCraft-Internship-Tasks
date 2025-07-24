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
<img width="794" height="536" alt="TS-1 Actual vs Predicted" src="https://github.com/user-attachments/assets/ce9776af-8fb3-4ad9-95f4-9bcd04e41de9" />

### 📌 Residuals vs Predicted  
<img width="1156" height="743" alt="TS-1 Predicated vs actual" src="https://github.com/user-attachments/assets/eb21d2b5-c584-4366-941c-ebd9c0cb5679" />


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

