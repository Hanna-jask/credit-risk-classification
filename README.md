# Overview of the Analysis
Through this analysis I used logical regression models to identify creditworthiness of borrowers from a peer-to-peer lending service. 
This dataset included fields loan size, interest rate borrower income, debt to income, number of accounts, derogatory marks and total debt. I used this to predict if a loan was either healthy or high risk. 
To analysis this data, I started by separating labels and features into x and y variables. Then I used sklearn to split the data into training and testing datasets using train_test_split module. Using this I created model 1 (results below). Due to the imbalance in the data, I resampled the data. This used to create model 2. Then I was able to compare the two models and analysis which would provide the better results.

## Results
### Machine Learning Model 1:
 
 *	Accuracy: 99%
 *	Healthy Loans
    *	Precision: 1
    *	Recall: 1
 *	High-Risk loans
    *	Precision: 0.87
    *	Recall: 0.89

### Machine Learning Model 2:

 *   Accuracy: 100%
 *	Healthy Loans
    *	Precision: 1
    *	Recall: 1
*	High-Risk loans
    *	Precision: 0.87
    *	Recall: 1

## Summary
Overall, both models perform well when predicting healthy loans. The second model, using resample data, increased the recall of the high-risk loans. However, this precision has not changed. I would recommend the use of second model as it has high rate of return for both types of loans. As miscalculating high risk loan is more of a risk it would be better to go with better accuracy for high risk over healthy loan. 
