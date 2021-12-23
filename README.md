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

* For my neural network model I used two hidden layers, one with 24 nodes and one with 12 nodes. I used the `ReLU` activation function for the two hidden layers, and `Sigmoid` for the output layers because the output is a binary classification.

* I was not able to achieve the target model performance of 75%. This model does not accurately predict the outcome of charity donations.

* To improve the performance of the model, I tried three changes. First, I added more nodes to the two hidden layers. Instead of 24 and 12 I used 80 and 40. The model was still under 75%. Next, I tried to add more hidden layers, and I increased from two to  three, with 80, 40 and 20 nodes respectively. This change didn't increase the model's performance to be greater than 75%. The last thing I tried was using a different activation function. I used `ReLU`, `Tanh`, and `Sigmoid`, instead of only `Relu` for the hidden layers. This, once again, did not increase the model's performance to be over 75%.

## Summary

I tweaked my model three times, and was not successful in reaching the target model performance of 75%. A better model I could use to potentially reach a target performance of 75% is Random Forest Classifier, since we are working with a binary classification problem. The Random Forest Classifier is a supervised machine learning model, which might have better results than my deep-learning neural network.