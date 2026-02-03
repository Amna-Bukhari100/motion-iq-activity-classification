# Human Activity Classification System

## Description
A system for classifying human activities using smartphone sensor data. The project combines traditional machine learning and deep learning approaches to predict activities such as walking, sitting, or lying based on accelerometer and gyroscope inputs.

## Features
- Preprocessing and feature engineering of sensor data
- Traditional ML models: Logistic Regression, SVM, Random Forest, XGBoost
- Deep learning models: Fully Connected Neural Network (FCNN)
- Sequential models: Simple RNN, LSTM, GRU
- Performance evaluation using Accuracy and F1-Score

## Dataset
- **Source**: MotionIQ Dataset  
- **Sensor Data**: 3-axial accelerometer and gyroscope  
- **Features**: 561 statistical features per observation (time and frequency domain)  
- **Activities**: Laying, Standing, Sitting, Walking, Walking Upstairs, Walking Downstairs  
- **Train/Test Split**: Stratified 80/20  
- **Sequence Window**: 20 time-steps for recurrent models  

## Results
| Model Type | Model | Accuracy | F1-Score |
|------------|-------|---------|----------|
| Traditional ML | Logistic Regression | 0.985 | 0.985 |
| Traditional ML | SVM | 0.983 | 0.983 |
| Traditional ML | Random Forest | 0.977 | 0.977 |
| Traditional ML | XGBoost | 0.993 | 0.993 |
| Deep Learning | FCNN (3-Layer) | 0.981 | 0.981 |
| Sequential | Simple RNN | 0.812 | 0.804 |
| Sequential | LSTM | 0.841 | 0.832 |
| Sequential | GRU | 0.887 | 0.881 |

## Tech Stack
- Python (NumPy, Pandas, scikit-learn, TensorFlow/Keras)
- Jupyter Notebook

## Notes
- Traditional ML models excel on pre-engineered features.
- GRU performs best for sequential sensor data.
- Recurrent models require higher computational resources and careful windowing.
