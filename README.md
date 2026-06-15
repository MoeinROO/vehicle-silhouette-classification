# vehicle-silhouette-classification
Multi-class classification of vehicle types using SVM, KNN, and Logistic Regression. Features class balancing with SMOTE and Hyperparameter tuning via GridSearchCV.

Vehicle Silhouette Multi-class Classification
This project aims to classify vehicles into four categories (Bus, Van, Saab, Opel) based on their geometric features and silhouettes. It covers a comprehensive machine learning pipeline, from handling imbalanced data to comparing multiple optimized models.

🧐 Problem Statement
The dataset contains 18 geometric features of vehicle silhouettes. The challenge is to accurately distinguish between types that might have similar silhouettes (like Saab and Opel) using various classification algorithms.

🛠 Tech Stack
Language: Python
Libraries: Pandas, Scikit-Learn, imbalanced-learn (SMOTE), Seaborn, Matplotlib

🚀 Key Features & Workflow
1. Exploratory Data Analysis (EDA)
Class Distribution: Analyzed the balance of the four vehicle types using bar plots.
Correlation Analysis: Identified highly correlated features using Seaborn Scatterplots and Heatmaps.
2. Data Preprocessing
Missing Values: Imputed missing values using the mean of each class.
Over-sampling (SMOTE): Addressed class imbalance using Synthetic Minority Over-sampling Technique to improve model fairness.
Scaling: Applied Standardization to ensure features contribute equally to models like SVM and KNN.
3. Model Training & Comparison
I implemented and optimized three different architectures:

Kernel SVM: Tuned C, gamma, and kernel (RBF vs Sigmoid).
K-Nearest Neighbors (KNN): Analyzed overfitting by comparing different K values and tuning via GridSearchCV.
Logistic Regression: Optimized using the newton-cg solver and tuning the regularization strength C.
4. Advanced Analysis
Feature Importance: Used Random Forest to identify the most significant features and analyzed the impact of removing low-importance features on model accuracy.
Model Evaluation: Detailed evaluation using Confusion Matrices and Classification Reports (Precision, Recall, F1-Score).

📊 Results
Best Model: SVM Optimized By GridSearchCV
Key Insight: Successfully reduced misclassification between similar classes (Saab/Opel) through hyperparameter tuning and class balancing.
Created by Moein Roshan

:::
