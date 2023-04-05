# Logistic Regression Model 

This repository contains a logistic regression model trained to classify penguins into two categories: Adelie and Chinstrap. The model uses a dataset of physical measurements for each penguin to predict its species.

### Dataset

The dataset used to train the model is the Palmer Penguins dataset, which contains information on three penguin species: Adelie, Chinstrap, and Gentoo. For this model, we only used the measurements for Adelie and Chinstrap penguins.

The dataset was preprocessed using the autoNorm() function, which applies min-max normalization to the dataset. This function returns the normalized dataset as well as the ranges and minimum values of each column.

### Model Training

The logistic regression model was trained using the logreg2() function, which implements gradient ascent to optimize the model weights. The function takes in the normalized training data, learning rate, and number of iterations as parameters, and returns the optimized weights for the model.

### Model Testing

To test the trained model, the x_test_norm data was passed through the model to obtain predictions for each penguin's species. The predictions were then thresholded using a threshold of 0.5, resulting in binary predictions of either 0 or 1 for each penguin.

### Evaluation

The accuracy of the trained model was evaluated using a confusion matrix. The confusion matrix was created by comparing the true labels of the test data to the predicted labels of the model. The resulting confusion matrix shows the number of true positives, true negatives, false positives, and false negatives for each class.

### Usage

To use this code, simply clone the repository and run the logistic_regression.py file. The output will show the loss for each iteration of training, as well as the resulting confusion matrix and weight values for the trained model.