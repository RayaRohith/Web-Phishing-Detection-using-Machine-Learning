# Web Phishing Detection using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-green?style=flat-square)
![Flask](https://img.shields.io/badge/Flask-Web%20App-lightgrey?style=flat-square&logo=flask&logoColor=white)
![IBM](https://img.shields.io/badge/IBM-AICTE%20Project-052FAD?style=flat-square&logo=IBM&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

---

**Type:** Collaborative Undergraduate Project
**Team:** Prasanna Srinivas R, Raya Rohith Yadav, Raghul C, Sakthivel P
**Institution:** Anna University (AICTE/IBM Project, 2022)

---

## Overview

Phishing is one of the most prevalent and damaging forms of cybercrime, targeting users through fraudulent websites that impersonate legitimate organisations to steal credentials, financial data, and personal information. High-profile breaches attributed to phishing include the 2014 JPMorgan Chase attack (76 million households affected) and the Sony Pictures breach ($100 million in damages).

This project builds a machine learning classification system capable of detecting phishing websites based on URL structure, domain identity, and security and encryption characteristics. The trained model is deployed as a Flask web application, allowing users to submit a URL and receive a real-time phishing verdict.

---

## Problem Statement

Existing phishing detection methods are limited in scope, often analysing fewer than 10 URL features and performing poorly against novel phishing campaigns. This project addresses that gap by applying supervised machine learning classification across a broader feature set derived from URL properties, domain registration data, and SSL/TLS indicators.

---

## Solution Approach

The system extracts features from a submitted URL across three categories:

- **Domain identity:** IP address usage, domain age, DNS record presence, WHOIS registration
- **URL structure:** Length, use of shortening services, presence of `@` or `-` symbols, subdomain depth
- **Security and encryption:** HTTPS usage, SSL certificate validity, favicon source, port usage

These features are used to train and evaluate multiple classification algorithms. The best-performing model is integrated into a Flask web application for real-time prediction.

---

## Technical Architecture

```
User submits URL
        |
Feature Extraction (URL, Domain, SSL)
        |
ML Classification Model
        |
Prediction: Phishing / Legitimate
        |
Flask Web App Response
```

---

## Tech Stack

| Category | Technology |
|---|---|
| Language | Python 3 |
| ML Libraries | Scikit-learn, Pandas, NumPy, Keras |
| Web Framework | Flask |
| Platform | IBM Watson, IBM Cloud |
| Development | Jupyter Notebook |

---

## ML Models Evaluated

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- Neural Network (Keras)

Models were evaluated on accuracy, precision, recall, and F1-score. The best-performing model was selected for deployment.

---

## Project Structure

```
Web-Phishing-Detection-using-Machine-Learning/
└── IBM-Project-25628-1659969123-main/
    ├── Assessments/          Project milestone assessments
    ├── Final Deliverables/   Final model, Flask app, and report
    ├── Ideation/             Problem framing and ideation documents
    ├── Project Design/       Architecture and design documents
    └── Project Development/  Notebooks, model training, Flask app code
```

---

## Key Learnings

- Phishing detection is a binary classification problem where feature engineering from URL and domain metadata is the critical determinant of model performance
- Random Forest and ensemble methods outperformed single classifiers on this dataset due to the heterogeneous nature of URL features
- Client-facing deployment via Flask requires careful input validation to prevent the detection tool itself from becoming an attack vector

---

## Disclaimer

This project was developed for educational purposes as part of the AICTE/IBM internship programme. All testing was conducted on publicly available phishing datasets. No unauthorised systems were accessed.

---

## Author Contribution

**Raya Rohith Yadav** — Feature engineering, model evaluation, Flask integration
MSc Cyber Security, University of Edinburgh (2023-2025)

[LinkedIn](https://www.linkedin.com/in/raya-rohith-yadav-b71206204/) | [GitHub](https://github.com/RayaRohith)
