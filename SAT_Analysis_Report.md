# Prediction Assignment Writeup

## Introduction
This report presents an analysis of SAT scores using a dataset containing information about the number of test takers and their corresponding average scores in Math, Reading, and Writing. The objective of this study is to understand patterns in SAT performance and build a predictive model for SAT Math scores.

## Data Preprocessing
### Steps:
- Removed missing or incomplete data entries.
- Selected relevant numerical features for analysis.
- Standardized variable names for consistency.

## Exploratory Data Analysis
### Key Statistics:
- **Average SAT Scores:**
  - **Math:** 413.37 (Min: 312, Max: 735)
  - **Reading:** 400.85 (Min: 279, Max: 679)
  - **Writing:** 393.99 (Min: 286, Max: 682)
- **Number of Test Takers:** Ranges from **6 to 1277**.
- **Observation:** No strong correlation between the number of test takers and SAT scores.

## Model Training
To predict SAT Math scores, a **linear regression model** was trained using the number of test takers as the independent variable.

### Model Details:
- **Algorithm Used:** Linear Regression
- **Training Data Split:** 80% Training, 20% Testing
- **Performance Metrics:**
  - **RMSE (Root Mean Squared Error):** 61.28
  - **R² Score:** 0.234

## Conclusion
The linear regression model showed limited predictive power, explaining only **23.4%** of the variability in SAT Math scores. The high RMSE suggests that additional features (such as socioeconomic factors, school funding, or curriculum rigor) may improve the predictive accuracy. Future work can explore more advanced models such as **Random Forest** or **Gradient Boosting** for better predictions.
