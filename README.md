# ADS504_G1_Project

<!-- This README provides an overview of the project and explains how to get up and running. It is intentionally concise; more detailed documentation (for example, extended methodology discussions or walk‑throughs) belongs in a wiki or a separate documentation folder. -->
Diabetes Risk Prediction Project
Overview
This repository contains an end‑to‑end data science project that predicts diabetes risk using health survey data. The project explores raw data, engineers informative features, builds several predictive models and evaluates their performance. It is designed as a learning exercise for the ADS 504 course and demonstrates common practices in exploratory data analysis (EDA), feature engineering and model evaluation.
The notebooks and scripts in this repository walk through the process of turning raw data into a useful model:
•	Exploratory Data Analysis (EDA) – understanding the distributions of variables, checking data quality and exploring relationships between predictors and the target variable. See ADS504_EDA.ipynb and ADS504_finalproj_EDA2.ipynb for the initial EDA steps.
•	Feature Engineering – creating new features from existing variables (for example, BMI categories or interaction terms) to improve model performance. These transformations are performed in Feature_Engineering.ipynb and saved to diabetes_features_engineered.csv for downstream use.
•	Modelling and Evaluation – building classification models (such as logistic regression, random forests or gradient boosting), tuning hyperparameters, and comparing results using metrics like accuracy, precision and recall. The modelling work is contained in modeling_v4.ipynb, while evaluation.ipynb and ads504_evaluation.ipynb provide detailed evaluation and comparisons.
Data Source
The raw data come from the Centers for Disease Control and Prevention’s Behavioral Risk Factor Surveillance System (BRFSS), a large‑scale health survey in the United States. We focus on variables that relate to diabetes risk, such as age, BMI, physical activity and medical history. After initial cleaning, the engineered data set (diabetes_features_engineered.csv) contains the predictor variables used for modelling.
Project Structure
The repository is organized as follows:
Path	Purpose
CDC source files/	Raw BRFSS data files from the CDC (not included in this repo due to size).
project support/ADS504_EDA.ipynb	Initial exploratory analysis of the raw data.
project support/ADS504_finalproj_EDA2.ipynb	A second EDA notebook refining the initial analysis.
project support/Feature_Engineering.ipynb	Notebook performing feature engineering and saving the cleaned dataset.
project support/modeling_v4.ipynb	Notebook building and tuning predictive models.
project support/evaluation.ipynb, project support/ads504_evaluation.ipynb	Notebooks evaluating model performance on test data.
project support/diabetes_features_engineered.csv	CSV file containing the engineered features for modelling.
README.md	This file.
Getting Started
To reproduce the analysis and results:
1.	Clone this repository.
 	git clone <repository-url>
cd <repository>
2.	Install dependencies. The project was developed with Python 3.9. Create a virtual environment (optional) and install the required packages. You can use the provided requirements.txt if available, or install packages manually as noted in the notebooks (e.g., pandas, numpy, matplotlib, seaborn, scikit‑learn). For example:
 	python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
3.	Obtain the raw data. Place the CDC BRFSS source files in the CDC source files/ directory. Due to licensing and file size, these files are not included in the repository.
4.	Run the notebooks in order.
5.	ADS504_EDA.ipynb and ADS504_finalproj_EDA2.ipynb perform exploratory analysis and initial cleaning.
6.	Feature_Engineering.ipynb creates engineered features and writes diabetes_features_engineered.csv.
7.	modeling_v4.ipynb builds and tunes the predictive models.
8.	evaluation.ipynb and ads504_evaluation.ipynb assess model performance on hold‑out data.
9.	View results. The notebooks contain plots, tables and discussion of results. You can export the final model or use it to predict diabetes risk on new data.
How This README Relates to the Wiki
This README follows GitHub’s recommendation to keep only the essential information required for others to understand and use the project. The GitHub documentation explains that a README should contain only the information needed for developers to get started and contribute, and that longer documentation is best suited for a wiki[1]. A README should quickly tell what your project can do, whereas a wiki can host long‑form content such as design notes, methodology discussions or detailed user guides[2]. In practice:
•	README (this file) – summarizes the purpose of the project, the data used, the structure of the repository and quick start instructions. Keep it concise and focused on helping someone unfamiliar with your work to get up and running quickly.
•	Wiki – use the wiki (or a /docs folder) for extended documentation. For example, you might include:
•	An in‑depth description of the BRFSS survey and the rationale for selecting specific variables.
•	Detailed descriptions of feature engineering techniques or modelling choices.
•	Experimental results comparing different algorithms or parameter settings.
•	Troubleshooting tips, frequently asked questions and user guides.
By separating short, actionable information in the README from long‑form documentation in a wiki, you avoid duplication and make it easier for contributors to find the information they need. Keeping technical documentation with the source code also ensures that it is versioned alongside the code and is more likely to be kept up to date[3].
Contributing
Contributions are welcome! If you have suggestions for improving this project, please fork the repository and open a pull request. When contributing new models or analyses, add brief explanations and update the README or wiki as appropriate.
License
Include your chosen license here (for example, MIT or Apache‑2.0). See choosealicense.com for guidance.
________________________________________
[1] About READMEs - GitHub Docs
https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes
[2] About wikis - GitHub Docs
https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis
[3] documentation - Documenting a project in a README.md and in a Wiki page? - Software Engineering Stack Exchange
https://softwareengineering.stackexchange.com/questions/415105/documenting-a-project-in-a-readme-md-and-in-a-wiki-page
