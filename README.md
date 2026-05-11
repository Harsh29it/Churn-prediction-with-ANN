# Churn-prediction-with-ANN

# Customer Churn Prediction using ANN

## Overview

This project uses an Artificial Neural Network (ANN) built with TensorFlow and Keras to predict customer churn based on banking customer data. The model analyzes customer information such as credit score, geography, gender, balance, and salary to determine whether a customer is likely to leave the bank.

The project also includes data preprocessing, feature scaling, model training, and evaluation using Python machine learning libraries.

---

## Features

* Data preprocessing and cleaning
* Encoding categorical variables
* Feature scaling using StandardScaler
* Train-test split for model evaluation
* Artificial Neural Network (ANN) implementation
* Model training and prediction
* Performance evaluation using accuracy

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook

---

## Dataset

The project uses the **Churn Dataset**, which contains customer banking details such as:

* Credit Score
* Geography
* Gender
* Age
* Balance
* Number of Products
* Estimated Salary
* Exited (Target Variable)

Target Variable:

* `0` → Customer Stayed
* `1` → Customer Left the Bank

---

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas.

### 2. Data Cleaning

Irrelevant columns such as:

* RowNumber
* CustomerId
* Surname

are removed.

### 3. Data Preprocessing

* Label Encoding is applied to categorical columns.
* StandardScaler is used for feature scaling.

### 4. Model Building

A Sequential ANN model is created using:

* Input Layer
* Hidden Layers with ReLU activation
* Output Layer with Sigmoid activation

### 5. Model Training

The model is trained using:

* Adam Optimizer
* Binary Crossentropy Loss Function

### 6. Prediction & Evaluation

The trained model predicts customer churn and evaluates performance using accuracy metrics.

---

## ANN Architecture

```python
ann = Sequential()
ann.add(Dense(6, input_dim=10, activation='relu'))
ann.add(Dense(4, activation='relu'))
ann.add(Dense(2, activation='relu'))
ann.add(Dense(1, activation='sigmoid'))
```


## Future Improvements

* Hyperparameter tuning
* Improve model accuracy
* Add confusion matrix and ROC curve
* Deploy the model using Flask or Streamlit
* Add Deep Learning optimization techniques

---

## Conclusion

This project demonstrates how Artificial Neural Networks can be used for customer churn prediction in the banking sector. By applying preprocessing techniques and deep learning models, the system can help businesses identify customers who are likely to leave and improve retention strategies.

---

## Author

Harshit Thapa

---
