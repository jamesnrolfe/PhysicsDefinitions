---
type: definition
aliases:
  - the Schrödinger equation
---
**The Schrödinger equation** is a fundamental equation in quantum mechanics. It describes how the quantum state of a physics system evolves over time. For a single, non-relativistic particle of mass $m$ in a potential energy field $V(r,t)$, the [[Time-Dependent Schrödinger Equation|time-dependent Schrödinger equation]] is given by
$$
i\hbar \frac{\partial}{\partial t} \Psi(r,t) = \left[ - \frac{\hbar^2}{2m} \nabla ^2 + V(r, t)  \right] \Psi(r, t)
$$
where $\Psi(r,t)$ is the **wave function** of the particle, which contains all the probabilistic information about the particle's position, momentum and other measurable properties and $\nabla^2$ is the **Laplacian operator**, which represents the **kinetic energy** of the particle.

When the potential energy $V(r, t)$ is independent of time i.e. $V(r, t)=V(r)$, we can use a technique called [[Separation of Variables|separation of variables]] to simplify the equation. This leads to the [[Time-Independent Schrödinger Equation|time-independent Schrödinger equation]], given by
$$
-\frac{\hbar^2}{2m} \nabla^2 \psi(r) + V(r)\psi(r) = E\psi(r)
$$
where $\psi(r)$ is the **stationary state wave function** (i.e. it represents the spacial part of the wave function, and not its time evolution) and $E$ is the **energy eigenvalue** representing the total energy of the system.

