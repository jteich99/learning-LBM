# Kinetic Theory 
Particle distribution function: $f(x, \xi, t)$.
- generalization of density $\rho$ taking into account the microscopic particle velocity
- represent the density of particles with a certain velocity $\xi$ at a certain position $x$ for time $t$
- $x$ = particle position
- $\xi$ = microscopic particle velocity
- $t$ = time
- [$f$] = $\frac{\text{kg}\,\text{s}^3}{\text{m}^6}$ 

From the particle distribution function you can recover macroscopic variables such as:
- density $\rho$
- momentum density $\rho\,\mathbf{u}$
- total energy density $\rho\,E$
- internal energy density $\rho\,e$

$f(x, \xi, t)$ reaches an equilibrium distribution $f^\text{eq}(x, \xi, t)$

## The Boltzmann Equation
Total derivative of the particle distribution function $\Omega(f) = \frac{d\,f}{d\,t}$:

$
\frac{\partial f}{\partial t} + \xi_\beta \frac{\partial f}{\partial x_\beta} + \frac{F_\beta}{\rho} \frac{\partial f}{\partial \xi_\beta} = \Omega (f)
$

- first 2 terms represent the advection of $f$ due to $\xi$
- 3rd term represent the forces affecting $\xi$
- $\Omega$ is a source term called the **collision operator**

Conservation laws:
- mass conservation: $\int \Omega(f)\, d^3\xi = 0$
- momentum conservation: $\int \mathbf{\xi}\, \Omega(f)\, d^3\xi = \mathbf{0}$
- total energy conservation: $\int |\mathbf{\xi}|^2\, \Omega(f)\, d^3\xi = 0$
- internal energy conservation: $\int |\mathbf{v}|^2\, \Omega(f)\, d^3\xi = 0$

The collision operator is usually simplified to the **BGK collision operator**:

$
\Omega(f) = \frac{1}{\tau} (f - f^\text{eq})
$

begin $\tau$ the relaxation time, this operator captures the relaxation of the distribution function towards equilibrium.

## The Boltzmann H-Theorem
Molecular collisions invariably drive the distribution function towards equilibrium.
