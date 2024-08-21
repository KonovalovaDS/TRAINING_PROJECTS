# <p align="center"> Various Methods to Optimize Hyperparameters

<p align="center"><img src = https://content.presspage.com/uploads/2170/6ae61bb5-ba0c-4eb0-b454-3c0073303768/1920_gettyimages-1182189621.jpg?10000></p>

# <p align="center"> Predicting a Biological Response

## Content
[1. Project description](README.md#project-description)

[2. Dataset](README.md#dataset)

[3. Conclusion](README.md#conclusion)

[4. Contacts](README.md#contacts)

## Project description

The target of the project is to review the performance of various hyperparameters optimization methods from the perspective of:
- model metrics improvement; and
- timing spent for each hyperperameters optimization technique.

Classification Models:
- Random Forest;
- Logistic Regression.

Metric: F1-Score

Hyperparameters methods used for both models:
- GridSearchCV;
- RandomizedSearchCV;
- Hyperopt;
- Optuna.

[To the top](README.md#content)

## Dataset

It is required to predict the biological response of molecules (column "Activity") from their chemical composition (columns D1 - D1776). Each row represents a molecule.

The first Activity column contains experimental data describing the actual biological response [0, 1];

The remaining columns D1-D1776 are molecular descriptors, which are computed properties that can capture some characteristic of a molecule, such as size, shape, or elemental composition.

[To the top](README.md#content)

## Conclusion
**Summary of achieved results for Rendom Forest Classifier Model:**

|**Method**|**Parameters**|**F1 Train**|**F1 Test**|**F1 cross-validation**|**Timing**|
|:--|:--|:--|:--|:--|:--|
|Baseline|Default Parameters|1.0000|0.8126|0.8132|---|
|GridSearchCV|criterion: entropy|0.9942|0.8238|0.7983|15 min 11 sec|
|            |max_depth: 25|
|            |min_samples_leaf: 2|
|            |n_estimators: 110|
|RandomizedSearchCV|criterion: entropy|0.9945|0.8196|0.7970|1 min 27 sec|
|                  |max_depth: 40|
|                  |min_samples_leaf: 2|
|                  |n_estimators: 170|
|Hyperopt|criterion: entropy|0.9933|0.8268|0.8139|4 min 22 sec|
|        |max_depth: 36|
|        |min_samples_leaf: 2|
|        |n_estimators: 210|
|Optuna  |criterion: gini|0.9920|0.8192|0.8181|4 min 52 sec|
|        |max_depth: 23|
|        |min_samples_leaf: 2|
|        |n_estimators: 175|

**Summary of achieved results for Logistic Regression Model:**

|**Method**|**Best Parameters**|**F1 Train**|**F1 Test**|**F1 cross-validation**|**Timing**|
|:--|:--|:--|:--|:--|:--|
|Baseline|Default Parameters|8.8849|0.7808|0.7759|---|
|GridSearchCV|C: 0.2|0.8157|0.7830|0.7827|22 min 52 sec|
|            |penalty: l2|
|            |solver: liblinear|
|RandomizedSearchCV|C: 0.05|0.8370|0.7967|0.7823|5 min 46 sec|
|                  |max_depth: 40|
|                  |min_samples_leaf: 2|
|                  |n_estimators: 170|
|Hyperopt|space_1|0.9193|0.7597|0.7596|5 min 15 sec|
|        |C: 0.07|
|        |penalty: l2|
|        |solver: lbfgs|
|Hyperopt|space_2|0.9005|0.7707|0.7703|13 min 03 sec|
|        |C: 0.03|
|        |penalty: l2|
|        |solver: saga|
|Optuna  |space_1|0.8545|0.7866|0.7824|6 min 38 sec|
|        |C: 0.14|
|        |penalty: l2|
|        |solver: sag|
|Optuna  |space_2|0.8545|0.7866|0.7916|18 min 54 sec|
|        |C: 0.03|
|        |penalty: l2|
|        |solver: liblinear|

**Logistic Regression** with build in **cross validation** on the initial run of the model showed F1 score 0.8368. With Optuna hyperparameters search showed F1 metric as 0.9779, but timing was 4 hours 15 min

[To the top](README.md#content)

## Contacts

*<p align="center">[Email](natalia_konovalova@icloud.com)</p>*

*<p align="center">[Kaggle](https://www.kaggle.com/nataliamantyk)</p>* 

*<p align="center">[LinkedIn](https://www.linkedin.com/in/natalia-ds-198612241)</p>*

[To the top](README.md#content)