This equation is an **eigenvalue equation**, where the Hamiltonian operator 
$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(r)
$$
acts on the wave function to return the same wave function, multiplied by the energy of the system
$$
\hat{H} \psi(r) = E \psi(r).
$$
### General Solution
If take the $\Psi(r, t)$ term in the [[Time-Dependent Schrödinger Equation|TDSE]] (the wave function), we can try and separate it out into the **spatial** and **time-dependent** parts. Let's first assume a separable solution as follows:
$$
\Psi(r, t) = \psi(r)\phi(t).
$$
Then, let's substitute this into the [[Time-Dependent Schrödinger Equation|TDSE]] 
$$
i\hbar \frac{\partial}{\partial t} (\psi(r)\phi(t)) = \hat{H}(\psi(r)\phi(t)).
$$
Since $\psi(r)$ does not depend on time and $\phi(t)$ does not depend on position, the partial derivatives simplify easily to
$$
i\hbar \psi(r) \frac{d}{dt}\phi(t) = \phi(t) \hat{H} \psi(r)
$$
(remember the **Hamiltonian** doesn't depend on time, only position). Then we will divide through by $\psi(r)\phi(t)$:
$$
\frac{i\hbar}{\phi(t)} \frac{d}{dt} \phi(t) = \frac{1}{\psi(r)} \hat{H} \psi(r).
$$
Now, for these two identities to be equal for all $r$ and $t$, both sides must be equal to a constant. This constant represents the total energy of the system, which we will call $E$.
#### Time dependent part
For the **time dependent part**, we can write the separated equation as
$$
i\hbar \frac{d\phi(t)}{dt} = E.
$$
This is a **first-order linear ordinary differential equation**. The solution to this is 
$$
\phi(t) = Ae^{-iEt / \hbar}
$$
The constant $A$ can be absorbed into the spatial part $\psi(r)$ by redefining $\psi'(r)=A\psi(r)$. We then write the time-dependent part as simply 
$$
\phi(t) = e^{-iEt / \hbar}.
$$
#### Time independent part
For the **spatial part**, we can write the separated equation as
$$
\frac{1}{\psi(r)} \hat{H} \psi(r) = E
$$
Multiplying by $\psi(r)$, we obtain the [[Time-Independent Schrödinger Equation|time-independent Schrödinger equation]]:
$$
\hat{H} \psi(r) = E \psi(r)
$$
This equation is a fundamental **eigenvalue equation**. $\psi(r)$ are the **eigenstates** of the **Hamiltonian**, representing the spatial part of the wave function for a state with a *definite energy*. We often denote them $\psi_{n}(r)$ to indicate that there can be many such solutions. $E$ are the **eigenvalues** of the **Hamiltonian**, and represent the **quantised** possible values of the total energy that the system can have. These are also typically denoted $E_{n}$.
#### Stationary states
Combining the solutions for $\psi(r)$ and $\phi(t)$, we get the **stationary state solutions** to the [[Time-Dependent Schrödinger Equation|TDSE]]:
$$
\Psi_{n}(r, t) = \psi_{n}(r)e^{-iE_{n}t / \hbar}
$$
These are called **stationary** because physical **observables** calculated from them (like **probability density** $|\Psi_{n}|^2$) do not change with time. This is because the time dependent factor $e^{-iE_{n}t / \hbar}$ cancels out when calculating probabilities or other observables (usually due to a modulus). 
### Spherical Symmetry
When there is **spherical symmetry**, it is often convenient to express the Schrödinger equation in terms of [[Coordinate Systems|spherical coordinates]] $(r, \theta, \phi)$ instead of [[Coordinate Systems|Cartesian coordinates]] $(x, y, z)$. The [[Laplacian]] in [[Coordinate Systems#Spherical Coordinates|spherical coordinates]] is given by
$$
\nabla^2 = \frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \right) + \frac{1}{r^2 \sin \theta} \frac{\partial}{\partial \theta} \left( \sin \frac{\theta \partial}{\partial \theta} \right) + \frac{1}{r^2 \sin^2 \theta} \frac{\partial^2}{\partial \phi^2}.
$$
If we substitute this into the [[Time-Independent Schrödinger Equation|time-independent Schrödinger equation]] and assuming a potential $V(r)$, we can assume that we can again apply separation of variables to the wave function 
$$
\psi(r, \theta, \phi) = R(r)Y(\theta, \phi)
$$
where $R(r)$ is the **radial part** and $Y(\theta, \phi)$ is the **angular part** of the wave function.

Then, if we plug this into the first term in the [[Time-Independent Schrödinger Equation|TISE]]:
$$
\begin{align}
-\frac{\hbar^2}{2m} &\left(\frac{1}{r^2} \frac{\partial}{\partial r} \left( r^2 \frac{\partial}{\partial r} \right) + \frac{1}{r^2 \sin \theta} \frac{\partial}{\partial \theta} \left( \sin \frac{\theta \partial}{\partial \theta} \right) + \frac{1}{r^2 \sin^2 \theta} \frac{\partial^2}{\partial \phi^2}\right)R(r)Y(\theta, \phi)   \\ 
&=-\frac{\hbar^2}{2m}\left( \frac{Y(\theta,\phi)}{r^2} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right) + \frac{R(r)}{r^2\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial Y(\theta,\phi)}{\partial \theta}\right) + \frac{R(r)}{r^2 \sin ^2\theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2}\right)
\end{align}
$$
where we have separated out the components into the derivatives they depend on, and taken the other one out. For example in the first term, $Y(\theta, \phi)$ does not depend on the derivative w.r.t. $r$ since it does not depend on $r$. The next step is divide through by $R(r)Y(\theta, \phi)$, and we get
$$
-\frac{\hbar^2}{2m}\left( \frac{1}{R(r)r^2} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right) + \frac{1}{Y(\theta, \phi)r^2\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial Y(\theta,\phi)}{\partial \theta}\right) + \frac{1}{Y(\theta, \phi)r^2 \sin ^2\theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2}\right).
$$
The next step is to multiple by $r^2$, and we get
$$
-\frac{\hbar^2}{2m}\left( \frac{1}{R(r)} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right) + \frac{1}{Y(\theta, \phi)\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial Y(\theta,\phi)}{\partial \theta}\right) + \frac{1}{Y(\theta, \phi) \sin ^2\theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2}\right).
$$
Now, we can clearly see that we have *separated out the variables* - the first term *only* depends on $r$, and the second two terms *only* depend on $\theta, \phi$. We have created **radial** and **angular** parts! Let's plug this back into the full [[Time-Independent Schrödinger Equation|TISE]]:
$$
-\frac{\hbar^2}{2m}\left( \frac{1}{R(r)} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right) + \frac{1}{Y(\theta, \phi)\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial Y(\theta,\phi)}{\partial \theta}\right) + \frac{1}{Y(\theta, \phi) \sin ^2\theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2}\right) +r^2V(r) = E r^2
$$
where we note that multiplied by $\psi(r) / r^2$ to account for the fact that we divided by $\psi(r)=R(r)Y(\theta, \phi)$ and multiplied by $r^2$ in the first term above. Let's move all the radial components to one side and all the angular components to the other.
$$
-\frac{\hbar^2}{2m}\left[ \frac{1}{R(r)} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right)\right] +r^2V(r)-Er^2 = \frac{\hbar^2}{2m} \left[\frac{1}{Y(\theta, \phi)\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial Y(\theta,\phi)}{\partial \theta}\right) + \frac{1}{Y(\theta, \phi) \sin ^2\theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2}\right].
$$
At this point, the LHS depends on *only* $r$, and the RHS depends *only* on the angles $\theta, \phi$. Now, for these two completely independent expressions to be equal for all values of $r$, $\theta$ and $\phi$, they *must both be equal to a constant*, which we will call $\lambda$. 

