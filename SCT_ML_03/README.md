Dataset Source : https://www.kaggle.com/competitions/dogs-vs-cats/data

# 🐶🐱 SCT_ML_03 - Cats vs. Dogs Image Classifier (SVM)

### Internship Task 03 – Cats vs Dogs Image Classifier (SVM)
💼 SkillCraft Technology | 📅 July 2025

🔗 **Dataset Source**: [Kaggle – Dogs vs Cats](https://www.kaggle.com/competitions/dogs-vs-cats/data)

---

## 🧠 Project Overview
This internship task involved developing a **Support Vector Machine (SVM)** model to classify images of **cats and dogs** using supervised learning. The goal was to build an accurate and efficient image classifier leveraging traditional machine learning techniques on real-world image data, focusing on feature engineering (pixel data) and effective classification.

---

## 🗂 Dataset
- **Classes**: `cats`, `dogs`
- Dataset includes thousands of `.jpg` images labeled by class
- Organized for training/testing using a folder-based structure:
    ```
    Your_Dataset_Root_Folder/
    ├── training_set/
    │   ├── cats/
    │   └── dogs/
    └── test_set/
        ├── cats/
        └── dogs/
    ```

---

## 📚 Libraries Used
- `NumPy` – Numerical processing, especially for image data.
- `OpenCV (cv2)` – Efficient image loading, resizing, and grayscale conversion.
- `Matplotlib` – Plotting and visualizing predictions.
- `scikit-learn` – Core library for SVM model (`SVC`), data splitting (`train_test_split`), feature scaling (`StandardScaler`), and evaluation metrics (`accuracy_score`, `classification_report`, `confusion_matrix`).
- `JupyterLab / Jupyter Notebook` – Interactive development environment.

---

## ⚙️ Methodology
- **Image Preprocessing:**
    - Resizing all images to a consistent `64x64` pixels.
    - Converting images to grayscale to simplify feature vectors.
    - Flattening each 2D grayscale image into a 1D feature vector.
- **Data Splitting:** The preprocessed dataset is split into training and validation sets.
- **Feature Scaling:** Pixel intensity values are standardized using `StandardScaler` to ensure optimal SVM performance, as SVMs are sensitive to feature scales.
- **SVM Model:**
    - A Support Vector Classifier (`SVC`) is used.
    - The `Radial Basis Function (RBF)` kernel is chosen for its ability to handle non-linear decision boundaries.
    - Model parameters like `C` (regularization) and `gamma` (kernel coefficient) are set to default (`C=1.0`, `gamma='scale'`).
- **Training & Evaluation:**
    - The SVM model is trained on the scaled training data.
    - Performance is evaluated using accuracy, a classification report, and a confusion matrix on both validation and unseen test data.

---

## 📈 Results Summary
Based on the execution of the provided code on the specified dataset, the SVM model achieved the following performance metrics:

- **Validation Accuracy**: **70.20%**
- **Test Accuracy**: **69.70%**

### Detailed Metrics:

**Validation Set Classification Report:**
Overall accuracy on the validation set was **70.20%**.
- **Cats (Class 0):** Precision: 0.67, Recall: 0.82, F1-score: 0.74
- **Dogs (Class 1):** Precision: 0.75, Recall: 0.57, F1-score: 0.65
- **Macro Average:** Precision: 0.71, Recall: 0.69, F1-score: 0.69
- **Weighted Average:** Precision: 0.71, Recall: 0.70, F1-score: 0.70

          precision    recall  f1-score   support

   Cat       0.67      0.82      0.74       796
   Dog       0.75      0.57      0.65       690
accuracy                           0.70      1486
macro avg       0.71      0.69      0.69      1486
weighted avg       0.71      0.70      0.70      1486



**Test Set Classification Report:**
Overall accuracy on the test set was **69.70%**.
- **Cats (Class 0):** Precision: 0.67, Recall: 0.81, F1-score: 0.73
- **Dogs (Class 1):** Precision: 0.73, Recall: 0.57, F1-score: 0.64
- **Macro Average:** Precision: 0.70, Recall: 0.69, F1-score: 0.69
- **Weighted Average:** Precision: 0.70, Recall: 0.70, F1-score: 0.69

          precision    recall  f1-score   support

   Cat       0.67      0.81      0.73      1000
   Dog       0.73      0.57      0.64      1000
accuracy                           0.70      2000
macro avg       0.70      0.69      0.69      2000
weighted avg       0.70      0.70      0.69      2000



The model demonstrates reasonable performance in distinguishing between cat and dog images, showing consistent accuracy and balanced performance across classes on both validation and unseen test data.

---

## 📸 Visual Results

### 🔹 Sample Predictions (Cat vs Dog Classification)
This section displays individual predictions from the test set, showing the image, its true label, and the model's predicted label. Correct predictions are indicated with green titles, while incorrect ones are in red.

![Sample Prediction: Cat vs Dog Classification using SVM] : <img width="1281" height="681" alt="Ts-03 ctdog Classification Using SVM" src="https://github.com/user-attachments/assets/8da1d17b-ea2a-44f3-b116-3949958d320d" />


---

## ▶️ How to Run

1.  **Clone this repository** (or download the files directly):
    ```bash
    git clone [https://github.com/YourGitHubUsername/YourRepoName.git](https://github.com/YourGitHubUsername/YourRepoName.git)
    cd YourRepoName/SCT_ML_03  # Adjust this path if your code is in a different subfolder
    ```

2.  **Ensure you have the Dataset:** Download the "Dogs vs. Cats" dataset from Kaggle and unzip it. Make sure its structure matches the one described in the [Dataset](#dataset) section.

3.  **Find your Dataset Paths:** Note down the **absolute, full paths** to your `training_set` and `test_set` folders. For example:
    * `C:\Users\shres\Downloads\Skillcarft Tasks\SCT_ML_03\Task-3 DATASET CAT DOG\training_set\training_set`
    * `C:\Users\shres\Downloads\Skillcarft Tasks\SCT_ML_03\Task-3 DATASET CAT DOG\test_set\test_set`

4.  **Set Up Conda Environment:**
    * Open your **Anaconda Prompt (Windows)** or **Terminal (macOS/Linux)**.
    * Deactivate any active environments:
        ```bash
        conda deactivate
        ```
    * Remove any old/conflicting environments (optional but recommended for a clean start):
        ```bash
        conda env remove -n catdog_svm_env # Remove if it exists
        # ... and any other old environments you might have used previously.
        ```
    * Create a new, dedicated environment:
        ```bash
        conda create -n catdog_svm_env python=3.9
        ```
    * Activate the new environment:
        ```bash
        conda activate catdog_svm_env
        ```
        **Verify your prompt now starts with `(catdog_svm_env)`**

5.  **Install Libraries:**
    * With `catdog_svm_env` active, install the necessary packages:
        ```bash
        conda install -y numpy=1.25.2 scipy matplotlib scikit-learn opencv jupyterlab
        ```

6.  **Run the Jupyter Notebook:**
    * From your activated `catdog_svm_env` in the Anaconda Prompt/Terminal, launch Jupyter:
        ```bash
        jupyter lab
        # OR
        # jupyter notebook
        ```
    * In the Jupyter web interface, navigate to the location where you've cloned this repository (or saved the notebook file).
    * Open the notebook file named `SCT_ML_03 Code using SVM.ipynb`.
    * **Crucially, update the `train_dir` and `test_dir` variables in the first code cell of the notebook with your actual dataset paths (e.g., `train_dir = r"C:\Your\Path\To\training_set\training_set"`).** Remember the `r` for Windows paths.
    * Run all cells in the notebook sequentially (from the "Cell" menu, select "Run All").

---

## Contributing
Feel free to fork this repository, open issues, or submit pull requests to improve the project.

## License
This project is open-sourced under the MIT License.
