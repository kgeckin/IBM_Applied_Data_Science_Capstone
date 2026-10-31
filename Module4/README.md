# Module 4 / Machine learning prediction

Classifier development and evaluation for Falcon 9 landing outcomes.

## Notebook

[SpaceX machine learning prediction](6-SpaceX-Machine-Learning-Prediction-Part-5-v1.ipynb)

Includes train and test splitting, hyperparameter search and comparison of Logistic Regression, SVM, Decision Tree and KNN.

## Recorded outcome

The saved notebook reports 83.3% test accuracy for all four models on an 18-record held-out sample. Cross-validation performance is not identical across models.

## Reproducibility caveat

The saved workflow scales features before splitting the data. To avoid preprocessing leakage, fit scaling inside the training folds using an sklearn Pipeline and reevaluate before comparing production suitability.

[Back to project](../README.md)
