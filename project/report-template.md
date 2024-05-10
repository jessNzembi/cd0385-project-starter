# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Jessica Gatura

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The output of the predictor needed to have no negative values for the predicions to be submited. Mine did not have any negatives so I did not neet to make any changes.

### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
With EDA I found out that the target value, count, was skewed hence the model was prone to bias.
I added more features by splitting the datetim column into year, month and day

### How much better did your model preform after adding additional features and why do you think that is?
Adding more features provided more data points for my model. Due to this it was able to make better predictions and the score significantly increased.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The model's performance slightly dropped after trying different hyperparameters. This indicates that the adjustments made did not lead to an improvement in the model's predictive capabilities. It suggests that the original hyperparameters might have been closer to the optimal configuration for the given dataset and task

### If you were given more time with this dataset, where do you think you would spend more time?
I would spend more time on hyperparameter tuning in order to find the combination of hyperparameters that makes my model make the most accurate predictions.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|time_limit|?|?|1.74993|
|add_features|time_limit|?|?|0.70208,|
|hpo|time_limit|auto_stack|num_bag_sets|0.73967|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.


![model_test_score.png](img/model_test_score.png)

## Summary
Further refinement and fine-tuning of hyperparameters may be needed to achieve better performance.
