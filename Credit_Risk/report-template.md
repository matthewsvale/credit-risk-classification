# Module 12 Report Template

## Overview of the Analysis

The goal of this analysis was to utilize machine learning techniques to train and evaluate the performance of Logistic Regression Models to identify the creditworthiness of borrowers. We compared the performance of these methods to see which model peformed better. to differentiate between the type of loans, we labeled one model as 0 (healthy loans) and the other as 1 (high-risk loans).

The datasets were split into features and labels, and then divided it further to make training and testing sets. Model 1 uses a logistic regression model and training with the original training sets, fitting it to the training sets, and then using it to make predictions. For Model 2, we resampled the original training data with the RandomOverSampler, and through the logistic regression model and the fitted resampled training sets, we also generated predictions. We then evaulated the peformance of model 1 and model 2 by using the balance accuracy score, the confusion matrix, the precision score, the recall score, and the f1-score in the classification report. 


## Results

* Machine Learning Model 1:
  
    For Model 1, we trained the original data, giving us a 94.4% accuracy for predicting the 2 labels. It was good at predicting the healthy loans as their precision and recall scores were 1.00. One thing to note is that the high-risk loan prediction sat at 0.87, which could be higher. This shows that 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model only identified 89% of all high-risk loans in the dataset. 



* Machine Learning Model 2:

    For Model 2, we trained the resampled data, giving us a 99.6% accuracy for predicting the 2 labels. It predicts the healthy loans well, as the precision and recall scores are 1.00. While the precision score of the high-risk loans remain at 0.87, the recal score went up to 1.00, showing that the model can now predict all high-risk loans in the dataset. 
  
  

## Summary

The analysis shows that Model 2 outperforms Model 1 when predicting high-risk loans and has predicted with a higher accuracy for the labels. Model 2 had a high precision when predicting high-risk loans with the dataset, which showed good performance. I would recommend using Model 2 in this setting as it identifies higher-risk loans and overall has better accuracy for predicting labels. 
