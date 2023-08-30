# deep-learning-challenge

# Neural Network Model Performance Report

## Overview of the Analysis

In this report, we will evaluate the performance of a neural network model created for Alphabet Soup, a charitable organization that seeks to predict which organizations will be successful after receiving funding. The goal of this analysis was to utilize a deep learning model to predict the success of these organizations based on various input features.

### Neural Network Model Overview

The neural network model employed for this analysis is designed for binary classification, aiming to predict the success (or lack thereof) of organizations. The target variable is the 'IS_SUCCESSFUL' column, and the features used in the model include the following columns: `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.

To preprocess the data, we removed the 'EIN' and 'Name' columns, which are neither targets nor informative features for the model.

## Results

### Data Preprocessing

**Target Variable**: 
- Target = 'IS_SUCCESSFUL' column.

**Features**:
- `APPLICATION_TYPE`
- `AFFILIATION`
- `CLASSIFICATION`
- `USE_CASE`
- `ORGANIZATION`
- `STATUS`
- `INCOME_AMT`
- `SPECIAL_CONSIDERATIONS`
- `ASK_AMT`

**Excluded Variables**:
- 'EIN' and 'Name' columns were removed as they do not contribute to the model's predictive power.

### Compiling, Training, and Evaluating the Model

**Model Architecture**:
- Three hidden layers with 'relu' activation.
- Each hidden layer contains 100 neurons.
- One output layer with 'sigmoid' activation.

**Model Performance**:
- The model achieved a maximum accuracy of approximately 72.59%.
- Despite several attempts to optimize the model by adjusting the activation functions, the number of neurons, the number of epochs, and hidden layers, the target model performance of greater than 72.59% was not achieved.

## Summary

The neural network model produced a moderate level of accuracy in predicting the success of organizations based on the provided features. However, it did not meet the target performance level. Here's a summary of the analysis:

- Data preprocessing was crucial to ensure that only relevant features were included in the model and that unnecessary variables were removed.
- Despite experimenting with different model architectures, including changing activation functions, the number of neurons, and the number of hidden layers, we were unable to achieve the desired target model performance.
- The maximum accuracy achieved, approximately 72.7%, suggests that there may be underlying complexities in the data that the current model architecture cannot capture effectively.
