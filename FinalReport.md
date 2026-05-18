# Introduction

Academic performance is influenced by a combination of academic, behavioral, and lifestyle-related factors. Variables such as study habits, stress levels, sleep duration, and previous academic achievement can all contribute to differences in student success. Understanding these relationships is important for identifying patterns that may help improve educational outcomes and student well-being.

With the increasing availability of educational and behavioral datasets, machine learning methods provide an opportunity to analyze complex relationships between these variables and predict academic performance more effectively. Different models may capture different types of patterns within the data, making it valuable to compare both simple and more advanced machine learning approaches.

# Motivation

The motivation behind this project is to explore how student lifestyle and academic characteristics affect academic performance and to determine whether GPA prediction can be achieved using machine learning techniques. Another motivation is to compare how different datasets and feature structures influence model behavior and predictive performance.

This project also aims to investigate which variables are the most influential predictors of student success and whether complex machine learning models provide advantages over simpler baseline methods.

# Research Question

Can student academic performance be predicted using lifestyle, behavioral, and academic factors?

To answer this question, multiple machine learning regression models were trained and evaluated on two separate student-related datasets. The project compares model performance and analyzes the relationships between various student characteristics and academic outcomes.

# Datasets

## 1. Student Lifestyle Dataset (Kaggle)

Dataset Link:  
https://www.kaggle.com/code/prernapriya52/student-lifestyle-dataset

This dataset contains lifestyle-related variables associated with student academic performance. The dataset includes features such as:

- Study hours
- Sleep duration
- Stress level
- Social activities
- Physical activities
- GPA (target variable)

The primary goal of using this dataset was to analyze how daily lifestyle habits and behavioral patterns influence student GPA.

---

## 2. Student Performance Dataset (UCI Machine Learning Repository)

Dataset Link:  
https://archive.ics.uci.edu/ml/datasets/Student+Performance

This dataset contains demographic, social, and academic information about students. Features include:

- Study time
- Absences
- Family background
- Social behavior
- Internet access
- Previous grades (G1 and G2)
- Final grade (G3 - target variable)

This dataset was used to examine whether academic and demographic variables improve prediction performance compared to lifestyle-related variables alone.

> Note: The datasets were analyzed separately and were not merged because they represent different student populations and contain different feature structures.

# Data Preprocessing

Before analysis and modeling, several preprocessing steps were applied to both datasets.

The preprocessing stage included:

- handling categorical variables,
- separating features and target variables,
- applying one-hot encoding to categorical features,
- preparing the datasets for machine learning models.

Categorical variables were transformed using one-hot encoding with `pd.get_dummies()`. After preprocessing, the datasets were divided into training and testing sets using an 80/20 train-test split.

The target variables used in the models were:

- GPA for the Student Lifestyle Dataset,
- G3 (final grade) for the Student Performance Dataset.

# Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to better understand the datasets and identify patterns related to academic performance.

The analysis focused on:

- distributions of GPA and academic grades,
- relationships between study habits and academic success,
- the impact of stress and sleep duration,
- correlations between numerical variables,
- detection of possible trends and outliers.

Several visualizations, including histograms, scatter plots, box plots, and correlation heatmaps, were used during this stage.

The exploratory analysis suggested that variables such as study time, previous grades, and stress levels may have important relationships with academic performance.

# Hypothesis Testing

Statistical hypothesis testing was performed to validate relationships observed during exploratory analysis.

The following statistical methods were used:

- Pearson Correlation Analysis
- t-tests
- ANOVA

The results showed that:

- Study hours had a significant positive relationship with GPA.
- Stress level significantly affected academic performance.
- Previous academic performance strongly influenced final grades.
- Some variables, such as sleep duration and absences, showed weaker statistical significance in certain analyses.

These findings helped guide feature selection and interpretation during the machine learning stage.

# Machine Learning Models

Three regression-based machine learning models were implemented and compared:

## 1. Linear Regression

Linear Regression was used as the baseline model. This model assumes linear relationships between input variables and academic performance.

## 2. Random Forest Regressor

Random Forest was implemented to capture possible non-linear relationships between student characteristics and GPA prediction. Feature importance analysis was also performed using this model.

## 3. XGBoost Regressor

XGBoost was used as an additional ensemble learning method to compare performance with both Linear Regression and Random Forest.

The models were evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

# Results and Findings

## Model Performance Comparison

### Student Lifestyle Dataset

| Model | MAE | MSE | R² Score |
|---|---|---|---|
| Linear Regression | 0.164 | 0.042 | 0.547 |
| Random Forest | 0.180 | 0.050 | 0.461 |
| XGBoost | 0.195 | 0.061 | 0.349 |

The results showed that Linear Regression achieved the strongest performance on the lifestyle dataset. This suggests that relationships between lifestyle-related variables and GPA were mostly linear.

---

### Student Performance Dataset

| Model | MAE | MSE | R² Score |
|---|---|---|---|
| Linear Regression | 1.647 | 5.657 | 0.724 |
| Random Forest | 1.165 | 3.798 | 0.815 |
| XGBoost | 1.196 | 4.552 | 0.778 |

For the Student Performance dataset, Random Forest achieved the highest R² score among the tested models. This indicates that the dataset contains more complex and non-linear relationships between variables.

## Overall Findings

The results demonstrate that:

- Machine learning models can successfully predict student academic performance to a certain extent.
- Model performance depends heavily on dataset structure and feature characteristics.
- Simpler models may outperform more advanced models when relationships are mostly linear.
- More complex models become advantageous when datasets contain non-linear interactions.

Feature importance analysis also showed that study-related variables and previous academic performance were among the strongest predictors of GPA.

# Limitations

This project has several limitations.

- The datasets represent different student populations and educational environments.
- Some datasets are relatively small, which may limit generalization.
- Lifestyle-related variables may contain self-reporting bias.
- Academic performance cannot be fully explained using the available variables alone.

Additionally, the datasets were static and did not include longitudinal or time-based behavioral changes.

# Future Work

Several improvements could be explored in future studies:

- using larger and more diverse datasets,
- incorporating psychological and socioeconomic indicators,
- applying deep learning approaches,
- testing additional machine learning models,
- developing interactive GPA prediction systems.

Future research could also investigate how student behavior changes over time and how those changes influence academic success.

# Conclusion

This project explored the relationship between student lifestyle factors, academic characteristics, and academic performance using machine learning techniques.

Two separate datasets were analyzed to compare how different types of student-related information affect GPA prediction. Exploratory analysis, hypothesis testing, and machine learning models were applied throughout the project.

The findings showed that academic performance can be predicted to a meaningful extent using behavioral and academic variables. While Linear Regression performed best on the lifestyle dataset, Random Forest achieved stronger performance on the academic dataset, highlighting the importance of selecting models according to dataset characteristics.

Overall, the project demonstrates that machine learning methods can provide valuable insights into factors affecting student success, although academic performance remains a complex phenomenon influenced by many variables.

# AI Usage Disclosure

AI tools such as ChatGPT were used for:

- debugging assistance,
- code organization,
- report structuring,
- writing support.

All analysis, interpretation, and final decisions were reviewed and completed by the author.
