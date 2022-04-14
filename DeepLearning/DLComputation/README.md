# Deep Learning Computation

## GPUs

To view the graphics card information of NVIDIA GPU (CUDA installed)
``` 
!nvidia-smi 
```

CPU or GPU can be indicated by
``` 
torch.device('cpu')
torch.device('cuda')
torch.device('cuda:0') 
```

Query the number of available GPUs
```
torch.cuda.device_count()
```

Try to use GPUs:
```
def try_gpu(i=0):  #@save
    """Return gpu(i) if exists, otherwise return cpu()."""
    if torch.cuda.device_count() >= i + 1:
        return torch.device(f'cuda:{i}')
    return torch.device('cpu')

def try_all_gpus():  #@save
    """Return all available GPUs, or [cpu(),] if no GPU exists."""
    devices = [torch.device(f'cuda:{i}')
             for i in range(torch.cuda.device_count())]
    return devices if devices else [torch.device('cpu')]

X = torch.rand(2, 3, device=try_gpu(0))

net = nn.Sequential(nn.Linear(3, 1))
net = net.to(device=try_gpu(0))
```

Query the device where the tensor is located
```
x = torch.tensor([1, 2, 3])
x.device
```

Transfer X to the second GPU
```
Z = X.cuda(1)
```