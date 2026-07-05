# Customer-Churn-Predcition

## Project Overview

Customer churn prediction is a machine learning project that predicts whether a customer is likely to leave a company based on customer demographics, account information, and service usage. This helps businesses identify at-risk customers and take proactive measures to improve customer retention.

---

## Features

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Label Encoding for categorical features
- Handling class imbalance using SMOTE
- Model training using XGBoost Classifier
- Model evaluation using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- Model serialization using Joblib
- Streamlit web application for real-time churn prediction

---

## Dataset

The project uses the **Telco Customer Churn Dataset**.

### Dataset Features

- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies
- Contract
- Paperless Billing
- Payment Method
- Monthly Charges
- Total Charges
- Churn (Target Variable)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Joblib
- Streamlit

---

## Project Structure

```
Customer-Churn-Prediction/
│
├── churn_app.py                 # Streamlit application
├── customer_churn.ipynb         # Jupyter notebook
├── customer_churn_model.pkl     # Trained model
├── churn_encoders.pkl           # Saved encoders
├── Telco-Customer-Churn.csv     # Dataset
├── requirements.txt             # Project dependencies
├── README.md
└── venv/
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
```

Navigate to the project folder

```bash
cd customer-churn-prediction
```

Create a virtual environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux/macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Train the model

Open and run

```
customer_churn.ipynb
```

This will generate:

- customer_churn_model.pkl
- churn_encoders.pkl

---

### Run the Streamlit App

```bash
streamlit run churn_app.py
```

The application will open in your browser.

---

## Model Workflow

1. Load the dataset
2. Perform data preprocessing
3. Encode categorical variables
4. Split the dataset into training and testing sets
5. Balance the training data using SMOTE
6. Train the XGBoost classifier
7. Evaluate model performance
8. Save the trained model
9. Deploy using Streamlit

---

## Evaluation Metrics

The model is evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## Sample Prediction

Input customer information through the Streamlit interface.

Example:

- Gender: Female
- Senior Citizen: No
- Contract: Month-to-Month
- Internet Service: Fiber Optic
- Monthly Charges: 75.25
- Tenure: 12

Output:

```
Prediction: Customer is likely to Churn
```

or

```
Prediction: Customer is likely to Stay
```

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Feature selection
- Explainable AI using SHAP
- Model deployment on cloud platforms
- REST API integration

---

## Requirements

Example dependencies:

```
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
imbalanced-learn
joblib
streamlit
```

Install using:

```bash
pip install -r requirements.txt
```



