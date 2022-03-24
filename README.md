# Arya_Assessment
The following repository is my efforts at performing binary classification of the given dataset

## Objective
To perform binary classification. After data processing, EDA, and feature selection to training a model classifying the data into class '0' or class '1'.

## Importing the Data
The data is provide by the folks at Arya.ai

## Data preprocessing
The data consisted of 57 features without any discriptive names and almost consisted of float data types with a couple of integer types. There was not much cleansing needed. After removing the index column, we moved on to EDA

## EDA
Since the data wasn't discriptive, I proceeded with plotting the correlation of the features. It let to the fact that barring 4, there wasn't much of a significant influence features had on the dependent variable. However there were too many features with not much of a relation with the target variable and hence I decided to approach with 40 most influential features to build prediction model. For that I employed that use of tree based classifier.

## Feature Selection and Splitting Data
As above mentioned the 40 selected features were drained out of the dataframe to create the training data and was then splitting into 4:1 test-train ratio as per team recommendation.

## Model building
To perform binary classification with 40 features, the approach necessitates Logistic Regression, Support Vector Machine or Artificial Neural Network. However, I preferred not to use SVM classifier due to its time consuming nature and being heavy on the GPU. I instead went with LR and ANN for building the model simply for there relative speed.
After experimenting with Various combinations of Neural networks,-with and without drop layers- the F1 score of the ANN and LR were relatively same.

## Prediction
ANN_prediction and LR_prediction are the two results saved below as the results of the binary classification assessment.
