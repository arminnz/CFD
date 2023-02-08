# CFD

## Continuity equations of fluid flow and heat transfer

The mass of the fluid is conserved.
Rate of increase of mass in fluid = Net rate of flow of mass into fluid element

The term on the left is representing the unsteady nature of a regime which equals the net rate of what enters our control volume and what exits.
$$\partial(\rho\delta x\delta y\delta z)/\partial t$$
of course the $\delta  x, \delta y\, \delta z $ are constants so they are moved out of the deravitive. That leaves $\partial \rho/\partial t$. This is the term that represents *"Rate of increase of mass in fluid"*.
For the phrase *"Net rate of flow of mass into fluid"* we would need to take into account what enters and what exits the control volume. If we assume since the control volume is very small the value of density on the left surface to the control center point is linearly smaller than the center point and carry out the algebra we achieve the following:
