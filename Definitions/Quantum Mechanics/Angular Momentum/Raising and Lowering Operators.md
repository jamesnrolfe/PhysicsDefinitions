---
type: definition
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

If we look at the angular part of [[The Schrödinger Equation|the Schrödinger equation]], we find the solutions are the **spherical harmonics**
$$
Y_{\ell, m} (\theta, \phi) = C_{\ell, m} P _{\ell}^m (\theta) e^{i m \phi}
$$

Then, if we apply the **raising operator** to this angular part, we find trivially if $m=\ell$
$$
\hat{L}^+ Y_{\ell, m} =0.
$$
However, if $m<\ell$
$$\begin{align}
\hat{L}^z(\hat{L}^+Y_{\ell,m})&=(m+1)\hbar(\hat{L}^+Y_{\ell,m}), \\
\vec{L}^2(\hat{L}^+ Y_{\ell,m}) &= \ell(\ell+1)\hbar^2(\hat{L}^+Y_{\ell,m}).
\end{align}$$
This is interesting! Compare to the eigenvalues of just $\hat{L}^z$ and $\hat{L}^2$ on $Y_{\ell, m}$:
$$
\hat{L}^z Y_{\ell, m} = m \hbar Y_{\ell, m}, \quad \hat{L}^2 Y_{\ell, m} = \ell(\ell+1) \hbar^2 Y_{\ell, m}.
$$
We can see that the raising operator has no effect on $\hat{L}^2$ - it produces the same eigenvalue. However, interestingly, the eigenvalue of $\hat{L}^z$ is *raised* by one unit of $\hbar$. This is why the operator $\hat{L}^+$ is called the **raising operator**. A very similar process can be done with the **lowering operator**:
$$
\begin{align}
\hat{L}^z(\hat{L}^-Y_{\ell,m})&=(m-1)\hbar(\hat{L}^+Y_{\ell,m}), \\
\vec{L}^2(\hat{L}^- Y_{\ell,m}) &= \ell(\ell+1)\hbar^2(\hat{L}^+Y_{\ell,m}).
\end{align}
$$
which instead lowers the eigenvalue by one unit of $\hbar$. Their eigenvalue equations are 
$$
\begin{align}
\hat{L}^+ Y_{\ell, m} &= A Y_{\ell, m+1}, \\
\hat{L}^- Y_{\ell, m} &= B Y_{\ell, m-1}.
\end{align}
$$
We can also show that 
$$
[\hat{L}^-, \hat{L}^+] = 2\hbar \hat{L}^z
$$
