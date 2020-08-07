**Lesson 3:Model Training**

# Chapter 23- Evaluating Model Performance

**Test dataset** is a portion of labeled data that is split off and reserved for model evaluation.

We need to decide what metrics we will use to evaluate performance, and whether there are any particular thresholds that the model needs to meet on these metrics in order for us to decide that it is "good enough."

When splitting the available data, it is important to preserve the statistical properties of that data. This means that the data in the training, validation, and test datasets need to have similar statistical properties as the original data to prevent bias in the trained model.

# Chapter 24 - Confusion matrices

A confusion matrix gets its name from the fact that it is easy to see whether the model is getting confused and misclassifying the data.

It is mostly represented in a more general form that uses the terms positive and negative:


<table>
 <caption>Confusion matrix</caption>
 <tr>
 <th colspan="2">Actual class</th>
 </tr>
 <tr>
  <td>Positive</td></td>
  <td>Negative</td>
 </tr>
 <tr>
  <th rowspan="2">Predicted class</th>
  <td>Positive</td>
  <td>True Positive (TP)</td>
  <td>False Positive (FP)</td>
 </tr>
 <tr>
  <th>Negative</th>
  <td>False Negative (FN)</td>
  <td>True Negative (TN)</td>
 </tr>

</table>


- **True positives** are the positive cases that are correctly predicted as positive by the model
- **False positives** are the negative cases that are incorrectly predicted as positive by the model
- **True negatives** are the negative cases that are correctly predicted as negative by the model
- **False negatives** are the positive cases that are incorrectly predicted as negative by the model

#Chapter 25 - Evaluation metrics for classification
## Confusion matrix

- Accuracy - (TP+TN)/(TP+FP+FN+TN)
- Precision - TP/(TP+FP)
- Recall-   TP/(TP+FN)
- F1 Scoree - 2∗ ((Precision+Recall)/(Precision∗Recall))
              
 ## Model Evaluation charts             
- Gains and lifts chart
- Receiver Operating Characteristics (ROC) - Area Under the Curve metric(0.5 corresponds to random guessing)

#Chapter 25 - Evaluation Metrics for Regression
- Root Mean Squared  Eror(RMSE) - Square root of the squared differences between the predicted and actual values.
- Mean Absolute Error - Average of the absolute difference between each prediction and the true value.
- Spearman's correlation - Strength and direction of the relationship between predicted and actual values.
- R-squared - How close the regression line is to the true values.
 ​	
 
           
            ​	
         
         ​	








