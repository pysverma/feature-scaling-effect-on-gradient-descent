# Feature Scaling Effect on Gradient Descent

This repository demonstrates why feature scaling is critical when using Gradient Descent.

---

## Problem

When features have very different scales:
- Gradient descent oscillates
- Convergence becomes extremely slow
- Learning rate must be tiny

---

## Mathematical Insight

Cost Function:

J(θ) = (1 / 2m) Σ (hθ(x) - y)^2

Gradient:

∂J/∂θ = (1/m) Xᵀ (Xθ - y)

If feature scales differ greatly,
the cost surface becomes elongated,
causing zig-zag optimization paths.

---

## What This Repo Shows

Without scaling:
- Extremely slow convergence
- Tiny learning rate required

With scaling:
- Faster convergence
- Larger learning rate possible
- Smooth optimization

---

## Key Learning

Feature scaling transforms the cost function from a narrow ellipse to a circular contour.

This dramatically improves optimization efficiency.

---

## Tech Stack

- Python
- NumPy
- Matplotlib
- scikit-learn