#### Angular part
For the **angular part**, we can rearrange it as follows:
$$ \frac{1}{\sin \theta} \frac{\partial}{\partial \theta} \left( \sin \theta \frac{\partial Y(\theta, \phi)}{\partial \theta} \right) + \frac{1}{\sin^2 \theta} \frac{\partial^2 Y(\theta, \phi)}{\partial \phi^2} = \frac{2m\lambda}{\hbar^2} Y(\theta, \phi).$$
It turns out for physically meaningful solutions, the constant $2m\lambda / \hbar^2$ must be equal to $-\ell(\ell+1)$, where $\ell$ is the **orbital angular momentum quantum number**. This is because the differential operator on the LHS is related to the square of the [[Orbital Angular Momentum|angular momentum operator]] $\hat{L}^2$. So, we get
$$
\left[\frac{1}{\sin \theta} \frac{\partial}{\partial \theta} \left( \sin \theta \frac{\partial }{\partial \theta} \right) + \frac{1}{\sin^2 \theta} \frac{\partial^2}{\partial \phi^2}\right]Y_{\ell, m}(\theta, \phi) = -\ell(\ell+1)Y_{\ell, m}(\theta, \phi).
$$
This is the equation whose solutions are the **spherical harmonics** $Y_{\ell, m}(\theta, \phi)$. We can further separate out into *independent* $\theta$ and $\phi$ terms. Let's first assume some separable solution
$$
Y(\theta, \phi) = \Theta(\theta) \Phi(\phi)
$$
and substitute into the angular equation using $\frac{\partial Y}{\partial \theta}=\Phi(\phi) \frac{d\Theta(\theta)}{d\theta}$ and $\frac{\partial^2 Y}{\partial \phi^2} = \Theta(\theta) \frac{d^2\Phi(\phi)}{d\phi^2}$,
$$
\frac{1}{\sin \theta} \frac{\partial}{\partial \theta}\left( \sin \theta \Phi(\phi) \frac{d\Theta(\theta)}{d\theta}  \right) + \frac{1}{\sin^2 \theta}\Theta(\theta) \frac{d^2\Phi(\phi)}{d\phi^2} = -\ell(\ell+1)\Theta(\theta)\Phi(\phi).
$$
Then, we can take the $\Phi(\phi)$ out of the first term, since it doesn't depend on $\theta$.
$$
\frac{\Phi(\phi) }{\sin \theta} \frac{\partial}{\partial \theta}\left( \sin \theta \frac{d\Theta(\theta)}{d\theta}  \right) + \frac{\Theta(\theta) }{\sin^2 \theta}\frac{d^2\Phi(\phi)}{d\phi^2} = -\ell(\ell+1)\Theta(\theta)\Phi(\phi).
$$
Then we will divide through by $\Theta(\theta)\Phi(\phi)$ and multiply by $\sin^2 \theta$,
$$
\frac{\sin \theta}{\Theta(\theta)} \frac{d}{d\theta}\left( \sin \theta \frac{d\Theta(\theta)}{d\theta} \right) + \frac{1}{\Phi(\phi)} \frac{d^2\Phi(\phi)}{d\phi^2} = -\ell(\ell+1)\sin^2\theta
$$
and now we rearrange terms so all the $\phi$-dependent terms are on one side and all $\theta$-dependent terms are on the other:
$$
\frac{1}{\Phi(\phi)} \frac{d^2\Phi(\phi)}{d\phi^2} = -\ell(\ell+1)\sin^2\theta - \frac{\sin \theta}{\Theta(\theta)} \frac{d}{d\theta} (\sin \theta) \frac{d\Theta(\theta)}{d\theta}.
$$
Now we can introduce the **separation constant** again, just as we did before, which we will this time call $\mu$.
##### Azimuthal part
For the **azimuthal part**, we can write 
$$
\frac{1}{\Phi(\phi)} \frac{d^2\Phi(\phi)}{d\phi^2} = \mu.
$$
For this, we are going to write $\mu=-m^2$, as will become clear. Rearranging, we find 
$$
\frac{d^2\Phi(\phi)}{d\phi^2}+m^2\Phi(\phi)=0
$$
which is just a **second-order differential equation**, with solutions of form
$$
\Phi(\phi) = Ae^{im\phi}+Be^{-im\phi}
$$
(which is why we set $\mu=-m^2$, so that we got simple terms in the exponent). For this function to be **single-valued** i.e. it satisfies $\Phi(\phi)=\Phi(\phi+2\pi)$, $m$ must be an integer $0, \pm{1}, \pm{2}, \dots$. This is where the **magnetic quantum number** $m$ is explicitly quantised. Often, we choose the $e^{im\phi}$ solution for simplicity, and absorb the constants into the **overall normalisation** $C_{\ell, m}$ (see below). 
##### Polar part
For the **polar part**, we can again set the term equal to a constant $-m^2$:
$$
-\ell(\ell+1)\sin^2\theta - \frac{\sin \theta}{\Theta(\theta)} \frac{d}{d\theta} (\sin \theta) \frac{d\Theta(\theta)}{d\theta} = -m^2.
$$
We can rearrange and multiply by $\Theta(\theta) / \sin^2\theta$ to get
$$
\frac{1}{\sin \theta} \frac{d}{d\theta} \left( \sin \theta \frac{d\Theta(\theta)}{d\theta} \right) - \frac{m^2}{\sin^2\theta} \Theta(\theta) = -\ell(\ell+1)\Theta(\theta)
$$
and then moving the $-\ell(\ell+1)$ to the LHS:
$$
\frac{1}{\sin \theta} \frac{d}{d\theta} \left( \sin \theta \frac{d\Theta(\theta)}{d\theta} \right) + \left[ \ell(\ell+1) - \frac{m^2}{\sin^2\theta} \right]\Theta(\theta)=0 .
$$
This is the [[Associated Legendre Differential Equation|associated Legendre differential equation]] (by performing a change of variables $x=\cos \theta$, this equation transforms into the standard form). For well-behaved, finite solutions over the range $0\leq \theta\leq \pi$, it is found that $\ell$ must be a **non-negative integer** ($\ell=0,1,2,\dots$) and $|m|$ must be less than or equal to $\ell$. The solutions to this equation are called the **Associated Legendre Polynomials** $P_{\ell}^m(\cos \theta)$ (sometimes written as $P_{\ell}^m(\theta)$).
##### Spherical harmonics
The **spherical harmonics** then look like 
$$
Y_{\ell, m} (\theta, \phi) = C_{\ell, m} P _{\ell}^m (\theta) e^{i m \phi}
$$
where $C_{\ell, m}$ is a normalisation constant such that 
$$
\int^{2\pi}_{0}\int ^\pi_{0} |Y_{\ell, m}(\theta, \phi)|^2 \sin \theta d\theta d\phi = 1
$$
usually given as 
$$
C_{\ell, m} = \sqrt{ \frac{2\ell+1}{4\pi} \frac{(\ell-m)!}{(\ell+m)!} },
$$
$P_{\ell}^m(\theta)$ are the **associated Legendre polynomials**. 

