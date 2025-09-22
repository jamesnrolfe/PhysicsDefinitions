---
type: definition
aliases:
  - Controlled-G Gate
  - Controlled-G gate
  - Controlled-G gates
  - controlled-G gate
  - controlled-G gates
  - CG
  - CGs
  - CNOT
  - controlled-NOT
---
A controlled-G gate (CG) is a [[Quantum Gate|quantum gate]] that uses an extra qubit to control whether the gate is applied or not - like a switch. This can be represented as 
$$
CG \ket{0}  \ket{\psi}  = \ket{0} \ket{\psi} 
$$
for 'off' (the control qubit is 0) and 
$$
CG \ket{1} \ket{\psi} = \ket{1} G \ket{\psi} 
$$
for 'on' (the control qubit is 1). $G$ then is the operation on the state $\ket{\psi}$, if and only if the control qubit is 1. In a [[Quantum Circuit|quantum circuit]] diagram, this is denoted using a filled circle on the control line. 
![[Pasted image 20250921193918.png]]
A particularly useful example of such a gate is a **controlled-NOT** (**CNOT**) gate^[See [[Course Notes.pdf]] page 7 for diagramatic representation.]. Written as a matrix with respect to the [[Computational Basis|computational basis]], 
$$
CNOT=  \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0.
\end{pmatrix}
$$
