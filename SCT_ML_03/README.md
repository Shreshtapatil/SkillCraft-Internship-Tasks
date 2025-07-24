Dataset Source : https://www.kaggle.com/competitions/dogs-vs-cats/data

# 🐶🐱 SCT_ML_03  
### Internship Task 03 – Cats vs Dogs Image Classifier (CNN)  
💼 SkillCraft Technology | 📅 July 2025  

🔗 **Dataset Source**: [Kaggle – Dogs vs Cats](https://www.kaggle.com/competitions/dogs-vs-cats/data)

---

## 🧠 Project Overview  
This internship task involved developing a **Convolutional Neural Network (CNN)** to classify images of **cats and dogs** using supervised learning.  
The goal was to build an accurate and efficient image classifier leveraging deep learning techniques on real-world image data.

---

## 🗂 Dataset  
- **Classes**: `cats`, `dogs`  
- Dataset includes thousands of `.jpg` images labeled by class  
- Organized for training/testing using a folder-based structure

---

## 📚 Libraries Used  
- `TensorFlow / Keras` – Model building  
- `NumPy` – Numerical processing  
- `Matplotlib` – Plotting accuracy results  
- `OpenCV` – Image handling  
- `scikit-learn` – Evaluation metrics

---

## ⚙️ Methodology  
- Image preprocessing: resizing, normalization, augmentation  
- CNN architecture:
  - Multiple Conv2D + MaxPooling layers  
  - Followed by Flatten → Dense → Dropout → Output  
- Compiled with `categorical_crossentropy` & `Adam` optimizer  
- Trained for 15 epochs with validation split  
- Final testing on new/unseen images

---

## 📈 Results Summary  
- **Training Accuracy**: ~92%  
- **Validation Accuracy**: ~89%  
- **Test Accuracy**: ~88%  
- Model performed well in real-world prediction scenarios

---

## 📸 Visual Results

### 🔹 Accuracy Graph  
![Training & Validation Accuracy]: <img width="959" height="360" alt="Ts-3 accuracy" src="https://github.com/user-attachments/assets/2723c03f-9132-4c80-97bf-c5a6a954fd55" />


### 🔹 Cat vs Dog Classification  
![Sample Prediction]: <img width="940" height="269" alt="Ts-3 catdog classification" src="https://github.com/user-attachments/assets/a9d4ed0b-82d6-4e66-8547-91bf2a3e8815" />


> ✅ Model successfully predicted cat and dog images with high confidence

---

## ▶️ How to Run

1. Clone this repository:  
   ```bash
   git clone https://github.com/Shreshtapatil/SkillCraft-Internship-Tasks.git
   cd SkillCraft-Internship-Tasks/SCT_ML_03
