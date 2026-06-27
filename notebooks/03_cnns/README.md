# Convolutional Neural Networks (CNNs)

Training a CNN on MNIST handwritten digits using PyTorch.

## Architecture
Input (1×28×28) → Conv1(8) → ReLU → MaxPool → Conv2(16) → ReLU → MaxPool → Flatten → Linear(10)

## What's covered
- Why CNNs beat regular NNs on images (weight sharing, spatial info)
- Convolution operation and output size formula
- MaxPooling — reduces spatial dimensions by half
- DataLoader — batching and shuffling
- CrossEntropyLoss for multiclass classification
- torch.max for picking predicted class
- model.eval() + torch.no_grad() for evaluation

## Results
| Metric | Value |
|--------|-------|
| Dataset | MNIST (60k train, 10k test) |
| Epochs | 3 |
| Final Loss | ~0.07 |
| Test Accuracy | ~98% |

## Key Takeaways
1. Weight sharing — same filter applied everywhere, fewer parameters
2. Output size = (input - filter + 2*padding) / stride + 1
3. MaxPool halves spatial dimensions
4. CrossEntropyLoss for multiclass, BCELoss for binary
5. Always use model.eval() + torch.no_grad() during evaluation
