# Activation Function

## ReLU

The rectifier or ReLU (Rectified Linear Unit) activation function is an activation function defined as the positive part of its argument: 
> f(x) = max (0,x)

ReLU activation functions mitigate the vanishing gradient problem. This can accelerate convergence.

<img src="./relu.svg" class="centerImage">


## Softmax

The softmax function, also known as softargmax or normalized exponential function, is a generalization of the logistic function to multiple dimensions. It is used in multinomial logistic regression and is often used as the last activation function of a neural network to normalize the output of a network to a probability distribution over predicted output classes, based on Luce's choice axiom. The standard (unit) softmax function <img src="https://render.githubusercontent.com/render/math?math={\displaystyle \sigma :\mathbb {R} ^{K}\to [0,1]^{K}}">is defined when *K* is greater than one by the formula
><img src="https://render.githubusercontent.com/render/math?math=\displaystyle \sigma (\mathbf {z} )_{i}={\frac {e^{z_{i}}}{\sum _{j=1}^{K}e^{z_{j}}}}\ \ \ \ {\text{ for }}i=1,\dotsc ,K{\text{ and }}\mathbf {z} =(z_{1},\dotsc ,z_{K})\in \mathbb {R} ^{K}"/>

## Sigmoid

A sigmoid function is a mathematical function having a characteristic "S"-shaped curve or sigmoid curve. A common example of a sigmoid function is the logistic function:

><img src="https://latex.codecogs.com/gif.latex?S(x)={\frac{1}{1+e^{-x}}}={\frac{e^{x}}{e^{x}+1}}=1-S(-x)"/>

<img src="./sigmoid.svg" class="centerImage">

## Softmax vs Sigmoid

Softmax is used for multi-classification in the Logistic Regression model, whereas Sigmoid is used for binary classification in the Logistic Regression model.

## Tanh

Like the sigmoid function, the tanh (hyperbolic tangent) function also squashes its inputs, transforming them into elements on the interval between -1 and 1:

><img src="https://latex.codecogs.com/gif.latex?tanh(x)={\frac{1 - e^{-2x}}{1 + e^{-2x}}}"/>

<img src="./tanh.svg" class="centerImage">
    
## Gradient of Point-Wise Activation Function

Gradient Matrix is
- Diagonal
- Sparse
- Fast to compute and apply