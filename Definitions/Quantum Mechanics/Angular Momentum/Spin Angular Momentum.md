---
type: definition
aliases:
  - spins
  - spin
  - spin angular momentum
  - intrinsic angular momentum
---
### Spin
The spin of a particle is an **intrinsic** property of that particle - much like **mass** or **charge**. 
It is often thought of as the particle "spinning" on its axis - but this is incorrect (electrons are thought to be point particles for example, and so have no axis to spin on). It is however related to angular momentum. It suggests that particles have some inherent angular momentum, even when *not physically rotating*.

Spin can take **integer** or **half-integer** values, depending on the type of particle.

| Particle Group           | Spin                                | Examples                     | Description                                                                         |
| :----------------------- | :---------------------------------- | :--------------------------- | :---------------------------------------------------------------------------------- |
| [[Fermions]]             | Half-integer spin (\(½, ³/₂, ...\)) | Electrons, Quarks, Neutrinos | Matter particles that obey [[Pauli Exclusion Principle\|Pauli exclusion principle]] |
| [[Bosons]]               | Integer spin (\(0, 1, 2, ...\))     | Photons, Gluons, Higgs Boson | Force-carrying particles and particles that can occupy same quantum state           |
| Fundamental [[Fermions]] | ½                                   | Quarks, Leptons              | Basic building blocks of matter                                                     |
| Fundamental [[Bosons]]   | 1                                   | Photon, W/Z Bosons, Gluons   | Fundamental force carriers                                                          |
| Composite [[Fermions]]   | Depends on constituents             | Protons, Neutrons            | Made of quarks with combined spin                                                   |
| Composite [[Bosons]]     | Depends on constituents             | Helium-4 atoms               | Particles with **integer** total spin                                               |
### Spin operators

^641449

The **spin angular momentum** has most of the same properties as [[Orbital Angular Momentum|orbital angular momentum]], but also some *special* properties.

We will write $\hat{S}$ for spin in place of $\hat{L}$ in [[Orbital Angular Momentum|orbital angular momentum]]. We can still use the eigenstates of $\hat{S}^z$ and $\vec{S}^2$ with the same quantum numbers $\ell$ and $m$, such that $$\begin{align} \hat{S}^z \ket{\ell, m} &=m\hbar \ket{\ell, m} \\\hat{S}^2 \ket{\ell, m} &= \ell(\ell+1)\hbar^2\ket{\ell, m} 
 \end{align}$$ as before.

Clearly, the spin eigenstate $\ket{\ell, m}$ behaves here just like the [[Orbital Angular Momentum|orbital]] eigenstate $Y_{\ell, m}$, but there are *two fundamental differences*:
1. $\ket{\ell, m}$ does not have an explicit form in terms of $\theta$ and $\phi$ like $Y_{\ell, m}$. 
2. $\ell$ may now be an integer, as before, *or* a **half-integer**.
The values of $m$ still differ by unity and still take all the values between $-\ell$ and ${} +\ell$, but if $\ell$ is an integer $+\frac{1}{2}$ then so are the $m$. For example:
- If $\ell= \frac{3}{2}$ then the possible values of $m$ are $- \frac{3}{2}, -\frac{1}{2}, \frac{1}{2}, \frac{3}{2}$.
- If $\ell=\frac{1}{2}$ then $m$ can be $-\frac{1}{2}$ or $\frac{1}{2}$.
Let's continue with the $\ell=\frac{1}{2}$ example. Hence, the state $\ket{l,m}$ take two values:
$$
\ket{\frac{1}{2}, \frac{1}{2}} \quad \text{or} \quad \ket{\frac{1}{2}, -\frac{1}{2}}
$$
which are the **two eigenstates** of $\hat{S}^z$. In this example, we can abbreviate
$$
\begin{align}
\ket{\frac{1}{2}, \frac{1}{2}}  & \equiv \ket{\frac{1}{2}} \equiv \ket{+}   \\
\ket{\frac{1}{2}, -\frac{1}{2}}  & \equiv \ket{-\frac{1}{2}} \equiv \ket{-} 
\end{align}
$$
These two eigenstates form a complete set for a single spin-$\frac{1}{2}$. They may be written
$$
\psi=\alpha \ket{+} +\beta \ket{-} .
$$
The eigenstates form an **orthonormal basis** i.e.
$$
\langle{+}|{+}\rangle = \langle{-}|{-}\rangle = 1, \quad \langle{+}|{-}\rangle=0.
$$
We often assume that we are working in units of $\hbar$ which has the value $1$. 

We can see that
$$
\hat{S}^z\ket{+} =\hat{S}^z\ket{\frac{1}{2}, \frac{1}{2}} = \frac{1}{2}\hbar \ket{\frac{1}{2}, \frac{1}{2}} \equiv \frac{1}{2} \ket{+}
$$
and similarly
$$
\hat{S}^z\ket{-} = -\frac{1}{2}\ket{-} .
$$
Also we have the spin [[Raising and Lowering Operators|raising and lowering operators]] which act identically to the angular momentum alternatives, namely
$$
\hat{S}^±\ket{\ell, m}  = \begin{cases}
0 & \text{if} \,\, m = ±\ell \quad \text{(for raising use positive, lowering use negative)}\\
\hbar \sqrt{ \ell(\ell+1)-m(m ± 1) } \ket{\ell, m±1} & \text{if} \,\,m < \ell
\end{cases}  
$$
$$
\hat{S}^+ \ket{+} = \hat{S}^+\ket{\frac{1}{2}, \frac{1}{2}} =0

