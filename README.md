# Modeling HPV Vaccination Rates Across the U.S.

Course: BMIN 5030 Final Project

Author: Johanna Momole

## Overview

This project explores factors influencing HPV vaccination rates across the U.S., focusing on disparities in socioeconomic and demographic groups. Using the NHANES dataset (2021–2023), the study identifies the effects of health insurance, poverty levels, and education on HPV vaccination coverage. Predictive models, including logistic regression and XGBoost, are employed to uncover barriers and provide actionable recommendations for public health interventions.

------------------------------------------------------------------------

## Project Goals

1.  **Understand disparities** in HPV vaccination rates based on socioeconomic and demographic factors.
2.  **Predict vaccination outcomes** using logistic regression and XGBoost models.
3.  **Provide actionable recommendations** to address barriers and improve vaccination coverage.

------------------------------------------------------------------------

## Dataset

-   **Source**: NHANES (2021–2023)
-   **Key Variables**:
    -   **HPV Vaccine (IMQ060)**: Whether participants have received the HPV vaccine.
    -   **Health Insurance (HIQ011)**: Indicates health insurance coverage status.
    -   **Poverty (IND310)**: Family monthly poverty level categories.
    -   **Education (DMDEDUC2)**: Highest level of education achieved.

------------------------------------------------------------------------

## Methods

### 1. Data Cleaning

-   Merged datasets on HPV vaccine, insurance, poverty, and education levels.
-   Recoded variables into consistent categories for analysis.
-   Removed missing values and standardized categorical variables.

### 2. Descriptive Analysis

-   **HPV Vaccination Rates**: Analyzed vaccination rates based on socioeconomic factors.
-   Visualized distributions for variables like insurance coverage, poverty, and education.

### 3. Predictive Modeling

-   **Logistic Regression** and **XGBoost** models were built to predict vaccination outcomes.
-   **SMOTE (Synthetic Minority Oversampling)** was applied to address class imbalance in the dataset.

### 4. Feature Importance Analysis

-   Identified the most influential factors affecting HPV vaccination rates using model coefficients and feature importance metrics.

------------------------------------------------------------------------

## Results

### Key Findings

-   **Insurance Coverage**: Strongly associated with higher HPV vaccination rates.
-   **Poverty Levels**: Individuals from low-income families were less likely to be vaccinated.
-   **Education**: Higher education levels were linked to better vaccination outcomes.

### Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 76.6%    | 76.6%     | 100%   | 86.8%    |
| XGBoost             | 76.3%    | 76.7%     | 99.1%  | 86.5%    |

### Feature Importance:

-   **XGBoost**: Education was the most important predictor, followed by poverty and insurance.
-   **Logistic Regression**: Education had the highest coefficient, highlighting its strong association with vaccination rates.

## Recommendations

1.  **Expand Insurance Access**: Offer free or low-cost vaccination programs for uninsured individuals.
2.  **Address Poverty Barriers**:
    -   Provide transportation vouchers or mobile vaccination units.
    -   Implement school-based vaccination programs in low-income areas.
3.  **Promote Education**:
    -   Launch community outreach programs to educate parents on HPV vaccination benefits.
    -   Counter misinformation using social media campaigns and local influencers.
4.  **Policy Interventions**:
    -   Advocate for mandatory HPV vaccinations as part of school-entry requirements.
    -   Allocate state and federal funding for vaccination campaigns targeting underinsured populations.

------------------------------------------------------------------------

## Repository Structure

-   **`.gitignore`**: Specifies files and folders to be excluded from version control.

-   **`README.md`**: Provides an overview of the project, including methods and instructions for reproducing the analysis.

-   **`final_project_Johanna Momole.qmd`**: Main Quarto document for the project, containing the analysis and visualizations.

-   **`final_project_Johanna Momole.html`**: Rendered HTML version of the final project report.
