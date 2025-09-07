# Model Development and Tuning

This project is a practicum in model development and tuning for health data science, demonstrating end-to-end data preparation, analysis, and machine learning workflows. It investigates the relationship between lifestyle, social determinants of health, and diabetic outcomes for patients in the USA. Using a dataset of health indicators, the analysis explores which features are most predictive of diabetes and applies several machine learning models for prediction. 

## Usage

1. Install the required Python packages:
    ```
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
2. Run the Jupyter notebook `Practicum_3_Model_Development_and_Tuning.ipynb` for a step-by-step analysis and model training.

## Overview

1. **Data Preparation**
    - Converted variables to appropriate types for machine learning.
    - Identified categorical and continuous variables.
    - Handled missing values and outliers.
    - Checked for and removed invalid values.

2. **Exploratory Data Analysis (EDA)**
    - Analyzed distribution of diabetic outcomes.
    - Explored relationships between key features (e.g., HighBP, HighChol, Income, Smoker, Sex) and diabetes status.
    - Visualized correlations and trends using bar charts and heatmaps.

3. **Statistical Testing**
    - Used Chi-squared tests for categorical variables and ANOVA for continuous variables to identify statistically significant features associated with diabetes.
    - Selected features for modeling based on statistical significance and feature importance from a random forest model.

4. **Data Partitioning and Preprocessing**
    - Split data into training and test sets (stratified by target).
    - Encoded categorical variables and normalized numeric features using sklearn transformers.

5. **Model Development and Tuning**
    - Built and evaluated at least three ML models (e.g., SVM, Random Forest, KNN) using the selected features.
    - Used GridSearchCV to tune hyperparameters for each algorithm.
    - Assessed performance through accuracy and classification reports.

## Key Findings

- The features most strongly associated with diabetes outcomes were BMI, general health, high blood pressure, physical health, and high cholesterol.
- Categorical variables like HighBP, HighChol, Stroke, HeartDiseaseorAttack, and PhysActivity showed significant associations with diabetes.
- Continuous variables BMI, PhysHlth, and GenHlth were also significant predictors.
- The best-performing models leveraged these key features, and hyperparameter tuning further improved predictive accuracy
