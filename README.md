

# 📊 Credit Risk Analyzer

A **production-grade Credit Risk Assessment System** that predicts **default probability**, generates a **credit score**, and classifies applicants into **Poor, Average, Good, or Excellent** risk categories—aligned with real-world **CIBIL-style scoring logic**.

---

## 🚀 Project Overview

This project leverages **machine learning** to evaluate loan applications using customer demographics, financial behavior, and credit bureau data.
The system helps financial institutions make **data-driven lending decisions** by quantifying creditworthiness accurately.

### 🔢 Credit Rating Logic

```python
def get_rating(score):
    if 300 <= score < 500:
        return 'Poor'
    elif 500 <= score < 650:
        return 'Average'
    elif 650 <= score < 750:
        return 'Good'
    elif 750 <= score <= 900:
        return 'Excellent'
    else:
        return 'Undefined'
```

---

## ✨ Key Features

🔍 **Risk Prediction**

* Predicts **default probability**
* Generates a **credit score**
* Assigns a **credit rating**

🧾 **Input Parameters**

* Age
* Income
* Loan Amount
* Loan Tenure (Months)
* Average DPD per Delinquency
* Delinquency Ratio
* Credit Utilization Ratio
* Number of Open Accounts
* Residence Type
* Loan Purpose
* Loan Type

📈 **Model Explainability**

* Feature importance visualization for transparency

---

## 🛠️ Tech Stack

* **Language**: Python
* **Frameworks & Libraries**:

  * `scikit-learn`
  * `xgboost`
  * `pandas`
  * `numpy`
  * `joblib`
  * `streamlit`

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone <repository-url>
cd <repository-folder>
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Application

```bash
streamlit run app.py
```

---

## 🧪 How to Use

1. Open the deployed application:
   👉 **[Live Streamlit App](https://credit-risk-analyzer-kesavadas.streamlit.app/)**

2. Enter customer and loan details.

3. View predictions:

   * **Default Probability** (e.g., `63.25%`)
   * **Credit Score** (e.g., `520`)
   * **Credit Rating** (e.g., `Average`)

---

## 🗂️ Dataset Information

📌 Combined datasets:

* Customers Dataset
* Loans Dataset
* Credit Bureau Dataset

📊 Final dataset:

* **50,000 rows**
* **33 features**

---

## 🧠 Machine Learning Pipeline

1. **Early Train-Test Split** – Prevents data leakage
2. **Data Cleaning** – Invalid values replaced using statistical mode
3. **Feature Selection** – VIF, IF, and domain expertise
4. **Scaling** – Min-Max normalization
5. **Train-Test Ratio** – 75% train, 25% test
6. **Model Training**:

   * Logistic Regression
   * Random Forest
   * XGBoost
7. **Hyperparameter Optimization**:

   * RandomizedSearchCV
   * Optuna
8. **Evaluation Metrics**:

   * AUC-ROC
   * KS Statistic
   * Gini Coefficient
   * Classification Report

---

## ☁️ Deployment

* **Platform**: Streamlit Cloud
* Fully interactive and accessible online

---

## 📸 Screenshots

### 🔹 Application Interface

![App Screenshot](https://github.com/user-attachments/assets/f68243f6-916c-4f78-96dd-dc7f1f243425)

### 🔹 Feature Importance

![Feature Importance](https://github.com/user-attachments/assets/66c829de-493e-4fa4-a174-5ac77c4265f0)

---

## 📄 License

This project is licensed under the **Apache 2.0 License**.

---

## 🤝 Contributions

Contributions are welcome!
Feel free to **open issues**, suggest improvements, or submit **pull requests**.

---

