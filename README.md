# credit-risk-classification
#To receive all points, you must:

Provide an overview that explains the purpose of this analysis. (5 points)

Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)

Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

This credit risk analysis uses a logistic regression model to train and test a data set that predicts if a loan is going to be healthy or high risk. This is useful for companies to decide weather to provide customers with the loan amount or to deny the loan request. 

First step is to seperate the data into our X (dependent variables), and y (independednt variables). We can then calssify them as X_test, X_train, y_test, y_train to have a subset to train and test the model with. The first model scores can be viewed in a confustion matrix. 

- Accuracy measures the percentage of correctly classified instances (both true positives and true negatives) out of the total number of instances in the dataset. Accuracy = (Number of Correct Predictions) / (Total Number of Predictions)
- Precision is a metric that focuses on the true positive predictions out of all the positive predictions made by the model. It indicates the model's ability to avoid false positives.
Precision = (Number of True Positives) / (Number of True Positives + Number of False Positives)
- Recall (Sensitivity or True Positive Rate):
Recall measures the percentage of true positive instances captured by the model out of the total actual positive instances in the dataset. It is particularly important when we want to minimize false negatives.
Recall = (Number of True Positives) / (Number of True Positives + Number of False Negatives)

The F1 score is the harmonic mean of precision and recall, can also be used to evaluate the model's performance comprehensively.

Our results for the first model had 0, helathy loan predictions at 100% for precision and recall. The 1, unhealthy loan hada score of 0.87 for precision, and 0.89 for recall. This means the model correctly predicted 89% of the truely unhealthy loans. Overall it had an accuracy or F1 of 0.88

When running the model again on the overfitted and resampled training data, the model correctly predicted 100% of the truley unhealthy loans. This was represented by a recall score of 1.00. Overall it had an accuracy or F1 of 0.93. I would recommend the refitted model to be used. 