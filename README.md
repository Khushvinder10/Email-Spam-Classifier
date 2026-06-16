# Machine Learning Internship Project

# 📧 Email Spam Classifier

## Overview

This project is a Machine Learning-based Email Spam Classifier that classifies emails into two categories:

* Spam Mail
* Ham Mail (Not Spam)

The model is trained using the Email Spam Collection Dataset and uses Natural Language Processing (NLP) techniques to analyze email content and predict whether an email is spam or legitimate.

---

## Project Objective

The objective of this project is to build a machine learning model capable of automatically detecting spam emails based on the text content of the message.

This helps reduce unwanted emails and improves email security and user experience.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* TF-IDF Vectorizer
* Logistic Regression
* Jupyter Notebook

---

## Dataset Information

Dataset Name: Email Spam Collection Dataset

Features:

* Category (Spam or Ham)
* Message (Email/SMS Content)

Dataset Size:

* 5572 Messages
* 2 Columns

---

## Machine Learning Workflow

### 1. Data Loading

The dataset is loaded into a Pandas DataFrame using the `read_csv()` function.

### 2. Data Preprocessing

Missing values are handled and the dataset is cleaned for further processing.

### 3. Label Encoding

The target labels are converted into numerical form:

* Spam → 0
* Ham → 1

### 4. Train-Test Split

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

### 5. Feature Extraction

TF-IDF (Term Frequency – Inverse Document Frequency) is used to convert text messages into numerical feature vectors.

### 6. Model Training

A Logistic Regression model is trained on the extracted features.

### 7. Model Evaluation

The model performance is evaluated using Accuracy Score.

### 8. Predictive System

A predictive system is implemented to classify new emails entered by the user.

---

## Model Performance

Training Accuracy: 96.70%

Testing Accuracy: 96.77%

The model demonstrates strong performance with minimal overfitting and good generalization on unseen data.

---

## Sample Predictions

### Example 1

Input:

Congratulations! You have won a free iPhone. Click here to claim your prize.

Prediction:

Spam Mail

### Example 2

Input:

Hi John, let's meet tomorrow regarding the project discussion.

Prediction:

Ham Mail

---

## Project Structure

Email_Spam_Classifier

├── Spam_Email_Classifier.ipynb

├── mail_data.csv

├── README.md

└── Screenshots

    ├── dataset.png

    ├── shape.png

    ├── training_accuracy.png

    ├── testing_accuracy.png

    ├── spam_prediction.png

    └── ham_prediction.png

---

## Future Improvements

* Deploy the model using Streamlit
* Add Support Vector Machine (SVM) classifier
* Improve accuracy using advanced NLP techniques
* Build a complete web application

## Key Features

- Detects Spam and Ham emails
- Uses TF-IDF for text feature extraction
- Uses Logistic Regression for classification
- Achieves 96.77% test accuracy
- Supports prediction on custom email messages
