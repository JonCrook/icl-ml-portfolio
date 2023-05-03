# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

The model described in this card has been built to analyse a dataset containing both fraudulent and non-fraudulent credit card transactions and then accurately predict fraudulent transactions while minimising false positives.

The dataset is highly unbalanced as the positive class (frauds) account for just 0.172% of all transactions. Therefore techniques have been used to 


**Input:** Describe the inputs of your model 
It contains only numerical input variables which are the result of a Principle Component Analysis transformation (dimensionality reduction technique).
Due to confidentiality issues, the original features and more background information about the data cannot be provided. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.
Feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.
Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

**Output:** Describe the output(s) of your model

**Model Architecture:** Describe the model architecture you’ve used

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
