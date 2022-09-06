# Loss

## MSE Loss

$L_{MSE}(\theta) = \frac{1}{K} \sum^{K-1}_{k=0} ||x_k - f_{\theta}(y_k)||^2$

- If training sample is wrong, the predicition error cna be very large.
- If a few bad training samples can dramatically degrade results.

## MAE Loss

$L_{MSE}(\theta) = \frac{1}{K} \sum^{K-1}_{k=0} |x_k - f_{\theta}(y_k)|$

## Cross Entropy Loss

$L_{MSE}(\theta) = -\frac{1}{K} \sum^{K-1}_{k=0} x_klog(f_{\theta}(y_k))$