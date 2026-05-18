# GPA Prediction from Student Lifestyle and Academic Data

## Project Overview

This project investigates whether student academic performance can be predicted using lifestyle, behavioral, and academic factors.

Different machine learning models were trained and compared on two separate student-related datasets to analyze how factors such as study habits, stress levels, sleep patterns, and previous academic performance influence GPA prediction.

---

# Research Question

Can student academic performance be predicted using lifestyle, behavioral, and academic factors?

---

# Motivation

Academic performance is influenced by multiple interconnected variables, including daily habits, mental well-being, and prior academic achievement.

The main motivation of this project is to:

- identify the most influential predictors of academic success,
- compare different machine learning approaches,
- analyze how dataset structure affects model performance,
- better understand relationships between lifestyle and educational outcomes.

---

# Datasets

## 1. Student Lifestyle Dataset (Kaggle)

Dataset Link:  
https://www.kaggle.com/code/prernapriya52/student-lifestyle-dataset

This dataset contains lifestyle-related student variables such as:

- Study hours
- Sleep duration
- Stress level
- Social activities
- Physical activities
- GPA (target variable)

---

## 2. Student Performance Dataset (UCI)

Dataset Link:  
https://archive.ics.uci.edu/ml/datasets/Student+Performance

This dataset contains academic and demographic information including:

- Study time
- Absences
- Family background
- Social behavior
- Previous grades (G1, G2)
- Final grade (G3 - target variable)

> Note: The datasets were analyzed separately and were not merged because they represent different student populations and different feature structures.

---

# Project Workflow

The project was completed in the following stages:

1. Data collection and preprocessing  
2. Exploratory Data Analysis (EDA)  
3. Hypothesis testing  
4. Feature engineering and encoding  
5. Machine learning model development  
6. Model evaluation and interpretation  

---

# Exploratory Data Analysis

EDA was conducted to examine:

- distributions of GPA and input variables,
- relationships between sleep, stress, study habits, and GPA,
- correlations among numerical variables,
- patterns useful for feature selection.

Several visualizations and statistical summaries were generated during this stage.

---

# Hypothesis Testing

Statistical hypothesis testing was applied to validate relationships observed during EDA.

The following methods were used:

- Pearson Correlation Analysis
- t-tests
- ANOVA

## Key Findings

- Study hours showed a strong positive relationship with GPA.
- Stress level significantly affected academic performance.
- Some variables, such as sleep duration and absences, showed weaker statistical significance.

---

# Machine Learning Models

Three regression models were implemented and compared:

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

The models were evaluated using:

- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- R² Score

---

# Results

## Lifestyle Dataset (GPA Prediction)

- Linear Regression achieved the strongest performance.
- This suggests that relationships within the lifestyle dataset are mostly linear.

## Student Performance Dataset (G3 Prediction)

- Random Forest achieved the highest R² score.
- This indicates the presence of more complex and non-linear relationships.

---

# Key Insights

- Model performance strongly depends on dataset structure.
- Simpler models can outperform more complex ones when relationships are primarily linear.
- Non-linear models become more effective when datasets contain more complex interactions between variables.

The findings demonstrate the importance of selecting machine learning models based on data characteristics rather than model complexity alone.

---

# Limitations

- The datasets represent different student populations.
- Results may not generalize to all educational settings.
- Some datasets are relatively small.
- Lifestyle-related variables may contain self-reporting bias.

---

# Future Work

Possible future improvements include:

- using larger datasets,
- incorporating psychological and socioeconomic indicators,
- testing deep learning approaches,
- developing interactive GPA prediction systems.

---

# Requirements

The project was developed using Python and the following libraries:

- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost
- seaborn

---

# AI Usage Disclosure

AI tools such as ChatGPT were used for:

- debugging assistance,
- code organization,
- report structuring,
- writing support.

All analysis, interpretation, and final decisions were reviewed and completed by the author.

