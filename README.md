# assignments-ml_workflow_assignment.md

# ML Workflow Assignment
 🧩 Problem Overview
We are given a dataset of customer orders and need to predict whether a customer will make a repeat purchase within 30 days.

✅ Task 1

🎯 Label (Target Variable)
*repeat_purchase_flag*

*Justification:*  
This column represents the outcome we want to predict — whether a customer makes a repeat purchase within 30 days (1 = yes, 0 = no).

⚠️ Data Leakage Column
*discount_used_on_repeat_order*

*Justification:*  
This column contains information about the repeat purchase itself, which occurs after the target event. Including it as a feature would introduce future information into the model, causing data leakage.

✅ Task 2

 1. 📊 Establish a Baseline Model

*Why it matters:*  
A baseline model (such as Logistic Regression or predicting the majority class) provides a reference point to evaluate whether more complex models actually improve performance.

2 Train-Test Split

*Why it matters:*  
Splitting the dataset into training and testing sets ensures that the model is evaluated on unseen data. This helps prevent overfitting and gives a realistic estimate of model performance.

## 🚀 Summary

- *Label:* repeat_purchase_flag  
- *Leakage Feature:* discount_used_on_repeat_order  
- *Key Steps Missed:*
  - Baseline model creation  
  - Proper train-test split
