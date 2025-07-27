
# Breast Cancer Prediction using Machine Learning
  (Based on Wisconsin Original Dataset)

# Introduction
Breast cancer is one of the most common forms of cancer among women.
Early detection significantly increases the chances of successful treatment and survival.
In this project, machine learning algorithms are used to predict whether a tumor is benign (non-cancerous) or malignant (cancerous) using the Breast Cancer Wisconsin (Original) dataset.

# Dataset
The dataset is taken from the UCI Machine Learning Repository.
It contains 699 samples with 9 numeric features describing cell characteristics such as:

• Clump Thickness
• Uniformity of Cell Size
• Uniformity of Cell Shape
• Marginal Adhesion
• Bare Nuclei, etc.
• The target variable (Class) has two values:
• 2 → Benign (converted to 0)
• 4 → Malignant (converted to 1)

# Data Preprocessing
The class label was encoded as 0 (benign) and 1 (malignant).
All features were standardized using StandardScaler.

# Data Splitting & SMOTE
Dataset was split into 70% training and 30% testing.
The dataset was imbalanced (more benign cases), so SMOTE (Synthetic Minority Over-sampling Technique) was used on the training set to balance the classes.

# Models Used
We trained the following six machine learning models:
1. Decision Tree
2. Random Forest
3. Logistic Regression
4. Naive Bayes
5. Support Vector Classifier (SVC)

# Model Evaluation
Each model was evaluated using:
Accuracy
Precision
Recall
F1-Score
Confusion Matrix

Additionally, 10-fold cross-validation was performed using Random Forest for better generalization results.

# Visualization & Analysis
 Accuracy Bar Chart: Compared the accuracy of all five models.
 Correlation Heatmap: Showed relationships between features.
 Feature Importance (Random Forest): Identified the most impactful features.
 Confusion Matrix: Visual summary of prediction results for Random Forest.

# Results Summary
Random Forest achieved the highest accuracy among all models.
Models SVC also performed well.
Using SMOTE improved prediction for malignant cases.

