---
type: maths
aliases:
---
The **Laplacian** $\nabla^2$ is defined as 
$$
\nabla^2 = \sum_{j=1}^n \left( \frac{\partial}{\partial x_{j}} \right)^2
$$
as characterised in $\mathbb{R}^n$. It takes different forms in different coordinate systems, which are scaled differently.

### Cartesian coordinates
$$
\nabla^2 =\left( \frac{\partial}{\partial x} \right)^2+\left( \frac{\partial}{\partial y} \right)^2+\left( \frac{\partial}{\partial z} \right)^2
$$
### Spherical coordinates
To find the Laplacian in [[Coordinate Systems|spherical coordinates]], substitute the translation into the above.
$$
\nabla^2 = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \right) + \frac{1}{r^2 \sin \theta} \frac{\partial}{\partial \theta} \left( \sin \frac{\theta \partial}{\partial \theta} \right) + \frac{1}{r^2 \sin^2 \theta} \frac{\partial^2}{\partial \phi^2}.
$$

