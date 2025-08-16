---
type: maths
aliases:
  - coupled spins
---
When spins interact with each other, new phenomena can arise, such as large-scale [[Ferromagnetism|ferromagnetism]] or [[Anti-ferromagnetism|anti-ferromagnetism]]. 
### Two interacting Spin-$\frac{1}{2}$'s
>See [[Spin Angular Momentum]] for context.

Suppose we have just two atoms, each with [[Spin Angular Momentum|spin]]-$\frac{1}{2}$, interacting with an [[Isotropic|isotropic]] exchange interaction $J$ (Heisenberg exchange). The [[Hamiltonian]] is then
$$
\hat{H}=J \vec{S}_{1} \cdot \vec{S}_{2}.
$$
Classically, the energy of this system depends on the **angle** between the spins since
$$
\vec{S}_{1} \cdot \vec{S}_{2} = S_{1}S_{2} \cos \theta.
$$
Since both atoms are [[Spin Angular Momentum|spin]]-$\frac{1}{2}$, $S_{1}=S_{2}=\frac{1}{2}$ so
$$
E_{\text{classical}} = \frac{1}{4} J \cos \theta
$$
and since $-1\leq \cos \theta\leq 1$, all energies are possible between $+\frac{1}{4}J$ and $-\frac{1}{4}J$.

Quantum mechanically, we need to find all the energy eigenstates of the system to find the allowed energies. First, we can write down a [[complete orthonormal basis]] of states for the system. Then, we can write $\hat{H}$ as a **matrix** using this basis and then [[diagonalise]] to find the [[eigenstates]].

Using the subscript 1 for the first [[Spin Angular Momentum|spin]], then a basis for the first spin consists of the two [[eigenstates]] of $\hat{S}_{1}^z$, namely $\ket{+}_{1}$ and $\ket{-}_{1}$. Similarly, $\ket{+}_{2}$ and $\ket{-}_{2}$ form a basis for the second spin: [[eigenstates]] of $\hat{S}^z_{2}$. A basis for this pair can then be written as all possible combinations of these states, i.e. the set
$$
\{\ket{++} , \ket{+ -} , \ket{- +} , \ket{--} \}
$$
where $\ket{+} \equiv \ket{+}_{1}\ket{+}_{2}$ etc. Hence the matrix for $\hat{H}$ will be of size $4 \times 4$. 

