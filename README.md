# Neural_Network_Charity_Analysis

## Overview of Analysis

I received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup. I need to use the features in the dataset to create a binary classifier that is capable of predicting whether apllicants will be successful or not if they are funded by Alphabet Soup, using my knowledge of machine learning and neural networks. I will preprocess the data for a neural network model, train/evaluate the model, and try to optimize the model.

### Purpose

The purpose of this analysis is to design a binary classifier that is capable of predicting whether or not applicants will be successful with funding from Alphabet Soup.

## Results

### Data Preprocessing

* The variable I am targeting is the `IS_SUCCESSFUL` column because it contains binary information that says whether or not funding was successful or not.

* The columns I am using as features for the model are `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.

*  I removed the identification columns (`EIN` and `NAME`) because they are neither targets or features.

### Compiling, Training, and Evaluating the Model



## Summary