<h1 align="center">Spam Detection using Machine Learning</h1>
<p align="center">Classifying messages as spam or ham using ML models</p>

## Introduction
Spam messages are a common issue in emails and SMS. They can be annoying and sometimes harmful. In this project, I built a machine learning model to automatically classify messages as spam or not spam based on their content.

## Problem Statement
The aim of this project is to develop a model that can accurately detect spam messages while minimizing incorrect classifications.

Some challenges faced:
- Converting text data into numerical format  
- Handling imbalance in the dataset  
- Avoiding false positives (normal messages marked as spam)  
- Detecting most spam messages effectively  

## Dataset
The dataset contains labeled messages:
- `text` → message content  
- `target` → spam or ham  

## Data Preprocessing
- Removed unnecessary columns
- Converted text to lowercase  
- Removed punctuation and stopwords  
- Applied lemmatization  
- Joined processed words into text format  

## Feature Extraction
Used TF-IDF to convert text into numerical features:

## Models Used

The following machine learning models were trained and evaluated:

- Naive Bayes
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest

## Evaluation Metrics

Models were evaluated using:

- Accuracy → overall correctness
- Precision → how many predicted spam messages were actually spam
- Recall → how many actual spam messages were detected
- F1 Score → balance between precision and recall
- Confusion matrix->Used to evaluate model predictions by comparing actual and predicted values
