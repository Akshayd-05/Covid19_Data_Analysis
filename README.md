# COVID-19 Mortality Data Analysis

This project performs an in-depth analysis of COVID-19 mortality data across different demographic categories, focusing on age, sex, and other mortality-related factors. The dataset "Provisional COVID-19 Deaths by Sex and Age" sourced from Data.gov provides information on mortality attributed to COVID-19 in the United States.

## Dataset Information
The dataset provides mortality data attributed to COVID-19, pneumonia, and influenza, segmented by age, sex, and state in the U.S. The key variables include:

- **Data As Of**: The date when the dataset was last updated.
- **Start Date**: The starting date for the recorded deaths.
- **End Date**: The ending date for the recorded deaths.
- **Group**: The category of data (e.g., by age, sex, or overall).
- **Year**: Year of recorded deaths.
- **Month**: Month of recorded deaths.
- **State**: U.S. state where deaths occurred (if applicable).
- **Sex**: Gender category (Male, Female, or Total).
- **Age Group**: Age category for recorded deaths (e.g., 0-4 years, 65-74 years).
- **COVID-19 Deaths**: The number of deaths attributed to COVID-19.
- **Total Deaths**: The total number of deaths in that category.
- **Pneumonia Deaths**: The number of deaths attributed to pneumonia.
- **Influenza Deaths**: The number of deaths attributed to influenza.
- **Pneumonia and COVID-19 Deaths**: The number of deaths involving both pneumonia and COVID-19.
- **Influenza and COVID-19 Deaths**: The number of deaths involving both influenza and COVID-19.

## Key Analysis
### 1. **Age-Related Disparities in COVID-19 Mortality Rates**
- Older adults (65+) account for the majority of COVID-19 fatalities, highlighting the increased risk with age.

### 2. **COVID-19 Mortality by Sex**
- Males show a higher mortality rate compared to females, supported by factors like comorbidities and lifestyle behaviors.

### 3. **Analysis of Mortality by Cause**
- COVID-19 has proven to be a more significant cause of death than influenza, with substantial mortality related to respiratory illnesses.

### 4. **COVID-19 Deaths Over Years by Gender**
- Analysis of how gender-based mortality trends evolved through different pandemic waves.

### 5. **Statistical Analysis**
- Chi-Square tests revealed a statistically significant association between gender and COVID-19 mortality.
- Geospatial analysis identified regional disparities in mortality across U.S. states.

## Data Transformation
- **Age Group Encoding**: Age group categories were numerically encoded for better statistical modeling.
- **Gender-Based Mortality Analysis**: Calculated COVID-19 and pneumonia/influenza death rates based on gender.

## Predictive Analytics
### 1. **Feature Selection**:
- Variables considered include Year, Month, Age Numeric, Total Deaths, Pneumonia Deaths, Influenza Deaths, and Pneumonia and COVID-19 Deaths.
- **LASSO Regression**: Applied for feature selection, identifying the most influential predictors for COVID-19 mortality.

### 2. **Model Training**:
- **Random Forest Regressor**: Used to train the predictive model.
- **Hyperparameter Tuning**: Conducted using Grid Search with cross-validation to optimize model performance.

## Key Findings
- Males have a higher mortality rate compared to females.
- COVID-19-related deaths peaked in 2021, followed by a decrease in subsequent years.
- The highest mortality rates are observed among older adults, especially those aged 85+.
