# PyTorch Basics

Building and training neural networks using PyTorch.

## What's covered
- Tensors vs NumPy arrays
- Autograd — automatic differentiation
- nn.Module — building neural networks
- Training loop: zero_grad → forward → loss → backward → step
- Adam optimizer vs SGD

## Architecture
- Input: 3 features
- Hidden layer: 4 neurons (ReLU)
- Output: 1 neuron (sigmoid)

## Results
| Metric | NumPy From Scratch | PyTorch |
|--------|-------------------|---------|
| Final Loss | ~0.13 | ~0.007 |
| Epochs | 1000 | 1000 |
| Optimizer | SGD | Adam |

## Key Takeaways
1. PyTorch = NumPy + autograd + GPU support
2. loss.backward() replaces entire manual backprop
3. optimizer.zero_grad() must be called before each step
4. Adam adapts learning rate per parameter — faster convergence
5. torch.no_grad() for inference — disables gradient tracking
