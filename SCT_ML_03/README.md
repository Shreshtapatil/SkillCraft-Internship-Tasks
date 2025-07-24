Dataset Source : https://www.kaggle.com/competitions/dogs-vs-cats/data

# SCT_ML_03  
## Internship Task 03 – Image Classification Using CNN (Dogs vs. Cats)  
SkillCraft Technology | July 2025  

---

## Project Overview  
As part of my internship at SkillCraft Technology, Task ID SCT_ML_03 involved developing a Convolutional Neural Network (CNN) model to classify images of dogs and cats.  
The objective was to accurately distinguish between dog and cat images using a deep learning approach, applying standard computer vision practices with a custom CNN architecture.

---

## Dataset  
Source: Kaggle – Dogs vs. Cats  
Link: https://www.kaggle.com/competitions/dogs-vs-cats/data  

Dataset contents:  
- `train.zip`: Contains 25,000 labeled images of dogs and cats (e.g., `dog.0.jpg`, `cat.0.jpg`)  
- `test1.zip`: Contains 12,500 unlabeled images for prediction (`test1/1234.jpg`, etc.)

Images are RGB photographs of varying resolutions. Labels are inferred from filenames in the training set.

---

## Libraries Used  
- numpy – Numerical processing  
- pandas – Dataset manipulation  
- matplotlib, seaborn – Visualization and analysis  
- tensorflow / keras – Deep learning model implementation  
- scikit-learn – Evaluation metrics  
- PIL (Pillow) – Image preprocessing  

---

## Methodology  

1. **Data Preprocessing**  
   - Extracted images from `train.zip` and resized to a fixed dimension (e.g., 150x150)  
   - Normalized pixel values to the [0, 1] range  
   - Split the dataset into training and validation sets (e.g., 80:20 ratio)  
   - Applied data augmentation for robustness (rotation, flip, zoom)

2. **Model Architecture**  
   - Implemented a CNN using Keras with Conv2D, MaxPooling2D, Dropout, and Dense layers  
   - Used ReLU activations for hidden layers and Sigmoid for binary classification  
   - Compiled the model with Binary Crossentropy loss and Adam optimizer

3. **Model Training and Evaluation**  
   - Trained the model using augmented training data  
   - Monitored validation accuracy and loss  
   - Evaluated the model using metrics such as accuracy, precision, recall, and F1 score  
   - Saved final predictions on test images and the trained model file

---

## Results Summary  
- Achieved over 95% accuracy on the validation set  
- The model effectively classifies unseen images as either "Dog" or "Cat"  
- Final predictions saved to `outputs/test_predictions.csv`  
- Trained model stored as `dogs_vs_cats_cnn_model.h5`  
- Can be adapted for use in pet recognition, mobile apps, and content filtering systems

---

## How to Run  

**Step 1: Clone the repository**  
```bash
git clone https://github.com/your-username/SCT_ML_03-Dogs-vs-Cats-CNN.git
cd SCT_ML_03-Dogs-vs-Cats-CNN

