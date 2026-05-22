# machine-learning-pipeline-for-diabetes-prediction
This project builds a complete machine learning pipeline for diabetes prediction using multiple classification algorithms and advanced optimization techniques. The goal is to accurately classify whether a patient has diabetes based on clinical and demographic features while handling class imbalance and improving generalization performance.
## Project Description

This project builds a complete machine learning pipeline for diabetes prediction using multiple classification algorithms and advanced optimization techniques. The goal is to accurately classify whether a patient has diabetes based on clinical and demographic features while handling class imbalance and improving generalization performance.

### Dataset Features

The dataset includes:

* Age
* BMI
* HbA1c Level
* Blood Glucose Level
* Gender
* Smoking History
* Hypertension
* Heart Disease

---

## Techniques and Technologies Used

### Data Preprocessing

* Duplicate removal
* Domain-based filtering for unrealistic medical values
* Feature scaling using `StandardScaler`
* One-hot encoding for categorical variables
* Train / Validation / Test splitting
* Feature engineering for clinical risk indicators

### Handling Imbalanced Data

Used:

* `SMOTE (Synthetic Minority Oversampling Technique)`

Reason:
The diabetes class distribution was imbalanced, so SMOTE generated synthetic minority-class samples to improve recall and F1-score.

---

## Machine Learning Models Implemented

### Linear Models

* Logistic Regression
* Gaussian Naive Bayes

### Support Vector Machines

* Linear SVM
* RBF Kernel SVM

### Neural Networks

* Multi-Layer Perceptron (MLP)

### Ensemble Models

* Random Forest
* XGBoost

---

## Hyperparameter Optimization

Different tuning strategies were applied:

| Model         | Optimization Method |
| ------------- | ------------------- |
| SVM Linear    | Optuna              |
| SVM RBF       | PSO + GridSearchCV  |
| MLP           | Optuna              |
| Random Forest | Optuna              |
| XGBoost       | Optuna              |

---

## Advanced Concepts Implemented

### Support Vector Machines

Implemented:

* Linear Kernel
* RBF Kernel
* Margin maximization
* Soft-margin classification
* Hyperparameter tuning for `C` and `gamma`

### Particle Swarm Optimization (PSO)

Used to optimize SVM RBF hyperparameters:

* Particle positions
* Global best search
* Local exploration
* Search bounds
* Iterative optimization

### Neural Networks (MLP)

Implemented concepts:

* Hidden layers
* Forward propagation
* Backpropagation
* Weight optimization
* Learning rate tuning
* Regularization using `alpha`
* Early stopping

---

## Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* PR-AUC
* Confusion Matrix

Threshold tuning was also applied to maximize F1-score instead of relying on the default 0.5 threshold.

---

## Visualizations Included

* ROC Curves
* Precision-Recall Curves
* Confusion Matrices
* Learning Curves
* Calibration Curves
* Correlation Heatmaps
* Feature Importance Graphs
* SHAP Explainability Plots

---

## Dimensionality Reduction

Used:

* PCA (Principal Component Analysis)

Purpose:

* Reduce feature dimensionality
* Analyze effect on model performance
* Compare original vs PCA-transformed models

---

## Best Performing Models

Top-performing models achieved high F1-scores and ROC-AUC values, with ensemble methods such as Random Forest and XGBoost showing the strongest overall performance.

Example results:

* Random Forest F1 ≈ 0.79
* XGBoost F1 ≈ 0.79
* MLP F1 ≈ 0.79
* SVM RBF F1 ≈ 0.71
* SVM Linear F1 ≈ 0.71

---

## Libraries and Frameworks Used

### Python Libraries

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`

### Machine Learning

* `scikit-learn`
* `xgboost`
* `imblearn`

### Optimization

* `optuna`
* `pyswarms`

### Explainability

* `shap`

---

## Key ML Concepts Demonstrated

* Classification
* Bias vs Variance Tradeoff
* Overfitting vs Underfitting
* Cross Validation
* Hyperparameter Tuning
* Decision Boundaries
* Kernel Trick
* Backpropagation
* Optimization Algorithms
* Model Calibration
* Feature Engineering
* Imbalanced Learning

---

## Example GitHub Repository Tags

`machine-learning` `diabetes-prediction` `svm` `mlp` `xgboost` `random-forest` `optuna` `pso` `smote` `classification` `python` `data-science` `deep-learning` `feature-engineering`

---

## Short GitHub README Summary

This project develops and compares multiple machine learning models for diabetes prediction using advanced preprocessing, feature engineering, imbalance handling, and hyperparameter optimization techniques. The pipeline includes SVMs, MLP neural networks, Random Forest, XGBoost, Optuna optimization, Particle Swarm Optimization (PSO), SMOTE balancing, PCA analysis, threshold tuning, and SHAP explainability. Models were evaluated using F1-score, ROC-AUC, PR-AUC, confusion matrices, and learning curves to identify the most effective classifier for diabetes detection.
