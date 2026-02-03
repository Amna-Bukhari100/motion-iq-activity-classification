Course: Machine Learning
Assignment 5.4 – Recurrent Neural Network Based Classification 
Deliverable: RNN, LSTM, GRU


Project Overview

This project implements and compares three types of Recurrent Neural Networks 
(Vanilla RNN, LSTM, and GRU) to classify human activities using sensor data 
Unlike the FCNN in 5.3, these models account for the temporal sequence of movements


Prerequisites

- Python 3.x
- Libraries: torch, numpy, pandas, matplotlib, seaborn, sklearn
- Dataset: motioniq_cleaned_dataset.csv


Setup Instructions

- Upload the 'code.ipynb'
- Upload the dataset 'motioniq_cleaned_dataset.csv'
- Run all cells sequentially


Data Preprocessing

- Label Encoding
- Feature Selection
- Standardization
- Sliding Windowing
- Stratified Split: Performed an 80/20 train-test split
- Tensor Conversion


Model Architecture

Recurrent Variants: Implemented and compared Simple RNN, LSTM, and GRU architectures
Layer Design: Each model consists of 1 recurrent layer followed by a Fully Connected output layer
Hidden State: Configured with 64 hidden units across all models
Sequence Processing: Captures temporal dependencies from a 20-step window


Training Configuration

Loss Function: CrossEntropyLoss
Optimizer: Adam optimizer
Learning Rate: Set to 0.001
Epochs: Trained for 30 epochs
Batch Type: Full-batch training


Evaluation Metrics 

For each model, 
- Accuracy 
- F1-score 
- Confusion Matrix 
- Training vs Validation Loss curves 


Files Included

- code.ipynb: Complete training and evaluation logic.
- report.pdf: Analysis of results and model comparison.
- README.txt: This instruction file.


Findings

GRU performed best with the lowest validation loss, proving
more efficient than LSTM and RNN in this case









