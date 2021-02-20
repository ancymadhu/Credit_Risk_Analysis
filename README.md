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

## Resources

* Data Source: LoanStats_2019Q1.csv
* Software: Python 3.7.9, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results

The bbulleted list below describes the balanced accuracy score and the precision and recall scores of all six machine learning models used in this analysis.

### I. RandomOverSampler Model

![Naive Random](https://user-images.githubusercontent.com/73450637/108589699-a7bf8080-732d-11eb-9bdf-dc030f77a656.png)


### II. SMOTE Model

![Smote Oversampling](https://user-images.githubusercontent.com/73450637/108589713-b6a63300-732d-11eb-8f3f-acdec92d975d.png)

### III. ClusterCentroids Model

![Undersampling](https://user-images.githubusercontent.com/73450637/108589715-ba39ba00-732d-11eb-9ce3-3c48ef05f63d.png)

### IV. SMOTEENN Model / Combination (Over and Under) Sampling

![Over and Under](https://user-images.githubusercontent.com/73450637/108589712-b4dc6f80-732d-11eb-8181-19ad700cc395.png)

### V. BalancedRandomForestClassifier Model

![Balanced Random Classifier](https://user-images.githubusercontent.com/73450637/108589703-ad1ccb00-732d-11eb-9070-7177e32b2714.png)
### VI. EasyEnsembleClassifier Model
