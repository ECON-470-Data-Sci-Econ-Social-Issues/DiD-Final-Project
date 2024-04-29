**Overview:** This project replicates the distribution of OxyCotin from pharmacies. Using difference-in-difference estimation, the authors examined how 
distribution varies between independent and chain pharmacies. The original paper explores several regressors to explain the distribution of 
OxyCotin like competition and concentration measures, time-fixed effects and multiple levels of entity-fixed effects, and ownership change 
before determining ownership change would be the best fit for the DiD model. Using scikit-learn's GradientBoostingRegressor, we include other 
regressors to allow the model to identify feature performance. 

We read in the raw data from the ARCOS database which initially has 378,572,920 observations. Due to the size of the data set, cleaning,
filtering, and variable creation for the model were handled in SAS. In python, we used the cleaned data to replicate the results from Table 3, 
column 6 to create the DiD model. scikit-learns GradientBoostingRegressor model is used to print summary statistics of the feature importance
and plot them against relative importance.


**Datasets & Code:**

- Replication.ipynb - reads in the data from diddata.sas7bdat

- Machine_Learning.ipynb - uses the GradientBoostingRegressor library from scikit-learn to generate a model for evaluating feature performance

- finalreport.pdf - report of the project 

- Final_Poster.pdf - poster presentation of the project

**Google Colab Links:**

Replication: https://colab.research.google.com/drive/1LerkZkSF5mzo6oaIx47ZGoN7cYeO8mkd?usp=sharing

Machine Learning: https://colab.research.google.com/drive/1EhvYjA2g0CYWcxg4iHvGE2sq6Il7TP3W?usp=sharing
