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
- Confusion matrix->Used to evaluate model predictions by comparing actual and predicted values### Best Model: Naive Bayes
## Results

Out of all the models, Naive Bayes performed the best overall.

F1 Score: 0.94  
Accuracy: 98.38%  
Precision: 98.61%  
Recall: ~89.87%  

It provides a good balance between precision and recall. It rarely classifies normal messages as spam, which means very low false positives. At the same time, it is able to detect most spam messages effectively.

### Other Models

#### SVM and Random Forest
Both SVM and Random Forest showed very similar performance.

F1 Score: ~0.93  
Accuracy: ~98.2%  

They maintain a good balance between detecting spam and avoiding false alarms, making them strong alternatives.

#### Logistic Regression
Precision: 98.43%  
Recall: 79.75%  

Logistic Regression gives reliable predictions when it labels a message as spam. However, it misses more spam messages compared to other models.

#### Decision Tree
F1 Score: ~0.88  

Decision Tree performed lower than the other models and was less consistent in classification.

### Conclusion
Naive Bayes turned out to be the best model for this task. SVM and Random Forest also performed well and can be considered good alternatives. Logistic Regression is very precise but misses more spam messages, while Decision Tree showed the least performance.

This shows that Naive Bayes works especially well for text-based classification problems like spam detection.
