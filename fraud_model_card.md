# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

The model described in this card has been built to analyse a dataset containing both fraudulent and non-fraudulent credit card transactions and then accurately predict fraudulent transactions while minimising false positives.

The dataset is highly imbalanced as the positive class (frauds) account for just 0.172% of all transactions. Therefore techniques have been used to try and counter this imbalance and prevent the model overfitting for the majority class.


**Input:** 

The dataset inputs used to build the model contain only numerical input variables which are the result of a Principle Component Analysis transformation.
Due to confidentiality issues, the original features and more background information about the data cannot be provided. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'.

- Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset.
- Feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.
- Feature 'Class' is the response variable a value 1 in case of fraud and 0 otherwise.

**Output:** Describe the output(s) of your model

The model outputs a dataframe showing the progression of the analysis and model building through the notebook as different analysis, optimisation and overfitting reduction techniques are attempted.

The performance of each version of the model is determined through the following metrics:

- Precision = ratio of the number of true positives divided by the sum of the true positives and false positives. It describes how good a model is at predicting the positive class. Precision is referred to as the positive predictive value.

- Recall = the ratio of the number of true positives divided by the sum of the true positives and the false negatives. Recall is the same as sensitivity.

- F1 score = combines precision and recall into one metric. If precision and recall are both high, F1 will be high, too. If they are both low, F1 will be low. If one is high and the other low, F1 will be low. F1 is a quick way to tell whether the classifier is actually good at identifying members of a class, or if it is finding shortcuts (e.g., just identifying everything as a member of a large class).

- Area Under the Precision-Recall Curve (AUPRC) = recommended metric by the dataset owners due to the class imbalance. A high area under the curve represents both high recall and high precision, where high precision relates to a low false positive rate, and high recall relates to a low false negative rate


**Model Architecture:** Describe the model architecture you’ve used

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
