# Credit_Risk_Analysis


## Overview of the analysis
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compareed two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results: 
### All six machine learning models:

-
![image](https://user-images.githubusercontent.com/96217224/164351814-d8e1a7a6-7b4f-40ee-931d-cfe809b8ef59.png)
-
![image](https://user-images.githubusercontent.com/96217224/164351902-e32c4f52-f241-45dc-9404-fe39bf60d234.png)

- ### Undersampling

![image](https://user-images.githubusercontent.com/96217224/164351992-88eed737-95f2-47da-b545-9945bf0b7b97.png)

- ### # Combination (Over and Under) Sampling
![image](https://user-images.githubusercontent.com/96217224/164352170-9860c555-500c-4f95-8c03-57797e617082.png)

-
![image](https://user-images.githubusercontent.com/96217224/164352293-d0c0b675-539f-41f1-af7f-5eaa6c484607.png)

-
![image](https://user-images.githubusercontent.com/96217224/164352374-9375d08f-ce3c-4877-9f5b-411179bc4849.png)

## Summary: 
This analysis is trying to find the best model that can detect if a loan is high risk or not. Becasue of that, we need to find a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk. Looking through the different models, the ones that scored the highest were: 

- Easy Ensemble Classifying (91%)
- SMOTEENN Sampling (76%)
- Naive Random Oversampling (72%)

While this is the most important statistic that is pulled from this analysis, another important statistic is recall rate for low risk as it shows how many low risk loans are flagged as high risk. Looking through the different models, the ones that scored the highest were:
- Balanced Random Forest Classifying (100%)
- Easy Ensemble Classifying (94%)

We can look at the accurary score to get a picture of how well the model performs in general. The models with the highest accuracy scores were:

- Easy Ensemble Classify (92.3%)
- SMOTEENN Sampling (68.1%)
- Balanced Random Forest Classifying (64.8%)

Factoring the three  statistics, the model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model.
