# Credit Card Customer Leads Prediction

## Introduction

Credit risk has been considered a great hurdle by most financial institutions around the world, making it a crucial financial aspect that needs to be closely monitored and managed from time to time. Institutions are constantly faced with uncertainty about borrowers' ability to repay their debt which poses a threat of defaulted loans and unexpected financial losses. 
Addressing such challenges is crucial to implementing measures to minimize potential losses from customers with a higher default risk. Companies are encouraged to assess individuals' financial reliability through the five C's of credit—character, capacity, capital, collateral, and conditions—to gauge their ability to meet debt obligations promptly.
With this in mind, we desire to build a model to identify potential credit card customers among existing account holders to give financial institutions a better target on customers and give a general overview of which customers may have an interest in purchasing credit cards based on credit features evaluated. 

## Data Collection

The data utilized in this project was obtained from an unknown bank's database and also, utilized publicly available demographics and economic data on level county as a supplementary dataset to enhance the available dataset.
The dataset includes different aspects of customer information which includes an individual’s age, gender, occupation, past records of credit, occupation, income, and state residence, among other attributes essential for a bank’s KYC.

## Data Preprocessing

KNN Imputer for missing data
IQR for outliers capping
Min-Max scaler for normalized numeric features (After Train Test Split)

## Model Fitting & Evaluation

The Binary Classification Models listed were run on the dataset using 5-fold cross-validation.
Multiple Binary Machine Learning Classifiers plus Neural Networks were trained and evaluated on each fold.

The model with the highest average ROC AUC score was chosen as the best performer, which was the Light GBM model.
ROC and AUC scores were chosen because predictive ability to measure a model across all classification thresholds and are less affected by imbalanced data compared to other metrics, such as accuracy.
The selected model was trained on the entire Train dataset and tested on an independent Test set for final evaluation and generalization and further Hyper-Tuned using Parameter Grid Search.



