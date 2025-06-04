# Telco Customer Churn Prediction 🎯

This project predicts customer churn for a telecom company using machine learning and presents the results through a user-friendly Streamlit web interface.

---

## 📁 Dataset

We use the **Telco Customer Churn** dataset which contains customer data such as demographic information, account details, and service usage.

- Target variable: `Churn` (Yes/No → 1/0)
- Features include:
  - Customer tenure, monthly/total charges
  - Subscription details (InternetService, Contract, etc.)
  - Demographics (SeniorCitizen, gender, etc.)

---

## 🧠 Machine Learning

Two models are trained:
- **Logistic Regression**
- **XGBoost Classifier** ✅ (chosen for deployment)

### Preprocessing
- Dropped missing values and customer ID.
- Converted categorical columns using one-hot encoding.
- Scaled numerical features using `StandardScaler`.

### Evaluation
Models were evaluated using classification metrics (accuracy, precision, recall, f1-score).

### Model Saving
The final `XGBoost` model and the scaler were saved using `joblib`.

---

## 💻 Streamlit Web App

The `Streamlit` UI allows users to input customer data and predict churn probability using the trained XGBoost model.

### Features:
- Interactive input forms
- Real-time prediction
- Displays churn status with probability

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/churn-prediction-app.git
   cd churn-prediction-app

