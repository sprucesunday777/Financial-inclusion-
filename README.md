
Predicting who in Africa is most likely to have a bank account: My first Data Science Project competition.

Introduction
Financial inclusion remains one of the main obstacles to economic and human development in Africa. For example, across Kenya, Rwanda, Tanzania, and Uganda only 9.1 million adults (or 14% of adults) have access to or use a commercial bank account.

Traditionally, access to bank accounts has been regarded as an indicator of financial inclusion. Despite the proliferation of mobile money in Africa, and the growth of innovative fintech solutions, banks still play a pivotal role in facilitating access to financial services. Access to bank accounts enables households to save and make payments while also helping businesses build up their credit-worthiness and improve their access to loans, insurance, and related services. Therefore, access to bank accounts is an essential contributor to long-term economic growth.

Aim and Objective
The objective of this competition is to create a machine learning model to predict which individuals are most likely to have or use a bank account. The models and solutions developed can provide an indication of the state of financial inclusion in Kenya, Rwanda, Tanzania and Uganda, while providing insights into some of the key factors driving individuals’ financial security.

Data Access
  This data used for this project was extracted from various Finscope surveys ranging from 2016 to 2018, and more information about these surveys can be found here:
FinAccess Kenya 2018
Finscope Rwanda 2016
Finscope Tanzania 2017
Finscope Uganda 2018  and can be accessed on the Zindi platform

Dataset Description
This dataset contains valuable information on various features related to people with bank accounts, including the 'country', 'year', 'uniqueid', 'bank_account', 'location_type','cellphone_access', 'household_size', 'age_of_respondent', 'gender_of_respondent', 'relationship_with_head', 'marital_status',  'education_level', 'job_type'

Data Preparation
The steps taken in the preparation of this data include:

Exploratory Data Analysis
Various visualisation charts were used to understand the pattern and behaviour of the dataset.
Data Cleaning
Missing values in the 'bank account' columns were amputated by dropna function.
category_encoders was used to change the categorical data to numerical data
Model Building/selection 
Lazypredict classifier as used to get model with the highest accuracy score, which LGBMClassifier happen to the highest with 0.88 accurate 

Model Evaluation
The models were evaluated using classification reports  to assess their predictive performance.

Feature Importance Analysis
Feature importance analysis was conducted on the LGBMClassifier model to identify which features have the most significant impact on bank accounts. This analysis provides valuable insights into the factors that drive people who will have/ open bank account in Kenya, Rwanda, Uganda and Tanzania. The top four features that have significant impact on it were age, job title, household size, education level.

Conclusion
This data science project successfully predicts who in Africa is most likely to have a bank account for the Financial institutions based on essential features like the  'year', 'location_type', 'household_size', 'age_of_respondent', 'gender_of_respondent', 'relationship_with_head', 'marital_status',  'education_level', 'job_type' and the top-performing model is the LGBMClassifier

