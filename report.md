# Module 12 Report 

## Overview of the Analysis

The analysis involved processing a historical lending dataset from a peer-to-peer lending company to construct a model capable of determining the creditworthiness of borrowers. The dataset encompassed various financial parameters: loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt for each loan application.

A notable observation was the disparity between the counts of healthy loans (0) and high-risk loans (1): 75,036 healthy loans compared to 2,500 high-risk loans.

The machine learning analysis involved several key stages:

Pre-processing: This initial phase cleaned and structured the raw data, ensuring no missing values or errors. It standardized the data for further analysis.

Training: After pre-processing, the model was trained. Logistic Regression, a binary classification model, was chosen. It learned patterns to predict loan outcomes.

Validation and Evaluation: The model was validated and evaluated after training. Using a separate dataset, its generalization to new data was assessed. Metrics like accuracy, precision, recall, F1-score, and AUC-ROC measured its performance.

Resampling: Due to class imbalance between healthy and high-risk loans, resampling was used. More high-risk data points were generated to balance the dataset, preventing bias.

These steps—pre-processing, Logistic Regression training, and resampling—were used to predict loan health. 


## Results

Machine Learning Model 1 Assessment:

Accuracy - a measure of correct predictions: the model achieves 18679 true positives and 558 true negatives.

Precision - the ratio of accurately predicted true positives to total predicted positives: the model's precision is 1 for healthy loans and 0.87 for high-risk loans.

Recall - the ratio of correctly identified actual positives: the model's recall is 1 for healthy loans and 0.89 for high-risk loans.

Support - the count of actual occurrences in the dataset: the support column highlights an imbalance in training data (18759 healthy loans vs. 625 high-risk loans), revealing potential weaknesses in reported scores during evaluation.


Machine Learning Model 2 Evaluation:

Accuracy - a measure of accurate predictions: the model demonstrates 55945 true positives and 55954 true negatives.

Precision - the ratio of accurately predicted true positives to total predicted positives: the model exhibits equal precision for both healthy loans (precision 0.99) and high-risk loans (precision 0.99).

Recall - the ratio of correctly identified actual positives: the model achieves equal recall rates for healthy loans (recall 0.99) and high-risk loans (recall 0.99).

Support - the count of actual occurrences in the dataset: as per the support column, the model maintains balance in training data (56277 healthy loans vs. 56277 high-risk loans), indicating robustness in the reported scores during evaluation.

## Summary

I suggest opting for 'Machine Learning Model 2' due to its well-balanced reported scores, showcasing elevated levels of Accuracy, Precision, and Recall for both healthy loans and high-risk loans. Benefiting from the additional data points resulting from resampling, 'Machine Learning Model 2' exhibited superior performance, rendering it more adept at predicting loan risks and accurately classifying them as either healthy loans or high-risk loans.
