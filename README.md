# Credit Risk Prediction 

An end-to-end data science and machine learning project focused on predicting the credit risk level of loan applications. The project covers exploratory data analysis, data visualisation, feature engineering, machine learning model development and deployment through an interactive Streamlit web application.

## Overview

Assessing credit risk helps financial institutions make informed lending decisions. This project uses an **Extra Trees Classifier** to predict whether a loan applicant is likely to be classified as having good or bad credit risk based on selected applicant details.

Users can enter information such as age, credit amount, loan duration, employment status, housing, savings, checking account status and loan purpose to generate a prediction.

## Features

- Explore and understand the credit risk dataset through exploratory data analysis.
- Identify patterns, trends and relationships using data visualisation.
- Prepare the dataset and perform feature engineering.
- Train and evaluate machine learning models for credit risk classification.
- Select a suitable model for prediction.
- Deploy the trained model through an interactive Streamlit web application.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

- Examined the dataset's structure, columns and data types.
- Investigated missing values and data distributions.
- Analysed relationships between applicant characteristics and credit risk.
- Used visualisations to identify patterns and potential insights.

### 2. Data Preprocessing and Feature Engineering

- Prepared the dataset for machine learning.
- Processed categorical variables using appropriate encoding techniques.
- Selected and prepared relevant features for model training.
- Prepared the target variable for classification.

### 3. Model Development and Evaluation

- Trained multiple machine learning models for credit risk classification.
- Evaluated model performance using appropriate classification metrics.
- Applied hyperparameter tuning to improve model performance.
- Selected an Extra Trees Classifier for integration into the deployed application.

### 4. Model Deployment

- Saved the trained model and categorical encoders using Joblib.
- Developed an interactive web application using Streamlit.
- Integrated the trained Extra Trees model into the application.
- Enabled users to enter applicant details and obtain predicted credit risk classifications.

## Technologies Used

- **Python** – Core programming language.
- **Pandas** – Data manipulation and analysis.
- **NumPy** – Numerical computing.
- **Matplotlib and Seaborn** – Data visualisation.
- **Scikit-learn** – Data preprocessing, machine learning, model evaluation and hyperparameter tuning.
- **Joblib** – Model and encoder persistence.
- **Streamlit** – Deployment of the interactive prediction application.

## Project Structure

```text
credit_risk_modelling/
├── app.py
├── analysis_model.ipynb
├── data.txt
├── extra_trees_credit_model.pkl
├── Sex_encoder.pkl
├── Housing_encoder.pkl
├── Saving accounts_encoder.pkl
├── Checking account_encoder.pkl
├── README.md
└── .venv/
```

> The `.venv` folder contains the local Python environment and should generally not be committed to GitHub. The model and encoder files are required by the app unless you modify the code to load them from another location.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/credit-risk-prediction-app.git
cd credit-risk-prediction-app
```

Replace `YOUR_USERNAME` and the repository name with your GitHub details.

### 2. Create and Activate a Virtual Environment

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

```bash
pip install streamlit pandas numpy scikit-learn joblib matplotlib seaborn
```

### 4. Run the Application

```bash
streamlit run app.py
```

Streamlit will provide a local URL, usually:

```text
http://localhost:8501
```

Open the URL in your browser to use the app.

## Using the App

1. Open the application in your browser.
2. Enter the applicant's financial details.
3. Submit the information for prediction.
4. View the predicted credit risk category.

The prediction is based on patterns learned from the dataset and should not be interpreted as a guaranteed outcome.

## Model

The application uses an **Extra Trees Classifier**, an ensemble learning algorithm that combines predictions from multiple decision trees.

The model can capture non-linear relationships between applicant features and credit risk. Its performance depends on the quality, representativeness and preprocessing of the training data.

## Future Improvements

- Add model performance metrics such as precision, recall, F1-score and ROC-AUC.
- Improve handling of missing and unseen categorical values.
- Add prediction confidence or probability estimates.
- Include feature importance visualisations.
- Improve the app's layout and user experience.
- Deploy the application to Streamlit Community Cloud or another hosting platform.
- Add automated tests for preprocessing and prediction.

## Disclaimer

This project is intended for **learning and demonstration purposes only**. It is not financial advice and should not be used to make real lending decisions. Credit decisions require validated models, appropriate data governance, fairness assessments, regulatory compliance and human oversight.

## Author

**Chioma Jennifer Muofunanya**
