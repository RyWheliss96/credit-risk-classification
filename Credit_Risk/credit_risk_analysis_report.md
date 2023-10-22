# Module 12 Report Template

## Overview of the Analysis

    The purpose of the analysis was to determine if we could predict whether the requested loan is healthy or high risk using logistic regression, supervised machine learning and this dataset.<br />

    This dataset used the features: Loan Size, Interest Rate, Borrower Income, Debt to Income, Number of Accounts, Derogatory Marks and Total Debt. Those metrics were used to determine whether the loan was Healthy or High Risk.<br />

    This dataset contained 77,536 different previous outcomes. We then trained the logistic regression model using 58,152 outcomes to train our data in the logistic regression model and having a test group of 19,384.<br />

    The machine learning process began with training a Logistic Regression Model on 58,152 different data points to determine whether a requested loan was High Risk or Healthy. We then tested that on 19,384 datapoints to see how accurate or model was. <br />
    
    At that point, we used a Random Over Sampler provided by Imbalance learn to resample the data. This gave us 112,554 datapoints to train our logistic regression model. This then greatly improved the predictability of our model.<br />


## Results

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.9442676901753825
  * Precision:
    * 0 (Healthy Loan): 1.00
    * 1 (High Risk Loan): 0.87
    * Macro Average: 0.94
    * Weighted Average: 0.99
  * Recall:
    * 0 (Healthy Loan): 1.00
    * 1 (High Risk Loan): 0.89
    * Macro Average: 0.94
    * Weighted Average: 0.99

* Machine Learning Model 2:
* Balanced Accuracy Score: 0.9959744975744975
  * Precision:
    * 0 (Healthy Loan): 1.00
    * 1 (High Risk Loan): 0.87
    * Macro Average: 0.94
    * Weighted Average: 1.00
  * Recall:
    * 0 (Healthy Loan): 1.00
    * 1 (High Risk Loan): 1.00
    * Macro Average: 1.00
    * Weighted Average: 1.00

## Summary

    In Summary, both of the models actually performed very well. Over 94% accuracy rate is very impressive generally. The issues arise when you dive deeper into the numbers of each Machine Learning Model. <br />
    
    Looking at the two models, the logistic regression model after the resampling performs better, which is to be expected. Having twice the amount of training data allows the model to better refine the outcomes and make a better determination in the end of what type of loan will be the outcome. A 99.6% success rate is a lot more encouragin even than a 94.4% accuracy rate. That 5% difference could mean the difference in a lot of money. <br /> 
    
    The performance is somewhat dependent on the problem we are trying to solve. Predicting if a loan is High Risk is a lot more important that predicting if it is a healthy loan. You would rather err on predicting loans as high risk and have them actually be healthy rather than having loans be predicted as healthy and end up being high risk.<br /> 
    
    I would of course recommend continuing to improve the model by increasing either data points or further sampling before putting into use. When it comes to money I tend to be on the conservative side and so would want it as guaranteed as possible. I think by investigating other models or increasing data quantity you could get the model to be at 99.99% success rate. Depending on margins this outcome could be okay but based off the change I saw in one resampling I would highly recommend continuing to resample or reshape the model until it is more accurate. there is still a lot of improvement visible.<br />

