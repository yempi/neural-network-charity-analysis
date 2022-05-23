# neural-network-charity-analysis

## Overview
In this project neural networks will be used to help predicting where to invest as a foundation. With the help of Machine Learning and Neural Networks we will create a binary classifier that is capable of predicting whether applicants will be successful if funded by the foundation (Alphabet Soup).

The data will be taken from a .csv file containing more than 34k organizations that have received funding in the past.

The process of completing this project is as follows:
- Preprocessing Data for a Neural Network Model
- Compile, Train, and Evaluate the Model
- Optimizing the Model

## Results
- Data Preprocessing
  - Variables considered as targets:
Column **IS_SUCCESSFUL** contains binary data pertaining whether or not the charity donation was used effectively.
  - Variables considered as features:
Columns **APPLICATION_TYPE**, **AFFILIATION**, **CLASSIFICATION**, **USE_CASE**, **ORGANIZATION**, **STATUS**, **INCOME_AMT**, **SPECIAL_CONSIDERATIONS**, **ASK_AMT**.
  - Variables that should be removed:
Columns **EIN** and **NAME** are considered identification information.
  
  
  
- Compiling, Training, and Evaluating the Model

  - Number of Neurons, Layers and Activation Functions selected for the model:
  
    Hidden Layers:
    - #1: 80 neurons.
    - #2: 30 neurons.
    
    Input Data:
    - 43 features
    - 25k samples
    
    Output Layer:
    - 1 neuron.
    
    Activation Functions:
    - ReLU: for speeding up the training process (hidden layers).
    - Sigmoid: considering a binary classification (output layer).
    - adam: optimizer for compilation.
    - binary_crossentropy: loss function for compilation.

- Target Model Performance

The goal was to meet or excede the 75% model accuracy, but this was not achieved obtaining numbers as close as 72% maximum.

- Steps taken to increase model performance
 1. Bucketing to the feature **ASK_AMT** and organizing the values by intervals.
 2. Increasing the number of neurons in a single hidden layer, then using a model containing 3 hidden layers.
 3. Trying the **tanh** activation function.
 
## Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
