---
type: definition
aliases:
  - angular momentum operators
  - Angular momentum operators
  - orbital angular momentum
---
### Orbital angular momentum
The **orbital angular momentum** can be thought of as the *actual* angular momentum that a particle has, for example that that an **electron** would have when orbiting a nucleus.
### Orbital angular momentum operators
Classically, we think of angular momentum $\vec{L}$ as being given by 
$$
\vec{L}=\vec{r} \times \vec{p}
$$
where $\vec{r}$ is the **position vector** of the particle, and $\vec{p}$ is the **momentum vector**. In quantum mechanics, the equation looks *exactly the same*:
$$
\hat{L}=\hat{r} \times \hat{p}
$$
where we now use the [[Operators|operator]] form instead.

We define angular momentum about each **axis** as $\hat{L}^x$, $\hat{L}^y$ and $\hat{L}^z$. This means that the angular momentum along the $z$-axis would amount to spinning in the $x$-$y$ plane. In other words, *the direction of the angular momentum operator is perpendicular to the plane of rotation*. Generally, we use $\hat{L}^z$ for simplicity.

These operators [[Operators#Commutation|commute]] via $[\hat{L}^x,\hat{L}^y] = i\hbar\hat{L}^z$ (cyclic). 

There is another operator that we use a lot, defined as $\vec{L}^2=(\hat{L}^x)^2 + (\hat{L}^y)^2 +(\hat{L}^z)^2$. This can be thought of as the **square magnitude** of angular momentum. 

It is true that $[\hat{L}^z, \vec{L}^2]=0$, which by [[Operators#Commutation|commutator rules]] means that states exist that are **eigenstates** of *both of these* operators. In fact, these states are the angular component of the eigenstates of the [[The Schrödinger Equation#Angular part|Schrödinger equation]] $Y_{\ell, m}(\theta, \phi)$. The corresponding **eigenvalues** are 
$$
\hat{L} Y_{\ell, m} = m \hbar Y_{\ell, m}
$$
and 
$$
\vec{L}^2 Y_{\ell, m} = \ell(\ell+1) \hbar^2 Y_{\ell, m}.
$$
In fact, this is exactly how $m$ and $\ell$ are *defined* - they relate to the **eigenvalues** of the angular momentum operators.
The values of $m$ and $l$ are such that 
$$
-l \leq m \leq l.
$$
For example, if $l=1$, $m$ can take the values $-1$, $0$ or $1$. 