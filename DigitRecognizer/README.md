# Digit Recognizer
This a project for solving the kaggle challenge of Recognizing the digit. [Kaggle Link](https://www.kaggle.com/competitions/digit-recognizer)

## Accuracy
Acheived a maximum accuracy of 99.58% which is the top 4% result. Researched optimization of hyperparameters and the deep learning layers to include while training.

## Deep learning model developed
* Created 4 convolution layers with elu activation function.
* After every CNN layer placed a batch normalization layer to keep the traning stable for dealing with vanishing/exploding gradients.
* After MaxPooling a dropout layer is kept to avoid overfitting while training.
* Finally created 2 dense layers to train the model to predict the digits.