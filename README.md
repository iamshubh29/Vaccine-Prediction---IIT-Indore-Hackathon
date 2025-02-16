# Vaccine Prediction Model

## Overview
This project aims to predict the likelihood of individuals receiving H1N1 and seasonal flu vaccines using machine learning techniques. The dataset contains demographic, health, and behavioral information, which helps build predictive models for vaccination trends.

## Dataset Description
The dataset consists of three files:
1. **Training Set Features:** Contains various features about individuals, such as demographics, medical history, and behaviors.
2. **Training Set Labels:** Includes the target labels indicating whether a person has taken the H1N1 and seasonal flu vaccines.
3. **Test Set Features:** Contains similar data as the training set without labels, used for making predictions.

### Key Features
- **Demographics:** Age, gender, race, and education level.
- **Health-related Factors:** Chronic conditions, doctor visits, and general health status.
- **Behavioral Aspects:** Frequency of doctor visits, trust in medical institutions, and awareness of vaccines.

## Model Comparison
| Model                        | H1N1 Vaccine Accuracy | Seasonal Vaccine Accuracy |
| ---------------------------- | --------------------- | ------------------------- |
| XGBoost                      | **0.9000**            | **0.7958**                |
| Logistic Regression          | 0.8392                | 0.7877                    |
| K-Nearest Neighbors          | 0.8152                | 0.7258                    |
| Support Vector Machine       | 0.8353                | 0.7849                    |
| Convolutional Neural Network | 0.8326                | 0.7847                    |
| Artificial Neural Network    | 0.5936                | 0.7042                    |
| K-Means Clustering           | 0.3690                | 0.3497                    |

## Techniques Used
### 1. **Preprocessing**
- Handled missing values using imputation techniques.
- Categorical encoding for non-numeric features.
- Standardization of numerical features.

### 2. **Feature Engineering**
- Created interaction features to improve model performance.
- Removed irrelevant or highly correlated features.

### 3. **Model Selection & Training**
- Evaluated multiple models including XGBoost, Logistic Regression, KNN, SVM, CNN, ANN, and K-Means.
- Used hyperparameter tuning to optimize performance.

### 4. **Evaluation Metrics**
- Accuracy was used as the primary metric for model evaluation.
- Cross-validation was applied to assess generalizability.

## Best Model Selection
Based on accuracy comparison, **XGBoost** was selected as the final model due to its highest performance in predicting both H1N1 and Seasonal Vaccine adoption.

## Usage
1. Install dependencies: `pip install -r requirements.txt`
2. Run the training script: `python train.py`
3. Generate predictions: `python predict.py`

## Results
Final predictions are saved in `xgboost_predictions.csv`.

## Conclusion
XGBoost provides the best results and is recommended for deployment due to its high accuracy and robustness in handling structured data.

