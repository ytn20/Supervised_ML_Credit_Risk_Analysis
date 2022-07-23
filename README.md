# Supervised_ML_Credit_Risk_Analysis


# Purpose

The purpose of this project is to use different Supervised Machine Learning models to predict the credit card risk. 

Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. There are many different models—a model is a mathematical representation of something that happens in the real world. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. 

We oversample the data using the **RandomOverSampler** and **SMOTE** algorithms, and undersample the data using the ClusterCentroids algorithm. In this analysis we also use a combinatorial approach of oversampling and undersampling  the data using the SMOTEENN algorithm which combines the SMOTE and Edited Nearest Neighbors (ENN) algorithms. 

Lastly, we also use two machine leanring models **BalancedRandomForestClassifier** and **EasyEnsemleClassifier** that reduce bias to predict credit risk rates. By calculating the **_balaced accuracy scores_**, **_precision and recall scores_** as well as tools like **_confusion matrix_** and **_imbalanced classification reports_** we can furthur analyze the outcomes of our Supervised Machine Learning models.

# Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models 15

# Summary:

There is a summary of the results 
There is a recommendation on which model to use, or there is no recommendation with a justification 
