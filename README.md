# Predictive Analytics for CKD among Bangladeshi Diabetic Patients:A Comparative Machine Learning Study of Clinical and Lifestyle Predictors


Code repository for the EMBA thesis:

**"Predictive Analytics for Chronic Kidney Disease among Bangladeshi Diabetic Patients: A Comparative Machine Learning Study of Clinical and Lifestyle Predictors"**

**Author:** Gazi Ahnaf Tahmid
**Student ID:** 6240505027
**Program:** EMBA in Management Information Systems
**Institution:** University of Dhaka


## Contents

| File | Description |
|---|---|
| `PREPROCESSING_CODE.ipynb` | Data preprocessing pipeline (patient-level collapse, feature engineering) |
| `LOGISTIC_REGRESSION_CODE.ipynb` | Logistic Regression classifier |
| `KNN_CODE.ipynb` | K-Nearest Neighbors classifier (K=7) |
| `SVM_CODE.ipynb` | Support Vector Machine classifier (RBF kernel) |
| `RANDOM_FOREST_CODE.ipynb` | Random Forest classifier (500 trees) |
| `XGBOOST_CODE.ipynb` | XGBoost classifier |
| `CATBOOST_CODE.ipynb` | CatBoost classifier |
| `PRINCIPAL_COMPONENT_ANALYSIS(PCA)_CODE.ipynb` | PCA on the full longitudinal dataset |
| `TREND_ANALYSIS_CODE.ipynb` | Longitudinal trend analysis over diabetic years |

## Dataset
Mendeley Data — DOI: 10.17632/hjkzgbxgv5.2
"A Dataset on Demographic and Lifestyle Factors for Prognosticating Chronic Kidney Disease Progression in Diabetic Patients"

## Environment
All codes were executed in Google Colab with Python 3.
Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `catboost`.

## Note on Data Leakage Prevention
- `Patient ID` was dropped from all features to prevent target leakage.
- `Average Age` and `Average Weight` were excluded as they aggregate information across all years.
- Feature scaling was fit only on the training set and applied to the test set.

## Contact
For questions regarding this code, please contact the author.
