# 🌧️ Weather Forecasting Project

Welcome to the **Weather Forecasting** project by **Team Semi Colon**. This repository contains a complete pipeline for weather data analysis, preprocessing, and rainfall prediction using both Machine Learning and Deep Learning models.

---

## 📊 Project Overview

The objective of this project is to **predict rainfall** based on daily weather parameters including temperature, humidity, wind speed, cloud cover, and pressure. The workflow includes:

- Data Preprocessing & Cleaning
- Exploratory Data Analysis (EDA)
- Handling Class Imbalance
- Model Building (Traditional ML, Ensemble, Deep Learning)
- Hyperparameter Optimization

---

## 🚀 Dataset

- **Source**: Daily weather data collected from January to October 2023.
- **Features**:
  - Average Temperature
  - Humidity
  - Average Wind Speed
  - Cloud Cover
  - Pressure
  - Rain or Not (Target)

🔗 **Preprocessed Dataset**: [Download Here](https://drive.google.com/file/d/1doLdSijUKPy7Pkld5RGil0OVigcouKXY/view?usp=sharing)

---

## 🔧 Data Preprocessing

### 📉 Handling Missing Values
- Utilized **KNN Imputation** for accurate estimation without bias.

### ⚙️ Encoding
- Binary categorical variable `rain_or_not` encoded as `0` (No Rain) and `1` (Rain).

### ⚖️ Addressing Class Imbalance
- Applied **SMOTE** and **SMOTE-ENN** to balance the dataset.

---

## 🔍 Exploratory Data Analysis (EDA)

### ✅ Key Insights:
- **Pressure & Temperature**: Negative correlation.
- **Cloud Cover & Humidity**: Positive correlation.
- Clear **seasonal trends** in temperature and humidity.
- **Rainfall** is strongly linked to **lower pressure** and **higher cloud cover**.

---

## 🤖 Machine Learning Models

Several models were trained and evaluated on resampled datasets:

| Model                   | Accuracy | ROC-AUC Score |
|------------------------|----------|---------------|
| Logistic Regression     | ✅       | ✅            |
| Decision Tree           | ✅       | ✅            |
| Random Forest           | ✅       | ✅            |
| XGBoost                 | ✅       | ✅            |
| LightGBM                | ✅       | ✅            |

---

## 🧠 Ensemble Model

An ensemble using **Soft Voting** combined predictions from:

- Random Forest
- XGBoost
- Decision Tree
- LightGBM

### ✅ Performance:
- **Accuracy**: High
- **Precision**: High
- **Recall**: High
- **F1 Score**: High
- **ROC-AUC**: High

---

## 🔬 Deep Learning (LSTM)

Designed a Bidirectional LSTM architecture to capture temporal sequences in weather data.

### ✅ Performance:
- **Accuracy**: Moderate
- **Precision**: Moderate
- **Recall**: Moderate
- **F1 Score**: Moderate

---

## 🛠️ Hyperparameter Optimization

Used **GridSearchCV** for fine-tuning key models:

- **Random Forest**:
  - `n_estimators`: Optimized
  - `max_depth`: Optimized

- **LightGBM**:
  - `n_estimators`: Optimized
  - `learning_rate`: Optimized

Final Ensemble Model achieved **high accuracy and ROC-AUC** after tuning.

---

## ✅ Conclusion

The **Ensemble Model** outperformed all other models, demonstrating excellent performance in rainfall prediction by leveraging the strength of multiple algorithms.

---

## 🚀 Future Improvements

- **Advanced Outlier Detection**: Use methods like Isolation Forest or DBSCAN.
- **Feature Selection**: Apply SHAP value analysis for better feature understanding.
- **Model Enhancements**: Experiment with Transformer models for temporal data.
- **Automated Tuning**: Use AutoML for automatic model and hyperparameter selection.
- **Class Imbalance**: Explore advanced resampling methods like ADASYN.

---

## 📂 Repository Structure

