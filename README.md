# Credit Risk Prediction System

## Overview

This project is a machine learning application that predicts the probability of loan default based on financial and behavioral attributes of borrowers. The system calculates the **default probability**, converts it into a **credit score**, and assigns a **risk rating**.

The model is deployed using **Streamlit**, allowing users to interactively input borrower details and receive real-time predictions.

Live App:
https://credit-risk-model-001.streamlit.app/

---

## Features

* Predicts **probability of loan default**
* Converts probability into a **credit score**
* Assigns a **risk rating category**
* Interactive **Streamlit web interface**
* End-to-end ML pipeline from input to prediction
* Cloud deployment using **Streamlit Community Cloud**

---

## Input Features

The model evaluates borrower risk using the following attributes:

* Age
* Income
* Loan Amount
* Loan Tenure (months)
* Average DPD per Delinquency
* Delinquency Ratio
* Credit Utilization Ratio
* Number of Open Accounts
* Residence Type
* Loan Purpose
* Loan Type

---

## Output

The system produces three outputs:

1. **Default Probability** – likelihood that the borrower will default on the loan
2. **Credit Score** – score derived from predicted probability
3. **Risk Rating** – credit rating category based on the score

---

## Tech Stack

**Programming Language**

* Python

**Libraries**

* pandas
* numpy
* scikit-learn
* xgboost
* joblib

**Framework**

* Streamlit

**Deployment**

* Streamlit Community Cloud

---

## Project Structure

```
credit-risk-model
│
├── main.py                 # Streamlit application
├── prediction_helper.py    # Prediction logic and scoring functions
├── requirements.txt        # Project dependencies
├── artifacts/              # Saved models and scalers
│
└── README.md
```

---

## How the System Works

1. User enters borrower details in the Streamlit interface
2. Input data is processed into a structured dataframe
3. The trained machine learning model predicts default probability
4. Probability is converted into a credit score
5. A rating category is assigned based on the score

---

## Installation (Run Locally)

Clone the repository:

```
git clone https://github.com/Sanjureddy-17/credit-risk-model.git
cd credit-risk-model
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the application:

```
streamlit run main.py
```

---

## Example Output

Input borrower details → Model prediction:

Default Probability: **23%**
Credit Score: **645**
Risk Rating: **Moderate Risk**

---
