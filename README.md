# Student Performance Prediction System

## Overview
This repository contains the complete end-to-end machine learning project for **Task 4** of the Devixo Solutions AI/ML Internship. The project successfully transitions a traditional machine learning pipeline into a fully functional, interactive web application using Streamlit.

---

## Project Pipeline & Architecture
1. **Data Preprocessing & Scaling**: Cleaned student dataset features and applied `StandardScaler` to normalize numerical indicators for optimal model training.
2. **Model Training & Evaluation**: Trained and evaluated four distinct classification models:
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
   - Gradient Boosting Classifier (Achieved top performance with 95% Accuracy, Precision, Recall, and F1-Score)
3. **Hyperparameter Tuning**: Optimized the top-performing Gradient Boosting model using `GridSearchCV` with 3-fold cross-validation (`cv=3`).
4. **Model Persistence**: Serialized the final optimized model and scaler into binary format using `joblib`.
5. **Interactive Web Application**: Developed a real-time prediction dashboard using Streamlit.

---

## Files Included in Submission
* **`app.py`**: The complete frontend and backend Streamlit web application code.
* **`best_model.pkl`**: The tuned Gradient Boosting classification model artifact.
* **`scaler.pkl`**: The fitted `StandardScaler` artifact.

---

## How to Run the Application Locally
1. Ensure `app.py`, `best_model.pkl`, and `scaler.pkl` are saved together in the exact same folder.
2. Open your terminal or command prompt inside that folder and install the required dependencies:
   ```bash
   pip install streamlit scikit-learn pandas numpy joblib
