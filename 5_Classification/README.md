# <p align="center"> Supervised Learning: Classification </p>

<p align="center"><img src =https://media.istockphoto.com/id/1194242628/vector/business-people-clients-and-bank-staff-on-workplace-bank-managers-and-customers-characters.jpg?s=612x612&w=0&k=20&c=gSQgpGabj1KmPXAI0x0Hf4yGVUyP8ARwuRDPjROXLp0=></p>

# <p align="center"> Logistic Regression, Decision Tree, Random Forest </p>

## Content
[1. Project description](README.md#project-description)

[2. Dataset](README.md#dataset)

[3. Technologies](README.md#technologies)

[4. Credits and Contacts]()

## Project description

A bank is seeking for help: they want to develop a loyalty campaign to retain their customers. To do this, bank wants to predict the probability of customers churn and determine whether the customer will leave in the near future. 

The task is to build the classifier that will allow timely identification of leaving the bank customers, assess the quality of the created models and interpret the results.

The best following results have been achieved:

|**Model**|**Train Recall**|**Train F1 Score**|**Test Recall**|**Test F1 Score**|
|:--|:--|:--|:--|:--|
|Random Forest|0.64|0.90 / 0.73|0.56|0.85 / 0.64|
|Random Forest (threshold = 0.37)| - | - |0.75|0.84 / 0.70|

[To the top](README.md#content)


## Dataset 

This dataset has been reviewed, cleaned and used in the project [Visualization poject](https://github.com/KonovalovaDS/SKILLFACTORY/tree/master/1_Visualization). Please click for more details. 

Each customer is described by the following features:

|**Name of feature**|**Feature description**|
|:---|:---|
|RowNumber|Number of the row in data frame|
|CustomerID|Identification of the customer|
|Surname|Surname of the customer|
|CreditScore|Customer credit score (the higher it is, the more the customer took loans and returned them)|
|Geography|Customer country of residency (Bank is international)|
|Gender|Gender of the customer|
|Age|Age of the customer|
|Tenure|How many years the customer has been using the bank|
|Balance|How much money is on the accounts of the customer in the bank|
|NumOfProduct|Number of bank services the customer is using|
|HasCrCard|Has the customer bank credit card (1 - yes; 0 - no)|
|IsActiveMember|Does customer have status "active client" (1 - yes; 0 - no)|
|EstimatedSalary|Estimated salary of the customer|
|Exited|Status of the customer (1 - left customer, 0 - loyal customer) - **target feature**|

[To the top](README.md#content)

## Technologies

The following tolls and techniques have been used:

- Logistic Regression;
- RobustScaler;
- Decision Tree Classifier;
- Random Forest Classifier.

[To the top](README.md#content)

## Credits and Contacts

Credits to SkillFactory team of mentors and coordinators. Special appreciation to Sergey Dobdin and Maria Zharova.

*<p align="center">[Email](natalia_konovalova@icloud.com)</p>*

*<p align="center">[Kaggle](https://www.kaggle.com/nataliamantyk)</p>* 

*<p align="center">[LinkedIn](https://www.linkedin.com/in/natalia-ds-198612241)</p>*

[To the top](README.md#content)