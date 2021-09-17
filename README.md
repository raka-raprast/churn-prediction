# Telco Customer Churn Prediction
Utilize and looking for the best models for predicting telco customer churn
## Dataset
IBM Telco Customer Churn Prediction : https://www.kaggle.com/yeanzc/telco-customer-churn-ibm-dataset
## Background 
Churn quantifies the number of customers who have left a brand by cancelling their subscription or stopping paying for the services. This is bad news for any business as it costs five times as much to attract a new customer as it does to keep an existing one. A high customer churn rate will hit a company’s finances hard.
## Goals
*Utilize machine learning for predicting customer churn

*Compare and choose the best Machine learning model for this case

*Model Evaluation using ROC AUC

## Data Dictionary
* CustomerID: A unique ID that identifies each customer.

* Count: A value used in reporting/dashboarding to sum up the number of customers in a filtered set.

* Country: The country of the customer’s primary residence.

* State: The state of the customer’s primary residence.

* City: The city of the customer’s primary residence.

* Zip Code: The zip code of the customer’s primary residence.

* Lat Long: The combined latitude and longitude of the customer’s primary residence.

* Latitude: The latitude of the customer’s primary residence.

* Longitude: The longitude of the customer’s primary residence.

* Gender: The customer’s gender: Male, Female

* Senior Citizen: Indicates if the customer is 65 or older: Yes, No

* Partner: Indicate if the customer has a partner: Yes, No

* Dependents: Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc.

* Tenure Months: Indicates the total amount of months that the customer has been with the company by the end of the quarter specified above.

* Phone Service: Indicates if the customer subscribes to home phone service with the company: Yes, No

* Multiple Lines: Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No

* Internet Service: Indicates if the customer subscribes to Internet service with the company: No, DSL, Fiber Optic, Cable.

* Online Security: Indicates if the customer subscribes to an additional online security service provided by the company: Yes, No

* Online Backup: Indicates if the customer subscribes to an additional online backup service provided by the company: Yes, No

* Device Protection: Indicates if the customer subscribes to an additional device protection plan for their Internet equipment provided by the company: Yes, No

* Tech Support: Indicates if the customer subscribes to an additional technical support plan from the company with reduced wait times: Yes, No

* Streaming TV: Indicates if the customer uses their Internet service to stream television programing from a third party provider: Yes, No. The company does not charge an additional fee for this service.

* Streaming Movies: Indicates if the customer uses their Internet service to stream movies from a third party provider: Yes, No. The company does not charge an additional fee for this service.

* Contract: Indicates the customer’s current contract type: Month-to-Month, One Year, Two Year.

* Paperless Billing: Indicates if the customer has chosen paperless billing: Yes, No

* Payment Method: Indicates how the customer pays their bill: Bank Withdrawal, Credit Card, Mailed Check

* Monthly Charge: Indicates the customer’s current total monthly charge for all their services from the company.

* Total Charges: Indicates the customer’s total charges, calculated to the end of the quarter specified above.

* Churn Label: Yes = the customer left the company this quarter. No = the customer remained with the company. Directly related to Churn Value.

* Churn Value: 1 = the customer left the company this quarter. 0 = the customer remained with the company. Directly related to Churn Label.

* Churn Score: A value from 0-100 that is calculated using the predictive tool IBM SPSS Modeler. The model incorporates multiple factors known to cause churn. The higher the score, the more likely the customer will churn.

* CLTV: Customer Lifetime Value. A predicted CLTV is calculated using corporate formulas and existing data. The higher the value, the more valuable the customer. High value customers should be monitored for churn.

* Churn Reason: A customer’s specific reason for leaving the company. Directly related to Churn Category.

## Exploratory Data Analysis
### Distribution of Churn Value in Payment Method

![download (2)](https://user-images.githubusercontent.com/88265749/132790138-9fea12d8-2497-4e02-91e9-f1e0ee8d2884.png)

### Distribution of Churn Value in Senior Citizen

![download (3)](https://user-images.githubusercontent.com/88265749/132790230-d657eafb-05e4-4a18-96a1-96d46f931d6b.png)

### Numerical Variable

![download (1)](https://user-images.githubusercontent.com/88265749/132790313-32ef7f6d-856a-4c2b-a83a-659e9e3fe2d8.png)

### Correlation Heatmap

![download (4)](https://user-images.githubusercontent.com/88265749/132790274-db95e897-9c4d-4d35-9ed0-d344f6cc37a0.png)

## Modelling
*The Data splitted into train and test and the train data size used is 20%.

*Models that are used for this analysis are Support Vector Machine, Gaussian Naive Bayes, Decision Tree and Random Forest.

*Comparing Accuracy, Recall, Precision, and F1 Score for choosing the best model.

*Evaluation using Receiver Operating Characteristic - Area Under Curve(ROC AUC).

## Evaluation
Evaluation metrics using Receiver Operating Characteristic - Area Under Curve

![download (5)](https://user-images.githubusercontent.com/88265749/132790537-b186b1d1-489c-457d-bcdd-f69822702287.png)

Based on the evaluation we can conclude that the ROC score are similar to the model overall score!

## Conclusion

*Some column was dropped because they can cause the model to overfit.

*Random Undersampling was chosen to handle the imbalance data.

*Random Forest Classifier was chosen as it is the best model compared to the other model in this case.

*Model were validated using ROC AUC.
