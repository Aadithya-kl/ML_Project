# Student Performance Prediction Using Machine Learning

## Project Overview

This project focuses on predicting **student academic performance** using multiple **machine learning regression models**.
The target variable is the **final grade (G3)**, predicted using academic, demographic, family, and lifestyle-related features.

The objective is to **analyze, compare, and optimize different regression models** through **systematic preprocessing and hyperparameter tuning**, and identify the most effective model for accurate grade prediction.

---

## Problem Statement

Student performance is influenced by a wide range of factors such as:

* Previous academic scores
* Family background
* Study habits
* Social and lifestyle attributes

Accurately predicting final performance can help educational institutions:

* Identify at-risk students early
* Design targeted academic interventions
* Improve overall learning outcomes

This project addresses the question:

**Which machine learning regression model best predicts student performance, and how much improvement can be achieved through hyperparameter tuning?**

---

## Dataset Description

* Dataset: Student Performance Dataset (student-mat.csv)
* Total samples: 395
* Total features: 33
* Target variable: Final grade (G3)
* No missing values

The dataset contains a mix of **numerical and categorical features**, including:

* Academic scores (G1, G2)
* Family background
* Study time and failures
* Health, absences, and lifestyle indicators

---

## Data Preprocessing

* Categorical features converted to numerical values using **Label Encoding**
* Feature scaling performed using **StandardScaler**
* Dataset split into training and testing sets (80:20 split)
* Exploratory analysis performed using:

  * Correlation matrix
  * Scatter matrix visualization

---

## Models Implemented

The following regression models were implemented and evaluated:

1. Linear Regression
2. Support Vector Regression (RBF Kernel)
3. Random Forest Regressor
4. AdaBoost Regressor
5. Gradient Boosting Regressor
6. Decision Tree Regressor

---

## Hyperparameter Tuning

To improve model performance, extensive tuning was performed using:

* GridSearchCV
* RandomizedSearchCV

Key tuned parameters included:

* Regularization strength and kernel parameters (SVR)
* Number of estimators, depth, and feature selection (Tree-based models)
* Learning rate and ensemble size (Boosting models)

---

## Evaluation Metric

* **R² Score** was used as the primary evaluation metric
* Higher R² indicates better explanatory power and prediction accuracy

---

## Performance Summary

| Model                       | R² Score |
| --------------------------- | -------- |
| Linear Regression           | 0.75     |
| SVR (RBF Kernel)            | 0.79     |
| Random Forest Regressor     | 0.83     |
| AdaBoost Regressor          | 0.83     |
| Gradient Boosting Regressor | 0.81     |
| Decision Tree Regressor     | **0.85** |

**Best performing model:** Decision Tree Regressor (after hyperparameter tuning)

---

## Key Observations

* Ensemble methods consistently outperformed simple linear models
* Hyperparameter tuning significantly improved model performance
* Decision Tree and ensemble-based models captured non-linear relationships effectively
* Feature scaling played a critical role in SVR performance

---

## Visual Analysis

The project includes:

* Correlation and scatter matrix visualizations for feature relationships
* Bar chart comparison of R² scores across all models

These visualizations help interpret both feature influence and model effectiveness.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

---

## Conclusion

This project demonstrates how **model selection, preprocessing, and hyperparameter tuning** can dramatically influence regression performance.
Tree-based and ensemble models proved to be the most effective for predicting student academic outcomes in this dataset.

---

## Future Enhancements

* Feature importance analysis
* Cross-dataset validation
* Neural network-based regression
* Model interpretability using SHAP or LIME

---

## Author

**Aadithya K L**

This project emphasizes understanding model behavior and performance trade-offs rather than relying on default configurations.
