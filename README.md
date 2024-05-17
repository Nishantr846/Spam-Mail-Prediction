## Spam Mail Prediction
This repository contains a Python script for detecting spam emails using a Logistic Regression model. The script performs data collection, preprocessing, feature extraction, model training, and evaluation. It also includes a simple example to predict whether a given email message is spam or ham.

# Table of Contents
Introduction
Installation
Usage
Dataset
Dependencies
Code Overview
  Data Collection & Preprocessing
  Feature Extraction
  Model Training
  Model Evaluation
  Prediction Example
Contributing
License
# Introduction
This project aims to classify emails as spam or ham (non-spam) using machine learning techniques. The model is trained using a dataset of labeled emails and leverages the TfidfVectorizer for feature extraction and Logistic Regression for classification.

# Installation
Clone the repository
Install the required dependencies

# Usage
Ensure you have the dataset (mail_data.csv) in the appropriate directory or modify the path in the script to point to your dataset location.

Run the script
To predict a new email, modify the input_mail variable in the script with the content of the email you want to classify.
Dataset
The dataset should be a CSV file named mail_data.csv with the following structure:

Category: The label of the email (spam or ham).
Message: The content of the email.

# Dependencies
The project requires the following Python packages:

numpy
pandas
scikit-learn

You can install these packages using pip

## Code Overview
# Data Collection & Preprocessing
The script begins by loading the dataset using pandas and replacing null values with empty strings. It then encodes the labels, converting 'spam' to 0 and 'ham' to 1.

# Feature Extraction
Text features are extracted using TfidfVectorizer, which converts the text data into numerical features suitable for machine learning algorithms.

# Model Training
A Logistic Regression model is trained using the extracted features and corresponding labels.

# Model Evaluation
The model's performance is evaluated on both the training and test datasets using accuracy as the metric.

# Prediction Example
The script includes a simple example that demonstrates how to predict whether a given email is spam or ham using the trained model.

# Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss changes or improvements.
