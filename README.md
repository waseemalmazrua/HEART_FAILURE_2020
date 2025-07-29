## Can Machine Learning Predict Mortality in Heart Failure Patients?
## In this applied project, I analyzed real-world data of 299 patients diagnosed with heart failure, aiming to predict mortality risk using their clinical features.


## Project Inspiration:
## This project was inspired by the published study:
##  “Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone”
 
### Article:https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/s12911-020-1023-5#Tab1

## The study found that serum creatinine and ejection fraction were among the strongest predictors of survival.
## What Did I Do?
## 1 - Statistical Analysis using the T-Test, which revealed:
## Deceased patients had significantly lower ejection fraction and higher serum creatinine (P-value < 0.0001)


## 2 - Built Two Predictive Models to evaluate the impact of variables:
## Model 1 – With time feature:
## Accuracy = 65%
## Recall for deaths = Only 32%
## Model 2 – Without time + Using a Pipeline:
## Applied StandardScaler + SMOTE to handle class imbalance
## Trained an XGBoostClassifier with GridSearchCV for hyperparameter tuning
## Accuracy = 71.6%
## Recall for deaths = 53%
## More balanced and clinically meaningful performance
## 3 - Extracted Feature Importance to identify top contributing variables.


## - What Did I Learn?
## Statistically significant variables are essential for effective feature selection
## Including time-related features like time may lead to bias and reduce clinical interpretability
## Using Pipeline + SMOTE improved model performance, especially for minority class (deaths)



### - Tools & Techniques Used:
Python (Pandas, Scikit-learn, imblearn, XGBoost, Seaborn)
Jupyter Notebook
Statistical Testing (T-Test)
ML Pipelines + GridSearchCV
 This project highlights the powerful intersection between data science and healthcare, demonstrating how AI can support clinical decision-making and patient risk stratification.




### Source: - https://archive.ics.uci.edu/dataset/519/heart+failure+clinical+records









<img width="3000" height="1800" alt="feature importance with time" src="https://github.com/user-attachments/assets/ae4a6906-0c2f-420e-b45d-20bf09dc5328" />

<img width="3000" height="1800" alt="feature importance(without time)" src="https://github.com/user-attachments/assets/157318c1-57d7-42f6-acd2-40f7f207b2cd" />




