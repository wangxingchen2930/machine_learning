# Optimizer

## Stochastic gradient descent (SGD)

SGD is an iterative method for optimizing an objective function with suitable smoothness properties (e.g. differentiable or subdifferentiable). It can be regarded as a stochastic approximation of gradient descent optimization, since it replaces the actual gradient (calculated from the entire data set) by an estimate thereof (calculated from a randomly selected subset of the data). Especially in high-dimensional optimization problems this reduces the computational burden, achieving faster iterations in trade for a lower convergence rate.

### Momentum (step-size optimization): 

The basic idea of momentum is to compare the current value of the gradient with its previous value.
- If they are both pointing in the same direction, that means you are continuing to go downhill and so you might as well accelerate and increase the step size.
- If they are in different direction, you had better watch out.

## Adaptive Gradients (AdaGrad)

The first well-known step-size estimation algorithm that adapted the learning rate to the different parameters at each training step.

**Sparse gradients**: It is highly unlikely that any one image, or even a given batch of images, would be equally senesitive to all the learnable parameters in a network. For example, you will zee zero partial derivatives in a large portion of the space spanned by the parameter vector in SGD.

## RMSprop

Improvement to AdaGrad: replace the monotonically increasing summation in the denominator with its average over the training iterations.

## **Adaptive Moment Estimation (Adam)**

Adam is an algorithm for optimization technique for gradient descent. The method is really efficient when working with large problem involving a lot of data or parameters. It requires less memory and is efficient. Intuitively, it is a combination of the ‘gradient descent with momentum’ algorithm and the ‘RMSP’ algorithm.

- Failed to solve easy problems
- Yet, extremely successful in cracking difficult DL models (e.g., BERT)