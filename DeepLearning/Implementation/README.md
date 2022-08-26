# Implementation (Pytorch)

## Torchvision and Random Tensors

Random tensor is useful when you are testing your code.

The data we feed into a neural network is likely to be formatted as $(B, C, H, W)$.
- $B$ is the batch size
- $C$ is the number of channels
- $H$ is height
- $W$ is width

### Normalization

What we need for feeding into a neural network is floating-point input data whose range spans $[-1.0,+1.0]$. Thus, it is required to normalize the data. 

If you need to do this manually, pay attention to convert integer to float before feeding into division.

Keeping in mind that data normalization is applied to each channel separatly.

### Data Augmentation

For a image data, you can use the functionality of <code>torchvision.transforms</code> to augment your training data.

### Ranfom Tensors

You have to cast the output of <code>torch.randint()</code> to type <code>torch.uint8</code> since the <code>torch.randint()</code> returns type <code>torch.int64</code> which will do wrong thing, leading to difficult-to-spot bugs in your code. 

<code>images = torch.randint(0, 256, (4, 3, 5, 9)).type(torch.uint8)</code>

But this bug can be ignored if you use "standard" dataloaders.

Pay attention to whether tensors are created on CPU or GPU.

You can fix the seed of the pseudorandom generator to make your code reproducible.




