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
```python
data.describe().T  # Basic statistics
data.isnull().sum()  # Missing values
