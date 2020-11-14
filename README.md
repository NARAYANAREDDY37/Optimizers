# Optimizers

## 1.Gradient Descent
Gradient descent is an iterative machine learning optimization algorithm to reduce the cost function. We update parameters in the negative gradient direction to minimize the loss.

## Types of Gradient Descent
Different types of Gradient descents are
- Batch Gradient Descent or Vanilla Gradient Descent
- Stochastic Gradient Descent
- Mini batch Gradient Descent

## Momentum
- Momentum is like a ball rolling downhill. The ball will gain momentum as it rolls down the hill. Momentum helps accelerate Gradient Descent(GD) when we have surfaces that curve more steeply in one direction than in another direction.
- For updating the weights it takes the gradient of the current step as well as the gradient of the previous time steps. This helps us move faster towards convergence.
- Convergence happens faster when we apply momentum optimizer to surfaces with curves.

## Adagrad — Adaptive Gradient Algorithm
- Adagrad is an adaptive learning rate method. In Adagrad we adopt the learning rate to the parameters. We perform larger updates for infrequent parameters and smaller updates for frequent parameters.
- It is well suited when we have sparse data as in large scale neural networks. GloVe word embedding uses adagrad where infrequent words required a greater update and frequent words require smaller updates.
- For SGD, Momentum, and NAG we update for all parameters θ at once. We also use the same learning rate η. In Adagrad we use different learning rate for every parameter θ for every time step t