$$
as well as 
$$
\hat{S}^+ \ket{-} = \hat{S}^+\ket{\frac{1}{2}, -\frac{1}{2}} = \hbar \sqrt{ \frac{1}{2}\left( \frac{1}{2}+1 \right) +\frac{1}{2}\left( -\frac{1}{2} +1 \right)} \ket{\frac{1}{2}, \frac{1}{2}} = \hbar \sqrt{ \frac{3}{4}+\frac{1}{4}} = \hbar \ket{+} \equiv\ket{+} 
$$
where we remember that $\hbar=1$ in these units.
We can do the same for $\hat{S}^-$ and we get the following results.
$$
\hat{S}^-\ket{+} = \ket{-}; \quad \hat{S}^- \ket{-} = 0
$$

>[!example] Single Spin-1 Example
> For a single spin-1 particle, we would have $l=1$ and thus $m=1,0,-1$. Again, we use a simplified notation
> $$\ket{1,1} \equiv \ket{1} \equiv \ket{+} $$
> as well as 
> $$\ket{1,0} \equiv \ket{0} $$
> and 
> $$\ket{1,-1} \equiv \ket{-1} \equiv \ket{-1} .  $$
> Note here that $\ket{+}$ and $\ket{-}$ are not the same states as before. They are just notational tools, so we can make them whatever. They represent a similar idea, but not the exact same one.
> Hence there are three possible states we need to consider: $\ket{+}, \ket{0}$ and $\ket{-}$.
> What are the effects of the [[Raising and Lowering Operators|raising and lowering operators]] as well as the spin-$z$ operator $S^z$?
> We just do the exact same as before, and get for $\hat{S}^+$
> $$\hat{S}^+\ket{+} = \hat{S}^+\ket{1, 1} = 0  $$
> as well as 
> $$\hat{S}^+\ket{0} = \hat{S}^+\ket{1, 0} = \sqrt{ 1(1+1) - 0(0+1) }\ket{1, 1} = \sqrt{ 2 }\ket{+}    $$
> and 
> $$\hat{S}^+ \ket{-} = \hat{S}^+\ket{1, -1} = \sqrt{ 1(1+1) + 1(-1 + 1) } \ket{1, 0} =\sqrt{ 2 }\ket{0}. $$
> We get similar results for $\hat{S}^-$:
> $$\hat{S}^- \ket{+} = \sqrt{ 2 }\ket{0} ; \quad \hat{S}^-\ket{0} = \sqrt{ 2 }\ket{-} ; \quad \hat{S}^- \ket{-} = 0 $$
> For $\hat{S}^z$, we can simply use $\hat{S}^z\ket{\ell, m}=m\hbar \ket{\ell, m}$ with $\hbar=1$ to find
> $$\hat{S}^z\ket{+} = \ket{+} ; \quad \hat{S}^z \ket{0} = 0; \quad \hat{S}^z \ket{-} = -\ket{-} $$

>[!info] Useful result
>A useful result to note, especially with [[Coupled Spins|coupled spins]], is
>$$\vec{S_{1}} \cdot \vec{S}_{2} = \hat{S}_{1}^z\hat{S}_{2}^z + \frac{1}{2}\hat{S}^+_{1}\hat{S}^-_{2}+\frac{1}{2}\hat{S}_{1}^-\hat{S}_{2}^+$$
>This can be seen from 
>$$\hat{S}_{1}^+\hat{S}_{2}^- = (\hat{S}_{1}^x+i\hat{S}_{1}^y)(\hat{S}_{2}^x-i\hat{S}_{2}^y) = \hat{S}_{1}^x\hat{S}_{2}^x+\hat{S}_{1}^y\hat{S}_{2}^y + i(\hat{S}_{1}^y\hat{S}_{2}^x-\hat{S}_{1}^x\hat{S}_{2}^y)$$
>and similarly 
>$$\hat{S}_{1}^-\hat{S}_{2}^+ = \hat{S}_{1}^x\hat{S}_{2}^x+\hat{S}_{1}^y\hat{S}_{2}^y - i(\hat{S}_{1}^y\hat{S}_{2}^x-\hat{S}_{1}^x\hat{S}_{2}^y)$$
>and so 
>$$\hat{S}_{1}^+\hat{S}^-_{2}+\hat{S}_{1}^-\hat{S}_{2}^+ = 2(\hat{S}_{1}^x\hat{S}_{2}^x+\hat{S}_{1}^y\hat{S}_{2}^y).$$
>Then using the definitions of $\vec{S}_{1}$ and $\vec{S}_{2}$, we can say that 
>$$\vec{S}_{1} \cdot \vec{S}_{2} = \hat{S}_{1}^x\hat{S}_{2}^x + \hat{S}_{1}^y \hat{S}_{2}^y + \hat{S}_{1}^z \hat{S}_{2}^z = \hat{S}_{1}^z\hat{S}_{2}^z + \frac{1}{2}\hat{S}^+_{1}\hat{S}^-_{2}+\frac{1}{2}\hat{S}_{1}^-\hat{S}_{2}^+$$

^39ec1f

