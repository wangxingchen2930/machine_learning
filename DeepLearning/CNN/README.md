# Convolutional Neural Networks (CNN)

Technically, deep learning CNN models to train and test, each input image will pass it through a series of convolution layers with filters (Kernals), Pooling, fully connected layers (FC) and apply Softmax function to classify an object with probabilistic values between 0 and 1.

Convolution of an image with different filters can perform operations such as edge detection, blur and sharpen by applying filters.

## Strides

Stride is the number of pixels shifts over the input matrix.

- Fractionally strided convolutions: sometimes referred to as deconvolutions, transpose images, typically from a minimized format to a larger one.

## Padding

Sometimes filter does not fit perfectly fit the input image:
- Pad the picture with zeros (zero-padding) so that it fits
- Drop the part of the image where the filter did not fit. This is called valid padding which keeps only valid part of the image

## Pooling Layer

Pooling layers section would reduce the number of parameters when the images are too large. Spatial pooling also called subsampling or downsampling which reduces the dimensionality of each map but retains important information:
- Max Pooling: Max pooling takes the largest element from the rectified feature map
- Average Pooling: Taking the largest element could also take the average pooling
- Sum Pooling: Sum of all elements in the feature map call as sum pooling

## Dropout Layer

A single model can be used to simulate having a large number of different network architectures by randomly dropping out nodes during training. This is called dropout and offers a very computationally cheap and remarkably effective regularization method to reduce overfitting and improve generalization error in deep neural networks of all kinds.


