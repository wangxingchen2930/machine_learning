# Optimization of Deep Learning


Loss functions in deep learning usually are non-convex. Thus, traditional optimization is not enough. We should modernize optimization for deep learning.

Traditional ML theory dictates $d$ must be smaller than $n$ to avoid overfitting. But, in practice $d>>n$ generalized extremely well.

**Convergence**: finding a solution that matches the training data

**Generalization**: good performance on unseen data


## Convexity Functions
**Properties**:
- The sums of convex functions is convex
- The maximum of a set of convex functions is convex
- If $f(y)$ is convex, $f(Ay)$ is also convex
- $f(y)$ is concave if $-f(y)$ is convex
- $f(y) = Ay+b$ is both convex and concave
- The second derivative of a convex function is positive

