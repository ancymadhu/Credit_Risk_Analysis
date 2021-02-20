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

The bulleted list below describes the balanced accuracy score and the precision and recall scores of all six machine learning models used in this analysis.

### I. RandomOverSampler Model

![Naive Random](https://user-images.githubusercontent.com/73450637/108589699-a7bf8080-732d-11eb-9bdf-dc030f77a656.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 64.61% |
| Precision Score | High risk has low poitivity of just 1% |
| Recall Score | For high risk it is 63% |


### II. SMOTE Model

![Smote Oversampling](https://user-images.githubusercontent.com/73450637/108589713-b6a63300-732d-11eb-8f3f-acdec92d975d.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 62.88% |
| Precision Score | High risk has low poitivity of just 1% |
| Recall Score | For high risk it is 60% |

### III. ClusterCentroids Model

![Undersampling](https://user-images.githubusercontent.com/73450637/108589715-ba39ba00-732d-11eb-9ce3-3c48ef05f63d.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 51.59% |
| Precision Score | High risk has low poitivity of just 1% |
| Recall Score | For high risk it is 60% |

### IV. SMOTEENN Model / Combination (Over and Under) Sampling

![Over and Under](https://user-images.githubusercontent.com/73450637/108589712-b4dc6f80-732d-11eb-8181-19ad700cc395.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 62.91% |
| Precision Score | High risk has low poitivity of just 1% |
| Recall Score | For high risk it is 72% |

### V. BalancedRandomForestClassifier Model

![Balanced Random Classifier](https://user-images.githubusercontent.com/73450637/108589703-ad1ccb00-732d-11eb-9070-7177e32b2714.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 78.77% |
| Precision Score | High risk has low poitivity of 4% |
| Recall Score | For high risk it is 67% |

### VI. EasyEnsembleClassifier Model

![Easy Ensemble  D3, b](https://user-images.githubusercontent.com/73450637/108589711-b148e880-732d-11eb-9103-dee8b2a02783.png)

| Quantities | Values |
| --- | --- |
| Balanced Accuracy Score | 92.54% |
| Precision Score | High risk has low poitivity of 7% |
| Recall Score | For high risk it is 91% |

## Summary

`
The first four sampling models have comparatively low accuracy score compared to the last two classifier models that we used. The sampling models had an accuracy in 60's range while the classifer models had accuracy levels of 78.77 and 92.54 percetanges each. Typically in our models we want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
