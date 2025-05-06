# Task7-cancer-detection-svm
# Breast Cancer Detection using Support Vector Machine (SVM)

This project was completed as part of the AI & ML Internship Task 7. The goal is to classify breast cancer tumors as benign or malignant using Support Vector Machines with different kernel types.

---

## Objective
Learn how to:
- Implement SVM with different kernels (Linear and RBF)
- Scale numerical features
- Perform hyperparameter tuning using GridSearchCV
- Visualize decision boundaries using PCA

---

## Dataset
We used the [Breast Cancer Wisconsin Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)), provided as `Cancer_Data.csv`.

---

## Tools & Libraries
- **Python**
- **Pandas** & **NumPy** for data manipulation
- **Matplotlib & Seaborn** for visualization
- **Scikit-learn** for SVM, scaling, splitting, evaluation, and tuning

---

## Steps Performed

### 1. Imported Dataset
Loaded the dataset, dropped irrelevant columns (`id`, `Unnamed: 32`), and verified no null values were present.

### 2. Preprocessed Data
- Encoded the target variable `diagnosis` (Benign=0, Malignant=1)
- Scaled all numerical features using `StandardScaler`

### 3. Trained Models
- Implemented **SVM with Linear Kernel**
- Implemented **SVM with RBF Kernel**

### 4. Evaluated Models
- Used `confusion_matrix` and `classification_report` to evaluate both models
- Compared accuracy and precision for both kernels

### 5. Hyperparameter Tuning
- Tuned `C` and `gamma` values using `GridSearchCV` for the RBF kernel
- Achieved improved accuracy with the best parameters

### 6. Visualized Results
- Used PCA to reduce features to 2D
- Plotted decision boundaries using a 2D SVM model

---

## Visualizations Included
- PCA scatter plot with SVM decision boundary
- Confusion matrix heatmaps

---

## Final Outcome
Successfully built and optimized SVM classifiers to detect breast cancer with high accuracy using both linear and non-linear kernels.
