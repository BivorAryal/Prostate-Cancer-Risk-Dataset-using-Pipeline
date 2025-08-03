# Prostate-Cancer-Risk-Dataset-using-Pipeline

Table of Contents:
  Intro:
      Load Data
      1,000 individual health profiles focusing on potential risk factors for prostate cancer.
      This dataset includes a variety of features such as age, body mass index (BMI), smoking habits, diet, physical activity, family history of cancer, mental stress levels, and health-check behavior.
EDA:
Check basic Statistics
Identify missig values
Visulize Distribution
Data Preprocessing:
Split data: 80% training, 20% Testing
Create Process Pipeline
Number: Fill missing values with mean -standardize
Categorical: Fill missing values with 'most frequent' -OHE
Build Model
Using Logistic Regression
Tuining with GridsearchCV to find best parameters:
tested 32 combination
2 numerical
3 categorical
2 fill values
4 Regulariztion strengths
Each combination using 10 fold cross validation
Results
Best Model Achieve:
85.5% Cross Validation Accuracy
87% Test Accuracy
Optimal Settings:
Mean Impuatation for numbers
Most Frequent for missing values
Medium regulariztion strength (c=10)
