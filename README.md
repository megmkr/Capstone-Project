# Capstone-Project
This document presents details on the process and results of creating a machine learning model to predict employee retention using data that encompasses an employee’s satisfaction, work conditions, and tenure. We have evalutated the performance of two models: Random Forest and XGBoost to enhance further exploratory research.

## Problem
High employee retention rates typically reflect a satisfied, engaged workforce, which is essential for sustainable growth. To support this effort, we will develop an employee retention model aimed at reducing turnover and proactively identifying employees at risk of leaving. A reliable and accurate model will not only help prevent unwanted attrition but also uncover the key factors that influence retention. Specifically, the model will help answer critical questions such as:
Which employees are most likely to quit or be terminated?
What factors contribute to employees leaving the company?
What actions can the organization take to improve retention?

* ## Response
* The team developed two supervised machine learning models to classify whether a user is likely to churn or not. We decided the best models to use were:
Random Forest and XGBoost.
These models are known for creating accurate and reliable predictions and require little preprocessing or transforming of the data, allowing us to speed the
model creation process along.
For preparation, we split the available data into three groups: training, validating, and testing. This allows us to train and test each individual model, then evaluate its performance using data that it has never seen before. This allows us to accurately predict future user patterns, without the risk of overfitting the model on historical data. Using an interative process, we tuned the parameters of each model to ensure the most accurate version of each.

## Model Summary
The final model has produced highly accurate results. We can be assured of correct categorization of employee retention when using this model.
The F1 score is a single metric that tells you how well a machine learning model performs by balancing two competing requirements: precision (avoiding false alarms) and recall (not missing important cases).
The provided model has a .95 F1 score, a near perfect result.
As displayed by the blue line in the ROC curve, the false positive rate is near 0% while the true positive rate is near 100%. 
A perfect model would be a point in the upper left corner.

## Conclusion
Above everything, satisfaction levels are most imperative to employee retention. I reccomend that we prioritize employee satisfaction as well as better distributing projects across employees. Being overworked is a driving factor in employee retention as well.
The model has a 98% precision, meaning it almost never falsely predicts an employee to leave when they were not going to. However, false negatives are slightly more likely to happen. The model can be improved perhaps by adding nonlinear features. This can include an overworked tag, seniority tag, or a feature that is determined by sasisfaction_level and project thresholds rather than a ratio.
We could do further research into being able to predict satisfaction since that is the leading factor of employee retention. If we are able to see the leading features then we can make the proper accomdations.

