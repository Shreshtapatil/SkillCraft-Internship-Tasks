# 🧠 Sign Language Recognition using Machine Learning (KNN)

**Internship Task:** SCT_ML_04  
**Organization:** SkillCraft Technology  
**Duration:** July 2025  
**Role:** Data Science Intern  
**Project Domain:** Image Classification | Supervised Learning  

---

## 📌 Objective

To develop a machine learning model that accurately recognizes American Sign Language (ASL) alphabets (A–Z excluding dynamic gestures) from grayscale image data. The goal is to enhance gesture-based human-computer interaction, especially for differently-abled individuals.

---

## 📊 Dataset Overview

- **Dataset:** Sign Language MNIST  
- **Source:** [Kaggle – Sign Language MNIST](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)  
- **Format:** Flattened 28×28 grayscale images  
- **Classes:** 0–25 representing A–Z (excluding J and Z)  
- **Training Samples:** 27,455  
- **Testing Samples:** 7,172  

Each row in the CSV corresponds to a single hand gesture represented as pixel values and a label.

---

## 🧰 Technologies & Tools Used

- **Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` – Data Handling  
  - `matplotlib`, `seaborn` – Visualization  
  - `scikit-learn` – Machine Learning  
- **Environment:** Jupyter Notebook

---

## ⚙️ Methodology

1. **Data Loading:**  
   - Loaded training and testing CSVs from local paths.  
   - Extracted labels and reshaped feature vectors into 28×28 images for visualization.

2. **Preprocessing:**  
   - Normalized pixel values to [0, 1]  
   - Ensured class balance and distribution.

3. **Model Training:**  
   - Algorithm: **K-Nearest Neighbors (KNN)**  
   - Parameter: `n_neighbors = 3`  
   - Trained on the full training dataset.

4. **Evaluation:**  
   - Accuracy, Classification Report, and Confusion Matrix on test data.  
   - Visual validation through predicted image samples.

---

## ✅ Results

- **Test Accuracy:** `94.04%`  
- **Precision & Recall:** High across most classes  
- **Model Type:** Non-parametric and interpretable  

---

## 📊 Output Visualizations

### Confusion Matrix  
Illustrates prediction performance across all sign classes.  
![Confusion Matrix]: <img width="915" height="710" alt="TS-04 CONFUSION MATRIX KNN" src="https://github.com/user-attachments/assets/60843bb4-d157-4408-9524-8012e02373a6" />


---

### Sample Predictions  
Random test images with actual and predicted labels to visually inspect accuracy.  
![Sample Predictions]: <img width="823" height="777" alt="TS04 - Predicted hand knn" src="https://github.com/user-attachments/assets/378d9402-5da0-4cac-a1f6-b81c67669fce" />




---

## 📁 Project Files

SCT_ML_04/
├── sign_mnist_train.csv
├── sign_mnist_test.csv
├── knn_model_script.py
├── confusion_matrix_knn.png
├── sample_predictions_knn.png
└── README.md

---

## 📌 Conclusion

This project shows that even traditional ML algorithms like KNN can deliver highly accurate results for gesture recognition tasks, given proper preprocessing. While deep learning could further enhance performance, this lightweight solution is interpretable and performs well in real-time or resource-constrained environments.

---

## 🙏 Acknowledgment

Thanks to **SkillCraft Technology** for the internship opportunity and learning experience.  
Dataset: [Kaggle – Sign Language MNIST](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)

---
