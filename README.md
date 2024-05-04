**Overview:** This project replicates the distribution of OxyCotin from 84,111 US pharmacies from 2006-2012 . Using difference-in-difference estimation, the authors' 
examined how distribution varies between independent and chain pharmacies. The original paper explores several regressors to explain the distribution of 
OxyCotin like competition and concentration measures, time-fixed effects and multiple levels of entity-fixed effects, and ownership change prior to 
determining that ownership change would be the best fit for the DiD model. Using scikit-learn's GradientBoostingRegressor, we include additional 
variables to allow the model to identify feature performance. 

We read in the raw data from the ARCOS database which initially has 378,572,920 observations. Due to the size of the data set, cleaning,
filtering, and variable creation for the model were handled in SAS. In python, we used the cleaned data to replicate the results from Table 3, 
column 6 of the original paper to create the DiD model. scikit-learn's GradientBoostingRegressor model is used to create more accurate predictions with
feature analysis.


**Datasets & Code:**

- Replication.ipynb - reads in the data from diddata.sas7bdat

- Machine_Learning.ipynb - uses the GradientBoostingRegressor library from scikit-learn to generate a model for evaluating feature performance

- Final_Poster.pdf - poster presentation of the project

- Combating the Opioid Crisis: Insights from Machine Learning - final report of the project 

- data_01.csv.zip, data_02.csv.zip, data_03.csv.zip - cleaned, replicated data set split into 3 files due to size limitations

**Google Colab Links:**

Replication: https://colab.research.google.com/drive/1LerkZkSF5mzo6oaIx47ZGoN7cYeO8mkd?usp=sharing

Machine Learning: https://colab.research.google.com/drive/1EhvYjA2g0CYWcxg4iHvGE2sq6Il7TP3W?usp=sharing

**Overleaf Poster Link:**

https://www.overleaf.com/read/ygdfxkxpcnst#484afa
