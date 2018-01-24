# optimization-generalization
Assignment 3 from UofT neural networks course on Coursera.

## Scope
Training a simple Neural Network for recognizing handwritten digits.

## Background
The dataset for this assignment is the USPS collection of handwritten digits. It consists of scans (images) of digits that people wrote. The input is a 16 by 16 image of greyscale pixels, showing an image of a handwritten digit. The output is simply which of the 10 different digits it is, so we're using a 10-way softmax as the output layer of our Neural Network. The input layer is simply 256 units, i.e. one for each pixel. We use one hidden layer of logistic units. One of the issues we'll be investigating is what number of hidden units works best for generalization. To keep things as simple as possible, we're not including biases in our model. In the diagram you can see that this model is significantly simpler than the model that we used in programming assignment 2.

![image](https://user-images.githubusercontent.com/6776991/33243747-ea9b262e-d2b9-11e7-99d9-1ca6748ce066.png)


# Part 1: Setting up
Run
```
./setup.sh
```

# Part 2: Process (IE what did I actually do)

Most of this code was provided already complete. The initial commit of `a3.m` is the exact copy of the code provided in the course. The script in a3.m loads the data (training, validation, and test), performs the optimization, and reports the results, including some numbers and a plot of the training data and validation data loss as training progresses.

For the optimization it needs to be able to compute the gradient of the loss function, and that part is what I implemented.
