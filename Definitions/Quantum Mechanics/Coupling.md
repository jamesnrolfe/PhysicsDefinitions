---
type: definition
aliases:
  - coupling
  - couples
  - couple
---
In quantum mechanics, **coupling** between states refers to the ability of the [[Hamiltonian]] to induce transitions between them. If two states, $\ket{\psi_{1}}$ and $\ket{\psi_{2}}$ are *coupled*, it means that the Hamiltonian has a non-zero matrix element between them:
$$
\langle \psi_{1} | \hat{H} | \psi_{2} \rangle \neq 0.
$$
This allows the system to transition from $\ket{\psi_{2}}$ to $\ket{\psi_{1}}$ or vice-versa, without changing the overall energy of the system. 

If $\hat{H}$ [[commutes]] with another operator representing some physical quantity, $\hat{A}$, it means that:
- $\hat{A}$ is **conserved** (in time).
- The Hamiltonian **cannot** induce transitions between different states that have *different [[eigenvalues]] of $\hat{A}$*. In other words, if you have a basis of states that are eigenvalues of $\hat{A}$ $\{ \ket{a_{1}}, \ket{a_{2}}, \dots \}$, then the Hamiltonian will have zero matrix elements between states with different $\hat{A}$ eigenvalues $$
\langle a_{i} | \hat{H}|a_{j}\rangle =0 \quad \text{if} \; a_{i} \neq a_{j}.
	$$This means that the Hamiltonian matrix, when written in the basis of $\hat{A}$ eigenstates, will be **block-diagonal**, with each block corresponding to a specific eigenvalue of $\hat{A}$. 