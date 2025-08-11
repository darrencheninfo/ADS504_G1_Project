<!-- This README provides an overview of the project and explains how to get up and running. It is intentionally concise; more detailed documentation (for example, extended methodology discussions or walk-throughs) belongs in a wiki or a separate documentation folder. -->

# Diabetes Risk Prediction Project

## Overview
This repository contains an end-to-end data science project that predicts diabetes risk using health survey data. The project explores raw data, engineers informative features, builds several predictive models and evaluates their performance. It is designed as a learning exercise for the **ADS 504** course and demonstrates common practices in exploratory data analysis (EDA), feature engineering and model evaluation.

The notebooks and scripts in this repository walk through the process of turning raw data into a useful model:

- **Exploratory Data Analysis (EDA)** – understanding the distributions of variables, checking data quality and exploring relationships between predictors and the target variable. See `ADS504_EDA.ipynb` and `ADS504_finalproj_EDA2.ipynb` for the initial EDA steps.
- **Feature Engineering** – creating new features from existing variables (for example, BMI categories or interaction terms) to improve model performance. These transformations are performed in `Feature_Engineering.ipynb` and saved to `diabetes_features_engineered.csv` for downstream use.
- **Modelling and Evaluation** – building classification models (such as logistic regression, random forests or gradient boosting), tuning hyperparameters, and comparing results using metrics like accuracy, precision and recall. The modelling work is contained in `modeling_v4.ipynb`, while `evaluation.ipynb` and `ads504_evaluation.ipynb` provide detailed evaluation and comparisons.

---

## Data Source
The raw data come from the **Centers for Disease Control and Prevention’s Behavioral Risk Factor Surveillance System (BRFSS)**, a large-scale health survey in the United States. We focus on variables that relate to diabetes risk, such as age, BMI, physical activity and medical history. After initial cleaning, the engineered data set (`diabetes_features_engineered.csv`) contains the predictor variables used for modelling.

---

## Project Structure

| Path | Purpose |
|------|---------|
| `CDC source files/` | Raw BRFSS data files from the CDC (not included in this repo due to size). |
| `project support/ADS504_EDA.ipynb` | Initial exploratory analysis of the raw data. |
| `project support/ADS504_finalproj_EDA2.ipynb` | A second EDA notebook refining the initial analysis. |
| `project support/Feature_Engineering.ipynb` | Notebook performing feature engineering and saving the cleaned dataset. |
| `project support/modeling_v4.ipynb` | Notebook building and tuning predictive models. |
| `project support/evaluation.ipynb`, `project support/ads504_evaluation.ipynb` | Notebooks evaluating model performance on test data. |
| `project support/diabetes_features_engineered.csv` | CSV file containing the engineered features for modelling. |
| `README.md` | This file. |

---

## Getting Started

To reproduce the analysis and results:

1. **Clone this repository:**
   ```bash
   git clone <repository-url>
   cd <repository>
