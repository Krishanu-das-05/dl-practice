# Neural Network From Scratch

Building a 2-layer neural network using only NumPy — no frameworks.

## What's covered
- Single neuron intuition (logistic regression = one neuron)
- Why activation functions are non-negotiable (linear layer collapse proof)
- Forward pass: input → hidden (ReLU) → output (sigmoid)
- Binary cross entropy loss
- Backpropagation via chain rule
- Full training loop with gradient descent

## Architecture
- Input: 3 features
- Hidden layer: 4 neurons (ReLU)
- Output: 1 neuron (sigmoid)

## Results
| Metric | Value |
|--------|-------|
| Initial Loss | ~0.69 |
| Final Loss (1000 epochs, lr=0.1) | ~0.13 |

## Key Takeaways
1. Without activations, stacking layers = single linear layer (mathematically proven)
2. ReLU derivative is 1 where active, 0 where not — explains dying ReLU problem
3. Backprop = chain rule backwards through layers — same math as logistic regression
4. Loss decreasing over epochs confirms network is learning
