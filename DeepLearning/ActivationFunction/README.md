# Activation Function

## ReLU

The rectifier or ReLU (Rectified Linear Unit) activation function is an activation function defined as the positive part of its argument: 
> f(x) = max (0,x)

## Softmax

The softmax function, also known as softargmax or normalized exponential function, is a generalization of the logistic function to multiple dimensions. It is used in multinomial logistic regression and is often used as the last activation function of a neural network to normalize the output of a network to a probability distribution over predicted output classes, based on Luce's choice axiom. The standard (unit) softmax function <img src="https://render.githubusercontent.com/render/math?math={\displaystyle \sigma :\mathbb {R} ^{K}\to [0,1]^{K}}">is defined when *K* is greater than one by the formula
> <img src="https://render.githubusercontent.com/render/math?math={\displaystyle \sigma (\mathbf {z} )_{i}={\frac {e^{z_{i}}}{\sum _{j=1}^{K}e^{z_{j}}}}\ \ \ \ {\text{ for }}i=1,\dotsc ,K{\text{ and }}\mathbf {z} =(z_{1},\dotsc ,z_{K})\in \mathbb {R} ^{K}.}">



    