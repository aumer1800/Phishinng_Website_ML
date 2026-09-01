#  Phishing Website Detection Using Machine Learning

A machine learning classification project that detects whether a website is **legitimate or phishing** based on different characteristics of the website and its URL.

##  Project Overview

Phishing websites are designed to trick users into providing sensitive information such as passwords, banking details, or personal information.

In this project, machine learning models are trained to identify suspicious websites and classify them as:

* 🟢 **Legitimate**
* 🔴 **Phishing**

The goal is to build a reliable classification model that can help identify potentially malicious websites.

##  What We Achieved

In this project, we:

* Cleaned and prepared the phishing website dataset
* Removed unnecessary features such as the dataset index
* Checked for missing values and duplicate records
* Performed exploratory data analysis (EDA)
* Split the data into training and testing sets
* Trained multiple classification models
* Compared models using multiple evaluation metrics
* Selected **Random Forest** as the best-performing model

##  Machine Learning Models

The following models were evaluated:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest

##  Model Performance

| Model               |     Accuracy |    Precision |       Recall |     F1 Score |      ROC-AUC |
| ------------------- | -----------: | -----------: | -----------: | -----------: | -----------: |
| **Random Forest**   | **0.973768** | **0.968850** | **0.984578** | **0.976651** | **0.994479** |
| KNN                 |     0.941203 |     0.944355 |     0.950487 |     0.947411 |     0.984616 |
| Logistic Regression |     0.938942 |     0.940562 |     0.950487 |     0.945499 |     0.982430 |
| Decision Tree       |     0.965626 |     0.966882 |     0.971591 |     0.969231 |     0.974149 |

###  Best Model

**Random Forest** achieved the best overall performance:

* **Accuracy:** 97.38%
* **Precision:** 96.89%
* **Recall:** 98.46%
* **F1 Score:** 97.67%
* **ROC-AUC:** 99.45%

This means the Random Forest model was able to correctly classify the majority of websites while maintaining a strong balance between detecting phishing websites and avoiding incorrect classifications.

##  Dataset

The dataset contains **11,054 website records** with features describing different characteristics of websites and their URLs.

Some of the features include:

* URL length
* HTTPS usage
* IP address usage
* URL shortening
* Redirects
* Subdomains
* Domain registration information
* Request URL
* Anchor URL
* Website traffic
* PageRank
* Google indexing
* DNS recording
* And other website-related characteristics

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Jupyter Notebook / Google Colab

##  Project Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature & Target Separation
   ↓
Train/Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Best Model Selection
```


##  Future Improvements

The project can be extended by:

* Hyperparameter tuning
* Cross-validation
* Feature importance analysis
* SHAP explainability
* Saving the trained model
* Building a Flask/FastAPI backend
* Creating a React dashboard
* Deploying the model as a web application

##  Disclaimer

This project is developed for **educational and research purposes**. The model should not be considered a complete security solution for detecting real-world phishing websites.

##  Project Goal

The main goal of this project was to demonstrate how machine learning can be applied to a real-world cybersecurity problem and to compare different classification algorithms to identify the most effective model.