This product form clearly shows how the two quantum numbers $\ell$ and $m$ characterise the angular behaviour of the quantum mechanical wave function. Each pair of $(\ell, m)$ defines a **unique** spherical harmonic, which in turn describes a specific angular distribution in space for a quantum particle. 
#### Radial part
For the **radial part**,  we can rearrange it as 
$$
-\frac{\hbar^2}{2mR(r)} \frac{d}{dr} \left( r^2 \frac{dR(r)}{dr} \right) + r^2V(r)-Er^2 = \lambda
$$
In the above, we said that $2m\lambda/\hbar^2=-\ell(\ell+1)$, and so
$$
\lambda=-\frac{\hbar^2l(l+1)}{2m}
$$
so
$$
-\frac{\hbar^2}{2mR(r)} \frac{d}{dr} \left( r^2 \frac{dR(r)}{dr} \right) + r^2V(r)-Er^2 = -\frac{\hbar^2l(l+1)}{2m}.
$$
Then multiply by $R(r) / r^2$ and we get
$$
-\frac{\hbar^2}{2m} \frac{1}{r^2} \frac{d}{dr} \left( r^2 \frac{dR(r)}{dr} \right) +V(r)R(r) - ER(r) = \frac{\hbar^2\ell(\ell+1)}{2mr^2}R(r)
$$
and rearrange to the standard form for this equation
$$
-\frac{\hbar^2}{2m} \frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{dR(r)}{dr} \right) + \left[ V(r)+\frac{\hbar^2\ell(\ell+1)}{2mr^2} \right]R(r)= ER(r)
$$
This is the **Radial Schrödinger equation**. The term $\hbar^2\ell(\ell+1) / 2mr^2$ acts as an effective potential term, known as the **centrifugal barrier**, which arises from the [[Orbital Angular Momentum|angular momentum]] of the particle.  