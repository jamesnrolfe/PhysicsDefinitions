---
type: definition
aliases:
  - action
---
The action is a defined as
$$
S[q_{i}] = \int_{t_{0}}^{t_{f}} L dt
$$
where $L$ is the [[Lagrangian]] for the system.

Classical paths **extremise** the action. To do this, they satisfy
$$
\left( \frac{\partial S[q_{i} + \lambda \varepsilon_{i}]}{\partial \lambda} \right) \Bigg | _{\lambda=0} =0
$$
where $\varepsilon_{i}$ is a slight variation from the classical path, satisfying the boundary conditions
$$
\varepsilon_{i}(t_{0}) = \varepsilon_{i}(t_{f}) = 0
$$
i.e. the start and end points are the same for the varied path and the original path.

>[!help] Why does that equation extremise the action?
>By extremise, we mean finding a **mimimum**, **maximum** or **saddle point**. It is almost identical to finding the point where the gradient of a regular function is zero i.e.
>$$\frac{df}{dx}=0.$$
>But we are working with [[Functional|functionals]] here. It's input $q_{i}(t)$ is a path and it assigns a number to every single path that the system could possibly have. So, the variable here is the path. We want to find the path that extremises the action. However, if we wanted to check every path, we can't just "add one" to the path. Instead, we add a small variation $\lambda\varepsilon_{i}$, which is then a slightly different path. When $\lambda=0$, we are on the original path (since the variation is zero). $\lambda$ can be thought of as a measure of *how far* we are from the original path.
>Then, when we find $\frac{\partial S}{\partial \lambda}$, we are asking "how does the action change as we vary the path". So, what we are asking with
>$$\left( \frac{\partial S[q_{i} + \lambda \varepsilon_{i}]}{\partial \lambda} \right) \Bigg | _{\lambda=0} =0$$
>is "what path exists that when we add an infinitesimally small variation to it, the gradient is zero". This is equivalent to finding a minimum, maximum or saddle point for a regular function, thus we have extremised it. 
