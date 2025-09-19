---
type: definition
aliases:
  - the chain rule
  - The chain rule
---
# Single variable functions
If we have a function $f(x) = g(h(x))$ then
$$
f'(x) = g'(h(x)) h'(x).
$$
# Multivariable functions
If we have a function $f(x_{1}, x_{2}, \dots)$ where each $x_{j}$ depends on some parameter $\lambda$, then the *total derivative* of $f$ with respect to $\lambda$ is 
$$
\frac{df}{d\lambda} = \sum_{j} \frac{\partial f}{\partial x_{j}} \frac{\partial x_{j}}{\partial \lambda}.
$$