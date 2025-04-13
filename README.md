# Wearable Sensor Data: Stress Response & Academic Performance Prediction

This repository contains the codebase for analyzing wearable physiological sensor data to predict student performance and explore stress responses during high-stakes academic exams.

We have leveraged a real-world dataset collected from university students during their final exams, using multimodal physiological signals such as heart rate, electrodermal activity (EDA), skin temperature, and accelerometer readings.

## Dataset

The original dataset is available at [PhysioNet: Wearable Exam Stress Dataset](https://physionet.org/content/wearable-exam-stress/1.0.0/).

> 📌 **Note:**  
> The dataset contains multimodal recordings from a real-world academic setting, including motion artifacts and a relatively small participant pool. In the original publication, only electrodermal activity (EDA) was explored with basic machine learning methods. In our work, we extend this to multimodal signals and advanced feature engineering for deeper insights.

## Project Structure

- **preprocessing.ipynb**  
  - Data cleaning and handling missing values with KNN imputer.
  - Rolling window creation to segment time-series data.
  - Timestamp windowing to maintain temporal consistency.
  - Feature extraction: basic (mean, std), statistical (range, entropy, kurtosis), and dimensionality reduction using PCA.
  - STL decomposition for trend analysis of physiological signals.
  - Feature selection using correlation-based filtering.

- **modelling.ipynb**  
  - Label encoding of student grades.
  - Leave-One-Student-Out cross-validation (LOSO-CV) to generalize model performance.
  - Baseline model: Random Forest Classifier.
  - Model experiments with XGBoost, MLP, SVM, ExtraTrees, Logistic Regression, KNN, and Random Forest.
  - Evaluation metrics: Accuracy, F1 Score, Precision, Recall (Classification); MAE, RMSE, R² Score (Regression).
  - Comparative analysis of models and performance visualization.

## Highlights

- **Multimodal Signal Processing:** Combined heart rate, EDA, temperature, and motion data.
- **Advanced Feature Engineering:** Trend decomposition (STL), statistical features, PCA for dimensionality reduction.
- **Robust Modelling:** Applied both classification and regression models to predict performance labels and actual grades.
- **Rigorous Validation:** Leave-One-Student-Out Cross-Validation ensures model robustness on unseen participants.
- **Result Insights:** Discussed both high and medium performers' physiological patterns, with meaningful academic stress implications.

## Future Directions

- Expand the participant pool for better generalization.
- Explore deep learning approaches for sequential modelling (e.g., LSTMs, Transformers).
- Integrate additional contextual data (e.g., self-reported stress levels, environmental factors).
- Deploy real-time monitoring dashboards for academic stress management.

## Reference

If you use this work, please consider citing the original dataset publication:

## License

This repository is for academic and research purposes only.
