# GPA Prediction from Student Lifestyle and Well-being Data

## Project Description

The aim of this project is to develop a machine learning model to predict students' GPA based on lifestyle, behavioral, and well-being related variables. The project explores how factors such as study time, sleep duration, stress, and other daily habits may influence academic performance.

In addition to the primary student dataset, an external dataset is included to enrich the analysis and provide broader context for student well-being. This helps reduce the limitations of relying on a single dataset.

## Research Question

Can student GPA be predicted using lifestyle and behavioral factors such as sleep duration, study habits, stress level, and well-being indicators?

## Motivation

Academic performance is influenced by many interconnected factors beyond classroom performance alone. By studying student lifestyle patterns together with broader well-being indicators, this project aims to better understand which variables are most informative for GPA prediction.

## Datasets

### Primary Dataset
Student Lifestyle Dataset (Kaggle):
https://www.kaggle.com/code/prernapriya52/student-lifestyle-dataset
The main dataset contains student-level variables related to lifestyle and academic behavior, such as:

- study hours
- sleep duration
- stress level
- daily habits
- GPA or academic performance indicator

### External Dataset
- :contentReference[oaicite:0]{index=0} Life Satisfaction Data  
- Source: https://stats.oecd.org/sdmx-json/data/BLI/LS.ALL.A/all?contentType=csv 
An external dataset is used to enrich the project with additional well-being context. This external data supports a broader interpretation of behavioral patterns and helps strengthen the overall analysis.

## Data Enrichment

The project does not rely only on feature engineering within a single dataset. Instead, it incorporates an additional external dataset to enrich the analysis. This enrichment is intended to improve the explanatory value of the project and align the dataset design with real-world behavioral analysis.

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

## Hypotheses

Some initial hypotheses of the project are:

- Students who sleep longer tend to have higher GPA
- Students who study more tend to have higher GPA
- Higher stress levels are associated with lower GPA
- Well-being related indicators may improve GPA prediction performance

## Machine Learning Models

Since behavioral data may contain non-linear relationships, the project will compare multiple models instead of relying on a single simple baseline.

Planned models include:
- Linear Regression as a baseline
- Random Forest Regressor
- XGBoost Regressor
