Assignment 5.3 – Fully Connected Neural Network Approach
Course: Machine Learning
Deliverable: FCNN / MLP for Classification


Project Overview

This project implements a Fully Connected Neural Network (FCNN), also known as a
Multi-Layer Perceptron (MLP), for multi-class activity classification using the
MotionIQ dataset. The model is developed using PyTorch and evaluated using
standard classification metrics.


Dataset

Dataset: motioniq_cleaned_dataset.csv

Preprocessing Steps:
- Removed rare activity classes to enable stratified splitting
- Dropped irrelevant columns (subject, activity_id, timestamps)
- Label encoded target variable (activity)
- Standardized numerical features using StandardScaler
- Performed stratified train-test split (80% training, 20% testing)


Model Architecture

- Fully Connected Neural Network (FCNN)
- 3 Hidden Layers:
  - 512 neurons (ReLU)
  - 256 neurons (ReLU)
  - 128 neurons (ReLU)
- Dropout (0.2) for regularization
- Output Layer:
  - Number of neurons equal to number of classes
  - Softmax implicitly applied via CrossEntropyLoss


Training Configuration

- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Learning Rate: 0.001
- Epochs: 50
- Batch Type: Full-batch training


Evaluation Metrics

- Accuracy
- Weighted F1-Score
- Confusion Matrix
- Training vs Validation Loss Curves


Files Included

- code.ipynb        → Full FCNN implementation
- README.txt        → Project documentation
- report.pdf        → Detailed analysis and discussion


How to Run

1. Ensure required libraries are installed:
   pandas, numpy, matplotlib, seaborn, scikit-learn, torch
2. Place motioniq_cleaned_dataset.csv in the same directory
3. Run code.ipynb cell-by-cell


Notes

Softmax is not explicitly applied in the output layer because PyTorch's
CrossEntropyLoss internally applies LogSoftmax, which is standard practice
for multi-class classification.
