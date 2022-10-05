# HEALTH-INSURANCE-CROSS-SELL-PREDICTION
HEALTH INSURANCE CROSS SELL PREDICTION![dataset-cover](https://user-images.githubusercontent.com/109526052/194065503-c5761c94-eeb5-410b-9079-ecce22a19fab.jpg)


Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.


Attribute Information:-

1.id : Unique ID for the customer                                              
2.Gender : Gender of the customer                                      
3.Age : Age of the customer                                   
4.Driving_License 0 : Customer does not have DL, 1 : Customer already has DL             
5.Region_Code : Unique code for the region of the customer                  
6.Previously_Insured : 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance                              
7.Vehicle_Age : Age of the Vehicle                                   
8.Vehicle_Damage :1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.                                           
9.Annual_Premium : The amount customer needs to pay as premium in the year            
10.PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.                   
11.Vintage : Number of Days, Customer has been associated with the company           
12.Response : 1 : Customer is interested, 0 : Customer is not interested   
Gender feature and it's effect on response feature:-

![download](https://user-images.githubusercontent.com/109526052/194065815-c4023005-0c62-420b-90cf-ea84318f9513.png)
Vehicle Age feature and it's effect on response feature:-
![download](https://user-images.githubusercontent.com/109526052/194066227-de245795-124d-4c76-92ab-1b539b0a1b58.png)

Concusion :-
The given dataset is an imbalance problem as the Response variable with the value 1 is significantly lower than the value zero
The male customers own slightly more vehicles and they are more tend to buy insurance in comparison to their female counterparts.
Customers of aged between 30 to 60 are more likely to buy insurance.wheras Youngsters under 30 are not intrigued by vehicle insurance. Reasons could be the absence of involvement, less awareness about insurance and they may not have costly vehicles yet.

the customers who have driving licences will option for insurance instead of those who don’t have it

Consumers with 1-2-year-old vehicles are more interested in buying insurance. as compared to Consumers with less than 1-year-old Vehicles

Customers with Vehicle_Damage are likely to buy insurance as they have experienced the expenditure in repairing vehicles The variable such as Age, Previously_insured, Annual_premium is more affecting the target variable.

We used different type of algorithms to train our model like, Logistic Regression, Random Forest model, Decision tree and XGB Classifier. And Also we tuned the parameters of XGB Classifier and Random Forest model Comparing the model on the basis of precision,recall, accuracy ,F1 score we can see that the XGBClassifier model performs better.Even comparing ROC curve XGB Classifier performed better because curves closer to the top-left corner indicate better performance.
