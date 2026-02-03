Project Overview:

This project focuses on classifying human activity using accelerometer data. The workflow includes data preprocessing, feature engineering, model training, evaluation, and comparison across multiple machine learning algorithms.

Files Included:

project.ipynb :full code for preprocessing, feature extraction, model training & evaluation

motioniq_cleaned_dataset.csv : dataset folder (CSV files)

report.pdf :final written report for submission

README.md : project description and usage guide

Feature Engineering:

The following features were created from raw accelerometer signals:

Statistical features: mean, variance, standard deviation

Temporal features: SMA (Signal Magnitude Area), zero-crossing rate

Frequency features: FFT energy, dominant frequency

Machine Learning Models Used:

The project evaluates four supervised learning models:

Logistic Regression

Support Vector Machine (SVM)

Random Forest Classifier

XGBoost Classifier

XGBoost achieved the best performance, with exceptionally high accuracy and ROC-AUC.

->How to Run the Project:

1. Install required libraries
   pip install numpy pandas scikit-learn xgboost matplotlib

2. Open the Notebook
   jupyter notebook project.ipynb

3. Run all cells

This will:

Load & clean the dataset

Extract features

Train all ML models

Print model performance metrics

Show confusion matrices & ROC curves
