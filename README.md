# Credit_Risk_Analysis

For this deliverable, you’ll write a brief summary and analysis of the performance of all the machine learning models used in this Challenge.

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. 
Use screenshots of your outputs to support your results.

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not 
recommend any of the models, justify your reasoning.

-----------------------------------------------------------------------------------

## Credit Risk Analysis Overview

The purpose of this analysis is to use machine learning to create models which can predict outcomes using several different algoriths. Those 
algorithms are RandomOverSampler, SMOTE, ClusterCentroids, and a combination algorithm called SMOTEENN.

We then compare two different models of BalancedRandomForestClassifier and EasyEnsembleClasifier. We can then check the performance of the models 
and if they should be used for predicting risk.


## Results

### RandomOverSampler

[Random OverSampler as and pr]

The balanced accuracy score for the RandomOverSampler method is 63%.
The precision is 99% and the sensitivity (recall) is 67%.


### SMOTE

[SMOTE as and pr]

The balanced accuracy score for the SMOTE method is 63%.
The precision is 99% and the sensitivity (recall) is 65%.


### UnderSampling

[Undersampling as and pr]

The balanced accuracy score for the UnderSampling method is 52%.
The precision is 99% and the sensitivity (recall) is 47%.


### SMOTEENN

[COMBO as and pr]

The balanced accuracy score for the SMOTEENN method is 62%.
The precision is 99% and the sensitivity (recall) is 55%.


### BalancedRandomForestClassifier

[Forest as and pr]

The balanced accuracy score for the BalancedRandomForestClassifier method is 79%.
The precision is 99% and the sensitivity (recall) is 91%.


### EasyEnsembleClassifier

[EasyEnsemble as and pr]

The balanced accuracy score for the EasyEnsembleClassifier method is 93%.
The precision is 99% and the sensitivity (recall) is 94%.


## Summary

These models created within this analysis have an obvious shortfall; high risk credit assessment. The above figures are for the 
averages of all scores, but the fallicy comes into play with the high risk numbers. The low risk assesments of the model are very 
accurate, however.

The Ensemble models definetly differ from the others in the area of precision. The EasyEnsemble method high risk in particular shows a 
91% recall, with only a 7% precision. What does this mean? We will see more False Positives in this scenario.

All of these models have prediction fallacies, expecially in the high risk assesments. I do not believe that the investment is considered safe, 
as the precisions are so low and the credit could default, costing the institutions more in funding and on-hand resources.