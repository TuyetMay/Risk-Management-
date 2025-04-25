# Risk Management Encoding Comparison

This project compares different feature encoding techniques (Label Encoding, One-Hot Encoding, and Weight of Evidence - WoE) to determine which performs best for predictive risk management models. We evaluate the impact of these encodings on the performance of Logistic Regression, Random Forest, and LightGBM models.

## Project Goals

* To systematically compare the effectiveness of Label Encoding, One-Hot Encoding, and WoE for categorical features in a risk management context.
* To assess the performance of Logistic Regression, Random Forest, and LightGBM models using each of these encoding methods.
* To identify the optimal encoding strategy for each model type in predicting risk.

## Methodology

The project involves the following steps:

1.  **Data Preprocessing:** Cleaning and preparing the risk management dataset. This includes handling missing values, outliers, and ensuring data quality.
2.  **Feature Selection:**
    * **Correlation Analysis:** Using a correlation matrix to identify and potentially remove highly correlated features to reduce multicollinearity.
    * **Information Value (IV):** Calculating the Information Value for each categorical feature to assess its predictive power with respect to the target variable. Features with low IV may be considered for removal.
3.  **Feature Encoding:** Applying Label Encoding, One-Hot Encoding, and Weight of Evidence (WoE) to the remaining categorical features after feature selection.
4.  **Model Training:** Training Logistic Regression, Random Forest, and LightGBM models using datasets encoded with each method.
5.  **Performance Evaluation:** Evaluating model performance using appropriate metrics (e.g., AUC, F1-score, precision, recall).
6.  **Comparison and Analysis:** Comparing the performance of different encoding methods for each model, considering the impact of feature selection, and drawing conclusions.
