# Wearable Stress Analytics & Performance Prediction Platform 📊⌚

**Multimodal wearable sensor analytics platform for modelling stress responses and predicting academic performance using machine learning.**

This project analyses real-world physiological data collected from university students during high-stakes exams to understand stress behaviour and predict academic outcomes. The system processes multimodal wearable signals — including heart rate, electrodermal activity (EDA), skin temperature, and accelerometer data — and applies advanced feature engineering and machine learning techniques to build reliable predictive models.

The platform demonstrates end-to-end **data preprocessing, time-series feature engineering, statistical modelling, and analytics pipeline design**, aligned with real-world data analytics and cloud-based workflows.

---

## 🚀 Project Overview

The objective of this platform is to explore how physiological stress patterns influence academic performance. By combining signal processing, statistical feature extraction, and machine learning experimentation, the project builds a reproducible analytics workflow for wearable datasets.

Key goals:

- Analyse multimodal physiological signals collected during exams  
- Predict academic performance using classification and regression models  
- Investigate stress-response trends through time-series analysis  
- Build a structured analytics pipeline for wearable sensor data  

---

## 📂 Dataset

- Source: **PhysioNet – Wearable Exam Stress Dataset**
- Participants: University students monitored during final exams
- Signals Included:
  - Heart Rate
  - Electrodermal Activity (EDA)
  - Skin Temperature
  - Accelerometer Data

📌 **Note:** Dataset access may require PhysioNet credentials and compliance with data usage policies.

---

## 🧱 Project Structure

### 🔧 `preprocessing.ipynb`

Data engineering and feature pipeline:

- Missing value handling using KNN Imputer  
- Rolling window segmentation for time-series modelling  
- Timestamp windowing for temporal consistency  
- Feature extraction:
  - Statistical metrics (mean, std, range, entropy, kurtosis)
  - STL trend decomposition
  - PCA for dimensionality reduction
- Correlation-based feature selection

---

### 🤖 `modelling.ipynb`

Model development and evaluation:

- Label encoding of academic performance  
- Leave-One-Student-Out Cross-Validation (LOSO-CV) for generalisation  
- Model experimentation:
  - Random Forest
  - XGBoost
  - MLP
  - SVM
  - ExtraTrees
  - Logistic Regression
  - KNN

Evaluation metrics:

- Classification: Accuracy, F1 Score, Precision, Recall  
- Regression: MAE, RMSE, R² Score  

Includes comparative analysis and performance visualisation.

---

## ⭐ Key Highlights

- Multimodal physiological signal processing  
- Advanced time-series feature engineering and statistical modelling  
- Robust validation using LOSO-CV methodology  
- Comparative machine learning experimentation  
- Insights into academic stress behaviour patterns

---

## 🔮 Future Enhancements

- Sequential deep learning models (LSTM, Transformers)  
- Real-time stress monitoring dashboards  
- Integration of contextual behavioural data  
- Cloud deployment for scalable analytics workflows  

---

## 🌍 Use Cases

- Academic stress monitoring systems  
- Wearable health analytics research  
- Behavioural signal modelling  
- Applied machine learning experimentation

---

## 👤 Author

**Charan Gorentla Ravi**  
Data Analytics | Cloud Platforms | Python | SQL  
🔗 https://linkedin.com/in/charan-gr

---

## 📜 License

This repository is intended for academic and research purposes only.
