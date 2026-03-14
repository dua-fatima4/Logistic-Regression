Perceptron vs Logistic Regression – Decision Boundary Visualization

This project demonstrates how different classification approaches create decision boundaries for a binary classification dataset.

The experiment compares three methods:

Perceptron using Step Function

Logistic Regression from Scikit-learn

Perceptron using Sigmoid Function

All models are trained on the same dataset and their decision boundaries are visualized together.

Dataset

A synthetic dataset is generated using make_classification() from Scikit-learn.

Dataset configuration:

100 samples

2 input features

Binary classes

High class separation for clear visualization

The dataset is visualized using Matplotlib where each point represents a sample and colors represent the class labels.

Models Implemented
1. Perceptron using Step Function

A perceptron is implemented from scratch using a step activation function.

Prediction rule:

if z > 0 → class 1  
else → class 0

Weights are updated using the perceptron learning rule:

w = w + lr * (y − y_hat) * x

This approach produces a hard classification boundary.

2. Logistic Regression

A logistic regression model from Scikit-learn is trained on the same dataset.

Logistic regression uses the sigmoid function internally to estimate probabilities and learns the optimal decision boundary using optimization.

The learned coefficients and intercept are used to plot the decision boundary.

3. Perceptron using Sigmoid Function

In this experiment, the perceptron is modified to use a sigmoid activation function instead of a step function.

Sigmoid function:

σ(z) = 1 / (1 + e^(-z))

Unlike the step function, the sigmoid outputs probabilities between 0 and 1, which makes the learning smoother.

Visualization

The final graph displays the dataset and the decision boundaries of all three approaches:

Red line → Perceptron with Step Function

Black line → Logistic Regression

Yellow line → Perceptron with Sigmoid Function

This helps visually compare how each method separates the data.

Libraries Used

NumPy

Matplotlib

Scikit-learn

Learning Outcome

This project helps understand:

How the Perceptron algorithm works

Difference between step and sigmoid activation functions

How Logistic Regression finds a decision boundary

Visualization of linear classifiers
