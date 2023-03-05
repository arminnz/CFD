# CFD

## Continuity equations of fluid flow and heat transfer

The mass of the fluid is conserved.
Rate of increase of mass in fluid = Net rate of flow of mass into fluid element

The term on the left is representing the unsteady nature of a regime which equals the net rate of what enters our control volume and what exits.
$$\partial(\rho\delta x\delta y\delta z)/\partial t$$
of course the $\delta  x, \delta y\, \delta z $ are constants so they are moved out of the deravitive. That leaves $\partial \rho/\partial t$. This is the term that represents *"Rate of increase of mass in fluid"*.
For the phrase *"Net rate of flow of mass into fluid"* we would need to take into account what enters and what exits the control volume. If we assume since the control volume is very small the value of density on the left surface to the control center point is linearly smaller than the center point and carry out the algebra we achieve the following:
*formula*
The equation above is the unsteady three dimensional mass conservation or continuity eqaution for a compressible fluid. Naturally, for a steady incompressible fluid the equation becomes:
*formula div u=0*
Generally there are two approaches to CFD. One is the Lagrangian approach where a rate of change of for instance property $\phi$ is defined and to develop numerical methods for fluid flow calculations by tracking the motion and computing the rates of change of property $\phi$. In order to find the rates of change we would need to know the definition of the total or substantive derivative:
*formual 2.7*
As opposed to Lagrangian approach we have the Eulerian approach where rather than following the particles, a method is developed to monitor the motion and rates of changes of properties within a fixed region in space or rather a collection of fluid elements. The Eulerian approach is far more common.

We would need a general term which explains the relationship between the substantive derivative $\phi$, and the rate of change of $\phi$ for a fluid element. 
Taking the continuity equation we can generalise the terms for an arbitrary conserved property :
*formula 2.9*
If we expant the divergence we get:
*formula 2.10*
the last part on the right hand side is actually the continuity equation which is equal to zero. 
The first part on the right hand side is actually the substantive derivative. Meaning that equation is words is:
Rate of increase of $\phi$ of fluid element+ Net rate of flow of $\phi$ out of fluid element = Rate of increase of $\phi$ for a fluid particle.

With the equation above we can obtain the rate of increase of $\phi$ for a fluid particle by analyzing the fluid element.

We can exchnage $\phi$ with velocities in three direction to obtain the momentum equations, energy to obtain the energy equations.

## Momentum equations
Newton's second law states that the rate of change of momentum of a fluid is equal to the sum of the forces in the particle. Rates of increase of x,y and z momentum per unit volume of a fluid particle is expressed by:
*formula 2.11*
There are two types of forces:
**surface forces**
- Pressure forces
- Viscous forces
- Gravity force
**Body forces**
- centrifugal force
- Coriolis force
- electromagnetic force

The surface forces are modelled here and the body forces are taken as a source term.

Followin drawing a free body diagram with all the forces that are resulted from the viscous stresses ($\taw$) and pressure, we can sum all the forces and after some algebra we would obtain:
*equation 2.13*

This is Armins dummy test