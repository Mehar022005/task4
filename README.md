# task4
task 4 logistic regression
Breast Cancer Detection using Logistic Regression
Project Overview
This project is about using Logistic Regression to detect whether a tumor is benign or malignant based on the features in the breast cancer dataset. I used the CSV file provided (data.csv) which includes different characteristics of cell nuclei (like radius, texture, smoothness, etc.).

The main idea is to build a model that can predict cancer diagnosis from these features using logistic regression — a basic but powerful classification algorithm.

Dataset Details
File Used: data.csv
Target Column: diagnosis
B = Benign (0)
M = Malignant (1)
Total Features: 30 (excluding ID and unnamed column)
Size: 569 rows
Steps I Followed
Loaded the CSV file and removed unnecessary columns (id and Unnamed: 32)
Converted diagnosis labels from M/B to 1/0
Split the dataset into training and testing sets
Scaled the feature values using standardization
Trained a logistic regression model on the training data
Evaluated the model using:
Confusion matrix
Precision score
Recall score
ROC AUC score
Plotted the ROC curve to visualize model performance
Model Results
The model performed really well. Here's a quick summary:

Precision: ~96%
Recall: ~95%
ROC AUC Score: ~99%
This means the model is good at identifying both malignant and benign cases, with very few false positives or negatives.

What is Logistic Regression?
It's a type of algorithm used for classification problems. Unlike linear regression which predicts numbers, logistic regression predicts probabilities. We use the sigmoid function to squeeze output values between 0 and 1, and then apply a threshold (usually 0.5) to decide the class.

Extra Notes
ROC curve shows the balance between sensitivity and specificity at different thresholds.
Scaling was important to ensure all features contributed equally.
This model is a good starting point, but other models (like decision trees or random forests) might perform even better with more tuning.
Tools Used
Python
pandas
scikit-learn
matplotlib
Credits
This task was done as part of the Elevate Labs AI & ML Internship. The goal was to practice basic machine learning workflows and understand evaluation metrics better.
