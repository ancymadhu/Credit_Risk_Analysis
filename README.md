# Credit_Risk_Analysis
![1](https://user-images.githubusercontent.com/73450637/108589078-9d4fb780-732a-11eb-8d0f-05189dad7199.png)

## Analysis Overview
In this project, we use Python to build and evaluate several machine learning models to predict credit risk.

We adopted the following procedure:

* Oversample the data using the RandomOverSampler and SMOTE algorithms.
* Undersample the data using the ClusterCentroids algorithm.
* Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
* Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.
