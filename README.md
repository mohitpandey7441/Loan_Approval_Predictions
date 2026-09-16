# Loan Approval Prediction

A Machine Learning project that predicts whether a loan application is likely to be **Approved** or **Rejected** based on applicant and loan-related information.

## Project Overview

This project covers the complete machine learning workflow:

* Data loading and exploration
* Exploratory Data Analysis (EDA)
* Missing-value handling
* Categorical data encoding
* Feature engineering
* Box-Cox transformation
* Loan-term conversion
* Train-test split
* Cross-validation
* Hyperparameter tuning using GridSearchCV
* Model comparison
* Feature importance analysis
* Flask-based model deployment

## Dataset

The project uses `Loan_Data.csv`.

Important features include:

* Gender
* Married
* Dependents
* Education
* Self_Employed
* ApplicantIncome
* CoapplicantIncome
* LoanAmount
* Loan_Amount_Term
* Credit_History
* Property_Area
* Loan_Status

**Target:** `Loan_Status`

## Machine Learning Models

The notebook evaluates:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Machine (SVM)
4. Decision Tree
5. Random Forest
6. AdaBoost
7. Gradient Boosting
8. XGBoost

The project also uses cross-validation and hyperparameter tuning.

## Model Evaluation

| Model               | Test Accuracy |
| ------------------- | ------------: |
| Logistic Regression |        78.30% |
| KNN                 |        70.75% |
| SVM                 |        78.30% |
| Decision Tree       |        78.30% |
| Random Forest       |        76.42% |
| AdaBoost            |        76.42% |
| Gradient Boosting   |        77.36% |
| XGBoost             |        77.36% |

> These values are the test results from the project notebook and should not be interpreted as guaranteed real-world performance.

## Deployment

The trained model is deployed using **Flask**.

The application accepts applicant information and returns:

* **Loan Approved**
* **Loan Rejected**

## Project Workflow

```text
Loan Dataset
     ↓
Data Loading
     ↓
Data Cleaning
     ↓
EDA
     ↓
Missing Value Handling
     ↓
Encoding & Feature Engineering
     ↓
Data Transformation
     ↓
Train / Test Split
     ↓
Cross-Validation
     ↓
Model Training
     ↓
Hyperparameter Tuning
     ↓
Model Evaluation
     ↓
Best Model
     ↓
Flask Deployment
     ↓
Loan Approval Prediction
```

## Project Structure

```text
Loan-Approval-Prediction/
│
├── app.py
├── model/
│   └── ab_best_model.pkl
├── templates/
│   └── index.html
├── static/
│   └── style.css
├── data/
│   └── Loan_Data.csv
├── notebooks/
│   └── Loan Prediction Project.ipynb
├── requirements.txt
└── README.md
```

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* SciPy
* XGBoost
* Matplotlib
* Seaborn
* Flask
* Jupyter Notebook

## Run the Flask Application

```bash
python app.py
```

Then open the local URL shown by Flask in your browser.

## Key Features

* Complete ML pipeline from preprocessing to deployment
* Multiple classification models
* Cross-validation
* Hyperparameter tuning
* Model comparison
* Feature engineering
* Flask web deployment
* Loan approval prediction interface

## Future Improvements

* Add more applicant and financial features
* Improve model performance with additional data
* Add probability/confidence output
* Deploy the application to a cloud platform
* Improve the user interface

## Disclaimer

This project is intended for educational and demonstration purposes. Loan predictions should not be used as the sole basis for real financial decisions.
