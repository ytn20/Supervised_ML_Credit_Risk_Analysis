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

![1_cr](https://user-images.githubusercontent.com/100486461/180588193-44ba4f6a-2fc4-4f18-b8f9-3d172e7c6248.PNG)
![1_as](https://user-images.githubusercontent.com/100486461/180588194-160546bb-bff3-4526-824e-23f7d9f243ff.PNG)
![1_cm](https://user-images.githubusercontent.com/100486461/180588195-dfea32d6-a887-479c-9024-3a2c8c0cc31a.PNG)

### SMOTE Oversampling
- The balanced accuracy score for this model is approximately 63.75% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 60%
- The F1 score for this model is approximately 2%
![2_cr](https://user-images.githubusercontent.com/100486461/180588202-8661519c-7e90-4700-a5b4-d553c8d34a1c.PNG)
![2_as](https://user-images.githubusercontent.com/100486461/180588203-e093f858-28ab-4ad3-95db-af3ad1f00233.PNG)
![2_cm](https://user-images.githubusercontent.com/100486461/180588204-0efd37db-4d71-4f7d-8f50-fd9a2c50d578.PNG)

## Undersampling

### Cluster Centroids algorithm
- The balanced accuracy score for this model is approximately 52.92% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 61%
- The F1 score for this model is approximately 1%
![3_cr](https://user-images.githubusercontent.com/100486461/180588209-74bc99fb-5328-4baa-919b-64fc648848ef.PNG)
![3_as](https://user-images.githubusercontent.com/100486461/180588210-1a3c4c91-8cae-48bd-b42e-e129672530a6.PNG)
![3_cm](https://user-images.githubusercontent.com/100486461/180588211-6519ad4b-2238-484d-b60b-6afb9d0db1ed.PNG)

## Combination (Over and Under) Sampling

### SMOTEENN algorithm
- The balanced accuracy score for this model is approximately 63.76% 
- The precision score for this model is approximately 1%
- The recall score for this model is approximately 70%
- The F1 score for this model is approximately 2%
![4_cr](https://user-images.githubusercontent.com/100486461/180588222-7fb3932e-4b64-4dee-9d67-eb1f77527845.PNG)
![4_as](https://user-images.githubusercontent.com/100486461/180588223-22c126fb-c4c9-4f4e-b3a2-5bf10462fb86.PNG)
![4_cm](https://user-images.githubusercontent.com/100486461/180588224-a1165897-6893-4b27-8b88-cc8abcc47cfc.PNG)


## Ensemble Learners

### Balanced Random Forest Classifier
- The balanced accuracy scores for this model is approximately 99.51%
- The precision score for this model is approximately 58%
- The recall score for this model is approximately 32%
- The F1 score for this model is approximately 41%
![5_cr](https://user-images.githubusercontent.com/100486461/180588230-7672fee9-297b-4750-a46e-6c99bc01eed2.PNG)
![5_as](https://user-images.githubusercontent.com/100486461/180588231-cc05dc56-6dfe-44ef-96e9-2416b1358f49.PNG)
![5_cm](https://user-images.githubusercontent.com/100486461/180588232-5118b1b8-e32a-415a-8596-a5d84a43b06b.PNG)

### Easy Ensemble AdaBoost Classifier

- The balanced accuracy scores for this model based on learning rate are as follows
    - **Learning rate:  5%**
      - Accuracy score (training): 0.997
      - Accuracy score (validation): 0.995

    - **Learning rate:  1%**
      - Accuracy score (training): 0.997
      - Accuracy score (validation): 0.995
  
    -  **Learning rate:  25%**
            -  Accuracy score (training): 0.996
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

![6_cr](https://user-images.githubusercontent.com/100486461/180588237-c077672c-629b-4a8a-9324-b322dce2a83a.PNG)
![6_as](https://user-images.githubusercontent.com/100486461/180588238-10017e5c-10d6-4ad9-a1ae-0f5f7b597b82.PNG)
![6_cm](https://user-images.githubusercontent.com/100486461/180588239-02a303d2-cd1e-47cf-a465-6578eacd7b47.PNG)


# Summary:

Based on the summary reports the supervised machine learning model with the highest accuracy score is BalancedRandomForestClassifer and the model with the lowest accuracy score is Cluster Centroids Algorithm. Overall the  Ensemble Learners models are far more accurate than combined and over and undersample models. For future analysis would be recommended to run the Ensemble Learners model either BalancedRandomForestClassifer or Easy Ensemble AdaBoost Classifier to get the most accurate predictions.

![1_as](https://user-images.githubusercontent.com/100486461/180588249-422f729e-2812-4487-a18c-a1ff981a0bee.PNG)
![2_as](https://user-images.githubusercontent.com/100486461/180588250-8586674d-69df-41ce-b6e5-59984a2f8058.PNG)
![3_as](https://user-images.githubusercontent.com/100486461/180588251-4e9da9d7-7742-4677-9fe9-9f6dd702e898.PNG)
![4_as](https://user-images.githubusercontent.com/100486461/180588252-4472b999-f5c5-4a78-bae7-2aa0dcdfa6a4.PNG)
![5_as](https://user-images.githubusercontent.com/100486461/180588253-80dc0a10-d1c7-46a7-a7fe-b7dbc6129906.PNG)
![6_as](https://user-images.githubusercontent.com/100486461/180588254-ba9ce334-b2f9-4e70-8be0-b6631efc9ee7.PNG)


- Balanced Random Forest Classifier - 99.51%
- Easy Ensemble AdaBoost Classifier - 99.45%
- Naive Random Oversampling - 64.13% 
- SMOTEENN algorithm - 63.76% 
- SMOTE Oversampling - 63.75% 
- Cluster Centroids algorithm - 52.92%


