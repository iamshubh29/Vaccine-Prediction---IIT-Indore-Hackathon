# Vaccine Prediction Model

## 📝 Overview
This project predicts the likelihood of individuals receiving **H1N1** and **seasonal flu** vaccines using machine learning models. The dataset includes demographic, health, and behavioral information, enabling us to analyze vaccination trends and build predictive models.

---

## 📂 Dataset Description
The dataset consists of three key files:
1. **Training Set Features**: Contains demographic, medical history, and behavioral data.
2. **Training Set Labels**: Includes target labels for H1N1 and seasonal flu vaccinations.
3. **Test Set Features**: Used for making predictions, similar to the training set but without labels.

### 🔑 Key Features
- **Demographics**: Age, gender, race, education level.
- **Health-related Factors**: Chronic conditions, doctor visits, general health status.
- **Behavioral Aspects**: Trust in medical institutions, awareness of vaccines.

---

## 📊 Model Performance Comparison

| Model                        | H1N1 Vaccine Accuracy | Seasonal Vaccine Accuracy |
|------------------------------|----------------------|--------------------------|
| 🎯 **XGBoost**               | **0.9000**          | **0.7958**               |
| 🔍 Logistic Regression       | 0.8392              | 0.7877                   |
| 🔎 K-Nearest Neighbors       | 0.8152              | 0.7258                   |
| 🏆 Support Vector Machine    | 0.8353              | 0.7849                   |
| 🧠 Convolutional Neural Net  | 0.8326              | 0.7847                   |
| 🔬 Artificial Neural Network | 0.5936              | 0.7042                   |
| 📊 K-Means Clustering        | 0.3690              | 0.3497                   |

✔ **Best Model:** XGBoost 🚀 (Highest accuracy for both vaccines)

---

## ⚙️ Techniques Used

### 1️⃣ Data Preprocessing
✔ Handled missing values using imputation techniques.
✔ Encoded categorical features into numerical values.
✔ Standardized numerical data for better model performance.

### 2️⃣ Feature Engineering
✔ Created interaction features to boost accuracy.
✔ Removed irrelevant or highly correlated features to avoid overfitting.

### 3️⃣ Model Selection & Training
✔ Evaluated multiple ML models: **XGBoost, Logistic Regression, KNN, SVM, CNN, ANN, K-Means**.
✔ Optimized performance with **hyperparameter tuning**.

### 4️⃣ Evaluation Metrics
✔ **Accuracy** was the primary metric for comparison.
✔ **Cross-validation** ensured better generalization.

---

## 🚀 How to Use

### 🔧 Installation
```sh
pip install -r requirements.txt
```

### 🏋️‍♂️ Train the Model
```sh
python train.py
```

### 🔍 Generate Predictions
```sh
python predict.py
```

### 📂 Output
Final predictions are saved in:
```sh
xgboost_predictions.csv
```

---

## 🎯 Conclusion
**XGBoost** provides the best results and is recommended for deployment due to its **high accuracy, robustness, and efficiency** in handling structured data. This model can be used in real-world applications to predict vaccination trends effectively. ✅

---


## Results
Final predictions are saved in `xgboost_predictions.csv`.

## Conclusion
XGBoost provides the best results and is recommended for deployment due to its high accuracy and robustness in handling structured data.

