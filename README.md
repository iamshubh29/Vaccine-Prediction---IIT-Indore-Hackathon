#  Vaccine Prediction Model

## Overview
This project aims to predict the likelihood of individuals receiving H1N1 and Seasonal Vaccines using various machine learning models.

## Model Comparison

| Model                   | H1N1 Vaccine Accuracy | Seasonal Vaccine Accuracy |
|-------------------------|----------------------|---------------------------|
| XGBoost                | **0.9000**           | **0.7958**                 |
| Logistic Regression     | 0.8392               | 0.7877                     |
| K-Nearest Neighbors    | 0.8152               | 0.7258                     |
| Support Vector Machine | 0.8353               | 0.7849                     |
| Convolutional Neural Network | 0.8326       | 0.7847                     |
| Artificial Neural Network | 0.5936           | 0.7042                     |
| K-Means Clustering     | 0.3690               | 0.3497                     |

## Best Model Selection
Based on the accuracy comparison, **XGBoost** was chosen as the final model due to its superior performance in predicting both H1N1 and Seasonal Vaccine adoption.

## Usage
1. Install dependencies: `pip install -r requirements.txt`
2. Run the training script: `python train.py`
3. Generate predictions: `python predict.py`

## Results
Final predictions are saved in `xgboost_predictions.csv`.

## Conclusion
XGBoost provides the best results and is recommended for deployment.



