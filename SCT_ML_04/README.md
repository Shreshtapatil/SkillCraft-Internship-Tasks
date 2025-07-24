Dataset Source : https://www.kaggle.com/datasets/datamunge/sign-language-mnist

# SCT_DL_04  
**Internship Task 04 – Hand Gesture Recognition using Convolutional Neural Networks (CNN)**  
💼 SkillCraft Technology | 📅 July 2025  

---

## ✋ Hand Gesture Recognition using CNN

This project is part of my internship with **SkillCraft Technology** under the Task ID `SCT_DL_04`.  
The objective was to develop a model that can accurately **identify and classify hand gestures** from images to enable gesture-based human-computer interactions.

Although the original task referenced a different dataset, I used the **Sign Language MNIST** dataset for effective image-based classification of hand gestures.

---

## 📚 Libraries Used

- `pandas` – Data handling and manipulation  
- `numpy` – Numerical operations  
- `matplotlib`, `seaborn` – Visualization  
- `tensorflow.keras` – Model building and training  
- `scikit-learn` – Evaluation metrics  

---

## 🗂 Dataset

I used the **Sign Language MNIST Dataset** available in CSV format:

- 27,455 training images  
- 7,172 testing images  
- 28×28 grayscale images  
- Labels from A–Z (26 classes)

Each image is represented by 784 pixel values and a label column indicating the hand gesture class.

---

## 🧠 CNN Model Architecture

The deep learning model was built using **TensorFlow Keras** with the following architecture:

- `Conv2D(32)` → `ReLU` → `MaxPooling2D`  
- `Conv2D(64)` → `ReLU` → `MaxPooling2D`  
- `Flatten()`  
- `Dense(128)` → `Dropout(0.3)`  
- `Dense(26)` with `Softmax` activation for multi-class classification  

### Compilation:

- **Loss Function**: `categorical_crossentropy`  
- **Optimizer**: `adam`  
- **Metrics**: `accuracy`  
- **Epochs**: 10  
- **Batch Size**: 64  

---

## 🏋️ Training & Testing

- Dataset reshaped to (28, 28, 1) and normalized  
- One-hot encoded labels using `to_categorical()`  
- 10 epochs of training with validation on test set  

---

## 📊 Model Performance

| Metric        | Value        |
|---------------|--------------|
| Test Accuracy | ~94.67%      |
| Test Loss     | ~0.18        |

---

## 📈 Visualizations

### 📌 Accuracy Graph  
Training vs Validation Accuracy  
![Accuracy Plot]:<img width="689" height="515" alt="Ts4 accuracy" src="https://github.com/user-attachments/assets/a92e8aea-32e9-4c42-9ae1-660d2071350d" />



### 📌 Confusion Matrix  
Classification heatmap across 26 classes  
![Confusion Matrix]: <img width="1025" height="773" alt="Ts-4 confusion matrix" src="https://github.com/user-attachments/assets/8dc81039-82a9-4e6e-ab68-d2ef845ec29a" />



---

## ✅ Summary

- The CNN model successfully classified 26 ASL hand gestures  
- Achieved **high accuracy** with minimal loss  
- Demonstrates the power of CNNs in gesture-based recognition tasks  
- The approach can be extended for real-time gesture control in HCI systems  

---

## ▶️ How to Run

1. Clone this repository  
2. Install the required libraries  
   ```bash
   pip install pandas numpy matplotlib seaborn tensorflow scikit-learn
