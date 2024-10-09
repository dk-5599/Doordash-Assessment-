![Red Logo](Doordash_Logo.jpg)
# Fraud Detection Analysis
#### (Please refer to the code_file.ipynb for comprehensive insights, including machine learning applications, exploratory data analysis (EDA), assumptions, detailed explanations, recommendations, and various visualizations.)
[Python Code](Code_File.ipynb)


## Overview

This project focuses on analyzing fraudulent transactions using a comprehensive dataset. The objective is to identify patterns and correlations that characterize fraudulent behavior, quantify the financial impact of fraud, and build a predictive model for real-time fraud detection. 

## Objectives

1. **Fraud Analysis**: Examine the characteristics of fraudulent versus non-fraudulent transactions, including SIFT scores and Gross Order Value (GOV).
2. **Financial Impact Assessment**: Calculate the total financial loss caused by fraudulent chargebacks.
3. **Correlation Analysis**: Investigate correlations between various transaction features and fraudulent behavior.
4. **Predictive Modeling**: Develop a machine learning model to predict fraudulent transactions based on key features.

## Assumptions

- Selected features are assumed to be relevant and informative for predicting fraud.
- Missing values are filled with zero, assuming no chargeback occurred in those cases.
- Correlation results are interpreted as indicative of potential relationships, not definitive causation.

## Methodology

1. **Data Preparation**:
   - Cleaned the dataset by handling missing values and selecting relevant features for analysis.
   - Key features included SIFT scores, failed charge attempts, and GOV.

2. **Exploratory Data Analysis (EDA)**:
   - Calculated the percentage of fraudulent transactions and averaged SIFT scores for both fraudulent and non-fraudulent transactions.
   - Visualized the distribution of SIFT scores and GOV using histograms.

3. **Financial Impact Calculation**:
   - Analyzed chargeback costs and calculated the total financial loss due to fraud, amounting to **$8,267.58**.

4. **Correlation Analysis**:
   - Computed the correlation matrix to understand relationships between variables, revealing moderate and strong correlations with fraudulent behavior.

5. **Machine Learning Modeling**:
   - Split the dataset into training and testing sets, standardized the feature data, and implemented a Random Forest Classifier.
   - Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score, and plotted the ROC curve for visual assessment.
  
## Visualizations

- Distribution of SIFT Scores and GOV for both fraudulent and non-fraudulent transactions.
- Chargeback cost distribution for fraudulent transactions.
- Correlation heatmap highlighting relationships among key variables.
- ROC curve illustrating the trade-off between true positive rate and false positive rate for the predictive model.

## Results

- **Percentage of Fraudulent Transactions**: **2.04%**
- **Average SIFT Score**:
  - Fraudulent: **31.88**
  - Non-Fraudulent: **11.87**
- **Average GOV**:
  - Fraudulent: **$37.22**
  - Non-Fraudulent: **$33.36**
- **Confusion Matrix**: Visual representation of the model's prediction performance.


## Conclusion

This analysis emphasizes the significance of understanding transaction behaviors to mitigate fraud effectively. The predictive model provides a foundation for real-time fraud detection strategies, ultimately aiming to reduce financial losses for the company.
