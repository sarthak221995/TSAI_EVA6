# Custom MNIST | Multi Input and Multi Output Model

## Objective:

Write a neural network that can take 2 inputs:
- Image from MNIST dataset
- Random number between 0 and 9

and gives two outputs:
- the "number" that was represented by the MNIST image, and
- the "sum" of this number with the random number that was generated and sent as the input to the network


## Digit Recognizer Accuracy

- Train Accuracy : 98.84%
- Test Accuracy : 99.07%

## Sum Calculator Model Accuracy

- Train Accuracy : 94.47%
- Test Accuracy : 97.26%

## Custom Data Loader

Loaded the downloaded data from the colab environment using torch.load method
In the "getitem" method,
- Loaded the data
- Created randomm integer
- Made a tuple with the expected target variables and input variables

## Network Architecture:

![image.png](attachment:image.png)

## Loss Function

Log Loss is the most important classification metric based on probabilities. It’s hard to interpret raw log-loss values, but log-loss is still a good metric for comparing models. For any given problem, a lower log loss value means better predictions.

Mathematical interpretation:

Log Loss is the negative average of the log of corrected predicted probabilities for each instance.

## Train and Test Functions
Model will be trained by following below steps:

Move the below variables to GPU
- x1 - Image
- x2 - Random Number
- y1 - image output
- y2 - Sum of digit in the image and random number
Calculate loss using the Negative loglikelihood function for both digit recognizing and sum calculation
Calculate total loss by adding both the values. To improve model accuracy, loss2(Sum calculation network loss) is multiplied by 2 in order to increase its weightage in loss so that the overall loss is magnified for every one unit of loss in Sum calculation network

![image.png](attachment:image.png)
