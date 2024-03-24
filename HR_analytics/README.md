**Project: predicting the level of employee's satisfaction and the quit's likelihood**

*The goal of the project: to help businesses optimize personnel management, avoid financial losses and employee's outflows.*

*Project objectives: The first task was to build a model for prediction the level of employee satisfaction based on customer data. The second task was to build a model that can, based on customer data, predict that an employee will leave the company*

The dataset describes employees of the company. job_satisfaction_rate — the first target feature; quit- the second target feature

 A pipeline (linear regression and a decision tree regressor)  was used to predict employee job satisfaction. The hyperparameters of the models were specified. smape was used  as metric   with a success criterion of less than or equal to 15%. The best model turned out to be DecisionTreeRegressor. 
The portrait of resigned employee was composed, it can be described as follows: an employee who has worked for a short time in the company (1-3 years), with junior level, low salary, average rating from the employer, low workload, has not had promotions and may have had penalties.

To predict a probability of quit the following models were selected: logistic regression, KNN, support vector machine and decision tree whith ROC-AUC-score and a success criterion greater than or equal to 91% on the test sample. The best model was DecisionTreeClassifier
