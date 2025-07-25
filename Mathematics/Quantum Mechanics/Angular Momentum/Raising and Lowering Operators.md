---
type: maths
aliases:
  - raising and lowering operators
  - raising operator
  - lowering operator
---
The raising and lowering operators are defined as 
$$
\hat{L}^+ := \hat{L}^x + i\hat{L}^y \, , \quad \hat{L}^- := \hat{L}^x - i\hat{L}^y
$$
respectively. They have the effect of "raising" or "lowering" the quantum numbers of a state.

### Where do they come from?
When we study the **eigenstates** of the [[The Schrödinger Equation|Schrödinger equation]] for the Hydrogen atom (for simplicity), we extract an **angular part** that looks like:
$$
Y_{\ell, m} (\theta, \phi) = C_{\ell, m} P _{\ell}^m (\theta) e^{i m \phi}
$$
where $P_{\ell}^m$ are **polynomials** in $\cos \theta$ and/or $\sin \theta$ of degree $\ell$ (called the **associated Legendre polynomials**) and $C_{\ell,m}$ is some normalisation constant. 

Then, if we apply the raising operator to this angular part, we find if $m=\ell$
$$
\hat{L}^+ Y_{\ell, m} =0.
$$
However, if $m<\ell$
$$\begin{align}
\hat{L}^z(\hat{L}^+Y_{\ell,m})&=(m+1)\hbar(\hat{L}^+Y_{\ell,m}), \\
\vec{L}^2(\hat{L}^+ Y_{\ell,m}) &= \ell(\ell+1)\hbar^2(\hat{L}^+Y_{\ell,m}).
\end{align}$$
