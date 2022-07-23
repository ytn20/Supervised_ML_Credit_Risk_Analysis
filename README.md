# Supervised_ML_Credit_Risk_Analysis


# Project Purpose and Overview

## Purpose

The purpose of this project is to use different Supervised Machine Learning models to predict the credit card risk. Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. There are many different models—a model is a mathematical representation of something that happens in the real world. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. 

## Overview
We oversample the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the **ClusterCentroids** algorithm. In this analysis we also use a combinatorial approach of oversampling and undersampling  the data using the **SMOTEENN** algorithm which combines the **SMOTE** and **Edited Nearest Neighbors (ENN)** algorithms. 

Lastly, we also use two machine leanring models **BalancedRandomForestClassifier** and **EasyEnsemleClassifier** that reduce bias to predict credit risk rates. By calculating the **_balaced accuracy scores_**, **_precision and recall scores_** as well as tools like **_confusion matrix_** and **_imbalanced classification reports_** we can furthur analyze the outcomes of our Supervised Machine Learning models.

# Results:
## Oversampling

### Naive Random Oversampling
- The balanced accuracy score for this model is approximately 64.13% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 60%
- The F1 score for this model is approximately 2%


### SMOTE Oversampling
- The balanced accuracy score for this model is approximately 63.75% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 60%
- The F1 score for this model is approximately 2%

## Undersampling

### Cluster Centroids algorithm
- The balanced accuracy score for this model is approximately 52.92% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 61%
- The F1 score for this model is approximately 1%

## Combination (Over and Under) Sampling

### SMOTEENN algorithm
- The balanced accuracy score for this model is approximately 63.76% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 70%
- The F1 score for this model is approximately 2%
-
## Ensemble Learners

### Balanced Random Forest Classifier
- The balanced accuracy scores for this model is approximately 99.51%
- The precision score for this model is approximately 58%
- The recall score for this model is approximately 32%
- The F1 score for this model is approximately 41%

### Easy Ensemble AdaBoost Classifier

- The balanced accuracy scores for this model based on learning rate are as follows
    - **Learning rate:  5%**
      - Accuracy score (training): 0.997
      - Accuracy score (validation): 0.995

    - **Learning rate:  1%**
      - Accuracy score (training): 0.997
      - Accuracy score (validation): 0.995
  
    -  **Learning rate:  25%**  
      - Accuracy score (training): 0.996
      - Accuracy score (validation): 0.994
  
    -  **Learning rate:  50%**
      - Accuracy score (training): 0.996
      - Accuracy score (validation): 0.994

    -  **Learning rate:  75%**
      - Accuracy score (training): 0.994
      - Accuracy score (validation): 0.991
   
    -  **Learning rate:  100%**
      - Accuracy score (training): 0.995
      - Accuracy score (validation): 0.994

- The balace accuracy score for this model is approximately 99.45%
- The precision score for this model is approximately 48%
- The recall score for this model is approximately 34%
- The F1 score for this model is approximately 39%



# Summary:

Based on the summary reports the supervised machine learning model with the highest accuracy score is BalancedRandomForestClassifer and the model with the lowest accuracy score is Cluster Centroids Algorithm. Overall the  Ensemble Learners models are far more accurate than combined and over and undersample models. For future analysis would be recommended to run the Ensemble Learners model either BalancedRandomForestClassifer or Easy Ensemble AdaBoost Classifier to get the most accurate predictions.

- Balanced Random Forest Classifier - 99.51%
- Easy Ensemble AdaBoost Classifier - 99.45%
- Naive Random Oversampling - 64.13% 
- SMOTEENN algorithm - 63.76% 
- SMOTE Oversampling - 63.75% 
- Cluster Centroids algorithm - 52.92%


