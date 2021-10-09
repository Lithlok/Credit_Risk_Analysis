# Credit Risk Analysis Overview

The purpose of this analysis is to use machine learning to create models which can predict outcomes using several different algoriths. Those 
algorithms are RandomOverSampler, SMOTE, ClusterCentroids, and a combination algorithm called SMOTEENN.

We then compare two different models of BalancedRandomForestClassifier and EasyEnsembleClasifier. We can then check the performance of the models 
and if they should be used for predicting risk.


# Results

### RandomOverSampler

![RandomOverSampler as](https://user-images.githubusercontent.com/85216568/136641270-4fe29b71-eec0-41e6-95e7-84867aab4381.PNG)
![RandomOverSampler pr](https://user-images.githubusercontent.com/85216568/136641274-3faf0c33-7f9f-4220-8fd0-a999dbfa8984.PNG)

The balanced accuracy score for the RandomOverSampler method is 63%.
<br> The precision is 99% and the sensitivity (recall) is 67%.


### SMOTE

![SMOTE as](https://user-images.githubusercontent.com/85216568/136641291-d1a6d594-c45f-424e-8aa3-3cbc05157717.PNG)
![SMOTE pr](https://user-images.githubusercontent.com/85216568/136641293-11fc7c85-4e8f-4566-8dc4-b10646b5d55d.PNG)

The balanced accuracy score for the SMOTE method is 63%.
<br> The precision is 99% and the sensitivity (recall) is 65%.


### UnderSampling

![Undersampling as](https://user-images.githubusercontent.com/85216568/136641302-ad02ebf4-cf47-4397-8d8c-0cc8b03fc816.PNG)
![Undersampling pr](https://user-images.githubusercontent.com/85216568/136641303-dda0e9dc-7529-4da8-824b-203cf2c2c7b0.PNG)

The balanced accuracy score for the UnderSampling method is 52%.
<br> The precision is 99% and the sensitivity (recall) is 47%.


### SMOTEENN

![Combo as](https://user-images.githubusercontent.com/85216568/136641307-37a84b27-e2d9-483f-8976-6cb4ebe77ca5.PNG)
![Combo pr](https://user-images.githubusercontent.com/85216568/136641311-a659904c-3c62-43b0-a51b-fd82837e3000.PNG)

The balanced accuracy score for the SMOTEENN method is 62%.
<br> The precision is 99% and the sensitivity (recall) is 55%.


### BalancedRandomForestClassifier

![Forest as](https://user-images.githubusercontent.com/85216568/136641331-70e02fa4-972e-429c-b3e2-a9ccd882e76e.PNG)
![Forest pr](https://user-images.githubusercontent.com/85216568/136641336-9683a871-bf3e-46de-8b87-5f315dd6db1f.PNG)

The balanced accuracy score for the BalancedRandomForestClassifier method is 79%.
<br> The precision is 99% and the sensitivity (recall) is 91%.


### EasyEnsembleClassifier

![EasyEnsemble as](https://user-images.githubusercontent.com/85216568/136641347-e1657db6-151a-413e-8005-29cfb0e4b914.PNG)
![EasyEnsemble pr](https://user-images.githubusercontent.com/85216568/136641350-552a9fe2-9c14-4114-a3b5-7cd683229a04.PNG)

The balanced accuracy score for the EasyEnsembleClassifier method is 93%.
<br>The precision is 99% and the sensitivity (recall) is 94%.


# Summary

These models created within this analysis have an obvious shortfall; high risk credit assessment. The above figures are for the 
averages of all scores, but the fallicy comes into play with the high risk numbers. The low risk assesments of the model are very 
accurate, however.

The Ensemble models definitely differ from the others in the area of precision. The EasyEnsemble method high risk in particular shows a 
91% recall, with only a 7% precision. What does this mean? We will see more False Positives in this scenario.

All of these models have prediction fallacies, expecially in the high risk assesments. I do not believe that the investment is considered safe, 
as the precisions are so low and the credit could default, costing the institutions more in funding and on-hand resources.
