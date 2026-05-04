# GPA Prediction from Student Lifestyle and Academic Data

## Project Description
The aim of this project is to develop machine learning models to predict students' academic performance based on lifestyle, behavioral, and academic factors.

The project analyzes how variables such as study habits, stress level, sleep patterns, and academic history influence student performance.

## Research Question
Can student academic performance be predicted using lifestyle, behavioral, and academic factors?

## Motivation
Academic performance is influenced by multiple interconnected factors, including daily habits and prior academic achievements. 

This project aims to identify the most important predictors of student performance and to understand how different types of data (lifestyle vs. academic records) affect model performance.

## Datasets

### 1. Student Lifestyle Dataset (Kaggle)
https://www.kaggle.com/code/prernapriya52/student-lifestyle-dataset

This dataset includes student-level lifestyle variables such as:
- Study hours
- Sleep duration
- Stress level
- Social and physical activities
- GPA (target variable)

### 2. Student Performance Dataset (UCI)
https://archive.ics.uci.edu/ml/datasets/Student+Performance

This dataset includes academic and demographic variables such as:
- Study time
- Absences
- Family background
- Social behavior
- Previous grades (G1, G2)
- Final grade (G3 - target variable)

> Note: The datasets are analyzed separately and are not merged, as they represent different student populations.

## Methodology

The project will proceed in the following steps:

1. Data collection and preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Hypothesis testing to examine relationships between variables  
4. Feature selection and feature engineering  
5. Machine learning model development for GPA prediction  
6. Model evaluation and interpretation  

## Exploratory Analysis

Initial exploratory analysis will be conducted to understand:

- the distribution of GPA and input variables
- relationships between sleep, stress, study habits, and GPA
- correlations among numerical variables
- possible patterns that can guide feature selection

## Hypothesis Testing

Statistical tests were conducted to validate relationships observed during EDA, including:

- Correlation analysis (Pearson)  
- t-tests  
- ANOVA  

Key findings:
- Study hours have a strong positive effect on GPA  
- Stress level significantly affects GPA  
- Some variables (e.g., sleep, absences) were not statistically significant

## Machine Learning Models

Three regression models were implemented and compared:

- Linear Regression (baseline)
- Random Forest Regressor
- XGBoost Regressor

## Results

### Lifestyle Dataset (GPA Prediction)
- Linear Regression performed best  
- Indicates mostly linear relationships between variables  

### Student Performance Dataset (G3 Prediction)
- Random Forest performed best  
- Indicates more complex and non-linear relationships  

## Key Insights

- Model performance depends on dataset structure  
- Simpler models can outperform complex ones when relationships are linear  
- More complex models are beneficial when data contains non-linear patterns  

This highlights the importance of selecting models based on data characteristics rather than model complexity.


## Limitations

- Datasets represent different student groups  
- Results may not generalize to all populations  
- Some datasets are relatively small 

