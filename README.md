# CREDIT CARD FRADULENT ANALYSIS 

Analysis of credit card fraudulent details with a globally available dataset. This repository contains code and analysis for credit card fraud detection using various machine learning models. The goal is to build and evaluate different models, compute ROC curves, and display confusion matrices to assess their performance in detecting fraudulent transactions. 

## PREREQUISITES:

1. Python:
   Necessary libraries have to be imported I have imported them in the code at the start itself. 
2. Datasets: I have taken it from Kaggle : (https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data)

## OVERVIEW:

### Dataset:
1. It comprises solely numeric input variables resulting from a PCA transformation. Regrettably, owing to confidentiality constraints, we are unable to furnish the original features and additional contextual details about the data. The features V1, V2, … V28 represent the principal components derived through PCA. The only features exempt from PCA transformation are 'Time' and 'Amount'. The 'Time' feature denotes the seconds elapsed between each transaction and the initial transaction in the dataset. The 'Amount' feature represents the transaction amount and can be utilized for instance-dependent cost-sensitive learning. The 'Class' feature serves as the response variable, assuming a value of 1 in instances of fraud and 0 otherwise.
2. Check for the duplicate and null values, drop them.


### VISUALISATION:

1. I have used boxplots, correlation matrix, basic plots (combined together as subplots for each feature)
 and bar charts.

 ### MODELLING:

1. Set the target and response variable, perform standardisation.
2. Since the dataset is highly imbalanced, I am also performing a method of oversampling known as SMOTE (Synthetic Minority Oversampling Technique).
3. Different models such as:
   (a) Logistic Regression


   (b) Random Forest
   (c) Naive Bayes
   (d) Decision trees
   (e) K-means Nearest Neighbour (KNN)
   (f) XGBOOST
Additionally I have used another classifier known as the dummy classifier, to show the classifiers comparison.

### MODEL COMPARISON:

Compared using the following:
(a) ROC curves 
(b) Best Threshold, F1 Score,	Accuracy,	Recall,	Precision
(c) Confusion Matrix 
