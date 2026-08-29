# Lab 1 — PyTorch Tutorial: Building an Artificial Neuron

**Course:** Neural Networks (7th Semester)
**Duration:** 3 Hours
**Software/Tools:** Python, Jupyter Notebook / Google Colab, PyTorch, NumPy, Matplotlib

## Overview

This lab introduces PyTorch as a deep learning framework and walks through building an artificial neuron from its mathematical formulation (`z = w·x + b`), applying activation functions, and using `nn.Linear` to construct a neuron with learnable parameters. It complements the theory covered in the accompanying slide deck (*ANN — up to Activation Functions*): the biological neuron analogy, the ANN neuron model, and activation functions including ReLU.

## Learning Objectives

- Understand the role of PyTorch in deep learning
- Create and manipulate tensors
- Perform tensor operations
- Implement an artificial neuron from its mathematical equation
- Apply activation functions using PyTorch
- Understand automatic differentiation (Autograd)
- Create neurons using `nn.Linear`

## Prerequisites

- Python 3.x
- PyTorch (`pip install torch`)
- Matplotlib (`pip install matplotlib`)
- Jupyter Notebook or Google Colab

## Contents

| # | Section | Key API |
|---|---------|---------|
| 1 | Introduction to PyTorch | — |
| 2 | First PyTorch Program | `torch.__version__`, `torch.cuda.is_available()` |
| 3 | Creating Tensors | `torch.tensor()`, `zeros()`, `ones()`, `rand()` |
| 4 | Tensor Properties | `.shape`, `.dtype`, `.ndim`, `.device` |
| 5 | Tensor Operations | `+`, `-`, `*`, `torch.dot()` |
| 6 | Artificial Neuron | `z = w·x + b` via `torch.dot()` |
| 7 | Activation Functions | `torch.sigmoid()`, `torch.tanh()`, `torch.relu()` |
| 8 | Plotting Activation Functions | `matplotlib.pyplot`, `torch.linspace()` |
| 9 | Automatic Differentiation | `requires_grad=True`, `.backward()`, `.grad` |
| 10 | Neuron via `nn.Linear` | `nn.Linear(in_features, out_features)` |

## How to Run

1. Open the notebook in Jupyter or upload it to Google Colab.
2. Run cells sequentially from top to bottom — each section builds on tensors/variables defined earlier.
3. For Section 2, note that `torch.cuda.is_available()` will return `False` on machines without a GPU; this does not affect the rest of the lab (all subsequent code runs on CPU).
4. For Section 8, ensure Matplotlib is installed; the plot will render inline in Jupyter/Colab.

## Student Tasks

- [ ] Create tensors of different shapes
- [ ] Perform arithmetic and dot product operations
- [ ] Implement a neuron with 5 inputs
- [ ] Change the weights and bias; predict the output before execution
- [ ] Plot Sigmoid, Tanh, and ReLU
- [ ] Use Autograd to compute the gradient of `y = x² + 5x + 2`
- [ ] Create `nn.Linear(5, 1)` and inspect its weights
- [ ] Compare the manual neuron implementation with `nn.Linear`

## Repository Structure

```
.
├── README.md
├── Lab1_PyTorch_Artificial_Neuron.ipynb   # main lab notebook
└── ANN_slides.pptx                         # reference slide deck (activation functions, neuron model)
```

## References

- PyTorch official documentation: https://pytorch.org/docs
- Course slide deck: *Deep Learning — Artificial Neural Networks (up to Activation Functions)*
