# Challenge_21
## Neural Networks and Deep Learning


## Overview of the analysis

In this Challenge, a tool was developed to assist in selecting financial applicants with higher chances of success in their projects. Neural networks were used to leverage dataset functions in creating a binary classifier capable of predicting whether applicants would succeed in receiving funding.

## Results


### Data Processing

The target variables of the model are:
* NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

The model's characteristic variables are:
* NAME
* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE
* ORGANIZATION
* STATUS
* INCOME_AMT
* ASK_AMT
* IS_SUCCESSFUL

The input variables EIN and SPECIAL_CONSIDERATIONS are neither targets nor data characteristics, so they were eliminated.

### Model Compilation, Training, and Evaluation.

For my model, I used 22 neurons distributed across 2 input layers using ReLU as the activation function with 21 neurons, and an output layer with the Sigmoid function with one neuron.
ReLU was used as the activation function and Sigmoid as the output function for effective feature extraction and learning of nonlinear relationships, as it is suitable for binary classification tasks requiring an interpretable output.

An effectiveness of 78.79% was achieved.

To increase performance, the applicant's name was considered. The outliers in the "CLASSIFICATION" and "APPLICATION_TYPE" fields with unique value counts less than 500 were removed. Outliers in the 'NAME' column with counts less than 5 were also eliminated.

In conclusion, this Challenge has resulted in the development of a useful tool for selecting financial applicants with higher chances of success in their projects. Neural networks were employed to build a binary classifier capable of predicting whether applicants would successfully receive funding.

A recommendation to address this classification problem could be to use a decision tree-based classification model, such as Random Forest. Random Forest is a supervised learning method based on constructing multiple decision trees during training and combining their predictions to obtain a final classification.


