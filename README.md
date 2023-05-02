# icl-ml-portfolio

# CREDIT CARD FRAUD DETECTION

Project aim is to analyse data containing both fraudulent and non-fraudulent credit card transaction data and use this to build a machine learning model that can accurately predict a fraudulent transaction in the future. This is important to minimise the amount of customers and vendors who are negatively impacted by the large scale of global credit card fraud.
The project will use a number of techniques to attempt to make the performance of the model as strong as possible.

## DATA
The dataset contains transactions made by credit cards in September 2013 by European cardholders. 

Data was obtained from Kaggle:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download

The dataset has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of ULB (Université Libre de Bruxelles) on big data mining and fraud detection.

This dataset presents transactions that occurred in two days, where there are just 492 frauds out of 284,807 transactions. The dataset is therefore highly unbalanced as the positive class (frauds) account for 0.172% of all transactions.\
It contains only numerical input variables which are the result of a Principle Component Analysis transformation (dimensionality reduction technique).\
Due to confidentiality issues, the original features and more background information about the data cannot be provided.
Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

- Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.
- Feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.
- Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## MODEL 
A summary of the model you’re using and why you chose it. 

## HYPERPARAMETER OPTIMSATION
Description of which hyperparameters you have and how you chose to optimise them. 

## RESULTS
A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

