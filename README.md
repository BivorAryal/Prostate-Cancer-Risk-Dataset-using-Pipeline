# Prostate Cancer Risk Analysis using ML Pipeline

![Prostate Cancer Awareness](https://img.shields.io/badge/Health-Informatics-blue) 
![Python](https://img.shields.io/badge/Python-3.8%2B-blue) 
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-1.0+-orange)

A machine learning pipeline to analyze prostate cancer risk factors from lifestyle and health data.

## 📌 Table of Contents
- [Dataset](#-dataset)
- [Exploratory Analysis](#-exploratory-analysis)
- [Data Preprocessing](#-data-preprocessing)
- [Model Building](#-model-building)
- [Results](#-results)
- [How to Use](#-how-to-use)

## 📂 Dataset
- **1,000 synthetic health profiles** with prostate cancer risk indicators
- **Features include**:
  - Demographic: Age, BMI
  - Lifestyle: Smoking, alcohol consumption, diet, physical activity
  - Medical: Family history, mental stress, sleep hours, health checkups
  - Target: `risk_level` (Low/Medium/High)

## 🔍 Exploratory Analysis
  - Check basic Statistics
  - Identify missig values
  - Visulize Distribution

## ⚙️ Data Preprocessing
  - Split data: 80% training, 20% Testing
  - Create Process Pipeline
    - Number: Fill missing values with mean -standardize
    - Categorical: Fill missing values with 'most frequent' -OHE
## 🤖 Build Model
  - Using Logistic Regression
  - Tuining with GridsearchCV to find best parameters:
    - tested 32 combination
      - 2 numerical
      - 3 categorical
      - 2 fill values
      - 4 Regulariztion strengths
      - Each combination using 10 fold cross validation

## 📊 Results
  - Best Model Achieve:
    - 85.5% Cross Validation Accuracy
    - 87% Test Accuracy
## Optimal Settings:
  - Mean Impuatation for numbers
  - Most Frequent for missing values
  - Medium regulariztion strength (c=10)

