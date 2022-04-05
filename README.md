# Code for the 2022 IMI Big Data and Artificial Intelligence Case Competition
In this Git, we conducted several analyses to predict the probability of corporate default from financial data of Canadian medium-sized entities. Any sensitive information (e.g., customer ID info) has been removed or modified as necessary.
The three primary methods to tackle this problem are logisitc regression, support vector machine (SVM), and XGBoost to assess the following specific problems:
1. Binary classification to predict good (investment grade) vs bad (non-investment grade) credit rating
2. Conduct multi-class classification to predict the credit rating of a medium-sized entity ranging from 1 (the best credit and least likely to default on a loan) to 17 (the worst credit and most likely to default on a loan)

# Major highlights of results
1. Cleaned the data by removing missing values and outliers
2. Engineered new features and identified key features using recurssive feature elimination (RFE) resulting in a data reduction of 90%
3. Achieved good performance for both binary and multiclass classification through hyperparameter tuning
4. Discovered data structure using clustering analysis

# The major sections of this repository are as follows:
- data_overview_and_cleaning: Removing missing values and outliers from the data to make it easier to analyze

- feature_engineering_and_initial_modeling: Based on previous research on corporate default probability, we engineered novel features and used all features to model some initial results using logistic regression, SVM, and XGBoost.

- feature_selection: Using RFE we identified the most informative features while reducing error resulting in 14 key features, reduced from 144 initial features.

- hyperparameter_tuning_final_modelling: Using our features identified using RFE, we then predict corporate default probability using logistic regression.
