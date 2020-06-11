# Santander-Customer-Satisfaction

### Problem Statement
When we have a classification problem, an imbalanced dataset brings forth a set of issues. Our models, after being trained on the dataset, do not see much of the minority class points and hence fail to proprely classify the test data points-especially the ones of the minority class. The high accuracy scores presented by the model metrics are misleading - one should look at the precision and recall scores of each of the classes to properly evaluate the model peformance. The area under the curve of the receiver operating charecteristic (also known as auc_roc) is the metric we seek to maximize here.

### Dataset
The dataset chosen for this project is from kaggle. Link :https://www.kaggle.com/c/santander-customer-satisfaction

The description on the Kaggle website is 

*"From frontline support teams to C-suites, customer satisfaction is a key measure of success. Unhappy customers don't stick around. What's more, unhappy customers rarely voice their dissatisfaction before leaving.*
*Santander Bank is asking Kagglers to help them identify dissatisfied customers early in their relationship. Doing so would allow Santander to take proactive steps to improve a customer's happiness before it's too late.*
*In this competition, you'll work with hundreds of anonymized features to predict if a customer is satisfied or dissatisfied with their banking experience."*

### Approach
1. Data Preprocessing
2. Vanilla decision tree model - No data manipulation
3. Resampling Technqiues
	1. Under-sampling of majority class points
	2. Over-sampling of minortiy class points
		1. using repititon
		2. using SMOTE
	3. Both under-sampling and over-sampling of data
  
 **Note : There are a lot of ways to deal with imbalanced data, this project only explores the various kinds of data sampling techniques**
 
### End Result

To evaluate our approaches, we assess both the training auc_roc scores as well the testing auc_roc scores (by uploading the predictions to kaggle)