It is useful now to rewrite the [[Hamiltonian]] as follows
$$
\hat{H}=J \vec{S_{1}} \cdot \vec{S}_{2} = J(\hat{S}_{1}^z\hat{S}_{2}^z + \frac{1}{2}\hat{S}^+_{1}\hat{S}^-_{2}+\frac{1}{2}\hat{S}_{1}^-\hat{S}_{2}^+)
$$
using [[Spin Angular Momentum#^39ec1f|this result]]. Now consider the effect of the [[Hamiltonian]] operating on each combination of the basis states, noting the following conditions:
1. All operators acting on *different* atoms [[commute]] i.e. $[\hat{S}_{1}^x\hat{S}_{1}^y]=0$.
2. $S_{1}$ operators act *only* on the first spin, and have *no effect* on the second, and similar for $S_{2}$.
It is simplest to do this by considering each term in the [[Hamiltonian]] in turn. First consider $\hat{S}_{1}^z\hat{S}_{2}^z$.
$$
\begin{align}
\hat{S}_{1}^z \hat{S}_{2}^z \ket{++}  & = \frac{1}{2} \cdot \frac{1}{2} \ket{++} = \frac{1}{4} \ket{++}  \\
\hat{S}_{1}^z \hat{S}_{2}^z \ket{+ -}  & =-\frac{1}{4} \ket{+ -} \\
\hat{S}_{1}^z \hat{S}_{2}^z \ket{- +}  & = -\frac{1}{4} \ket{ - +} \\
\hat{S}_{1}^z \hat{S}_{2}^z \ket{--}  & = \frac{1}{4} \ket{- -}  .   
\end{align}
$$
Now we can consider $\hat{S}^+_{1}\hat{S}_{2}^-$ operating on each basis state. We can use the results from [[Spin Angular Momentum#Spin operators|Spin Operators]]. Since $\hat{S}_{1}^+ \ket{+} = 0$, it follows that $\hat{S}_{1}^+ \ket{++}=0$ etc., and so
$$
\begin{align}
\hat{S}_{1}^+\hat{S}_{2}^- \ket{++}  & = 0 \\
\hat{S}_{1}^+\hat{S}_{2}^-  \ket{+ -}  & = 0 \\
\hat{S}_{1}^+\hat{S}_{2}^-  \ket{- +}  & = \ket{+ -} \\
\hat{S}_{1}^+\hat{S}_{2}^-  \ket{- -} & = 0     
\end{align}
$$
and similarly
$$
\begin{align}
\hat{S}_{1}^-\hat{S}_{2}^+ \ket{++}  & = 0 \\
\hat{S}_{1}^-\hat{S}_{2}^+  \ket{+ -}  & = \ket{- +}  \\
\hat{S}_{1}^-\hat{S}_{2}^+  \ket{- +}  & = 0 \\
\hat{S}_{1}^-\hat{S}_{2}^+  \ket{- -} & = 0     
\end{align}
$$
Using all of these results together, we can find the effects of the [[Hamiltonian]] on the set of basis states.
$$
\begin{align}
\hat{H} \ket{++}  & = \frac{1}{4}J \ket{++}  \\
\hat{H} \ket{+ -}  & = -\frac{1}{4}J \ket{+ -} + \frac{1}{2} J \ket{- +} \\
\hat{H} \ket{- +}  & = -\frac{1}{4}J\ket{- +} + \frac{1}{2}J\ket{+ - }  \\
\hat{H} \ket{--}  & = \frac{1}{4}J \ket{--}  
\end{align}
$$
which means that in matrix form (where the rows represent the basis states, in the order we have provided), we find
$$
\hat{H} = J\begin{pmatrix}
\frac{1}{4} & 0 & 0 & 0 \\
0 & -\frac{1}{4} & \frac{1}{2} & 0 \\
0 & \frac{1}{2} & -\frac{1}{4} & 0 \\
0 & 0 & 0 & \frac{1}{4}
\end{pmatrix}
$$
Omitting $J$ for simplicity, we can find the [[eigenvalues]] of this matrix, using
$$
\begin{vmatrix}
\frac{1}{4}- E & 0 & 0 & 0 \\
0 & -\frac{1}{4}-E & \frac{1}{2} & 0 \\
0 & \frac{1}{2} & -\frac{1}{4}-E & 0 \\
0 & 0 & 0 & \frac{1}{4}-E
\end{vmatrix} = 0
$$
and so it follows that 
$$
\begin{align}
\left( \frac{1}{4}-E \right)^2 \begin{vmatrix}
-\frac{1}{4}-E & \frac{1}{2} \\
\frac{1}{2} & -\frac{1}{4}-E 
\end{vmatrix} & = 0 \\
\left( \frac{1}{4}-E \right)^2 \left[ \left( \frac{1}{4}+E \right)^2-\frac{1}{4} \right] & =0 \\
\left( \frac{1}{4}-E \right)^2\left[ \left( \frac{1}{4}+E \right)+\frac{1}{2} \right]\left[ \left( \frac{1}{4}-E \right)-\frac{1}{2} \right] & =0
\end{align}
$$
which is factorised, and so produces results $E=\frac{1}{4}, \frac{1}{4}, \frac{1}{4}, -\frac{3}{4}$. Hence there are **two** allowed energies of this system only (reintroducing $J$):
$$
E=\frac{J}{4}, \quad E=-\frac{3J}{4}
$$
where the first forms a **triplet** and the second is a **singlet**.

The maximum eigenvalue here: $\frac{J}{4}$ is the same as the classical case. However, the minimum eigenvalue: $-\frac{3J}{4}$ is much lower. This is clearly a *new quantum effect*. 

We might also find the eigenvectors of this matrix, to which we would get 
$$
\psi_{1}=\begin{bmatrix}
1 \\
0 \\
0 \\
0
\end{bmatrix}, \quad \psi_{2} = \begin{bmatrix}
0 \\
\frac{1}{\sqrt{ 2 }} \\
\frac{1}{\sqrt{ 2 }} \\
0
\end{bmatrix}, \quad \psi_{3} = \begin{bmatrix}
0 \\
0 \\
0 \\
1
\end{bmatrix}, \quad \psi_{4} = \begin{bmatrix}
0 \\
\frac{1}{\sqrt{ 2 }} \\
-\frac{1}{\sqrt{ 2 }} \\
0
\end{bmatrix}
$$
with the first three having eigenvalue $\frac{J}{4}$ and $\psi_{4}$ having eigenvalue $-\frac{3J}{4}$.
