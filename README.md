#   Neural Network Charity-Analysis

## Overview of Project
Alphabet Soup is a philantrophic organization, dedicated to helping organizations which help protect the environment, help people and make the world a better place.
Beks is a senior analyst responsible for analyzing each donation and identifying the recipients. It has been noted that a few organizations which take loan and disappear. Andy Glad, the President of Alphabet Soup,has asked Beks to predict which organizations are worth donating to. 
The objective of this project is to assist Beks using machine learning and neural networks, to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Purpose

The required input dataset with more than 34,000 organizations that have received funding from Alphabet Soup over the years, is available in a Comma Separated Values (CSV) file

The purpose of this project is to provide the below deliverables:

Deliverable 1: Preprocessing Data for a Neural Network Model


Deliverable 2: Compile, Train, and Evaluate the Model


Deliverable 3: Optimize the Model


Deliverable 4: A Written Report on the Neural Network Model

## Results

### Data Preprocessing

#### What variable(s) are considered the target(s) for your model?

The column IS_SUCCESSFUL can be considered as a target for the model.
This field actually contains the information/binary data denoting whether the donation has been been used successfully or not.

![Screen Shot 2021-10-01 at 1.43.20 PM](https://i.imgur.com/TCjHHCq.png)

#### What variable(s) are considered to be the features for your model?

The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for the model.
Encoding of the categorical variables, splitting into training and testing datasets and standardization have been applied to the features.

#### What variable(s) are neither targets nor features, and should be removed from the input data?

The columns EIN and NAME can be removed from the input data
![Screen Shot 2021-10-01 at 2.27.22 PM](https://i.imgur.com/lW16BY3.png)

### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively.
The output layer is made of a unique neuron as it is a binary classification.
The input data has 43 columns and 34299 records. Considering the size of the input data set and the number of columns in it, taking two hidden layers seems to be the most feasible.
The activation function that is being used is ReLU. This function has been used basically, to speed up the training process in the hidden layers.
Our output is a binary classification, hence sigmoid is used on the outer layer.

![Screen Shot 2021-10-01 at 2.34.28 PM](https://i.imgur.com/q7bT0EI.png)


For the compilation, the optimizer is adam and the loss function is binary_crossentropy.

![Screen Shot 2021-10-01 at 2.38.52 PM](https://i.imgur.com/k2h1y3O.png)

#### Were you able to achieve the target model performance?

Unfortunately, the target model performance was not achieved
![Screen Shot 2021-10-01 at 2.40.37 PM](https://i.imgur.com/ecQ0x4d.png)

#### What steps did you take to try and increase model performance?

Tried using the activation function as tanh

![Screen Shot 2021-10-01 at 2.56.19 PM](https://i.imgur.com/YKaDsPQ.png)

Also increased the number of neurons in the hidden clusters. Also tried adding another hidden layer.



#   Neural Network Charity-Summary









