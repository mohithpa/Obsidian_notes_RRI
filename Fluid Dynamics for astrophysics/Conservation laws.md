#main
There are mainly 3 conservation laws:
1. Mass conservation 
2. Momentum conservation 
3. Energy Conservation

## Mass Conservation gives us the continuity equation
Mass defined as the amount of mass flowing in or out (say in grams) of a given surface;
- Mass flux is given in units $g cm^{-2}s^{-1}$ ==(mass per area per sec)==
- ==Mass flux is== = $\rho u$ => $gcm^{-3} cm.s^{-1}$ => $g cm^{-2}s^{-1}$

Envisage a surface and now mass can either be going in or coming out 

![[Pasted image 20220316123618.png]]  

The mass contained in the volume can neither be created nor be destroyed , the $\int \rho dV$ can only change due to mass flux.
	
![[Pasted image 20220316124419.png]]

Therefore time rate of change of total mass is gives as;
$$\dfrac{\partial}{dt} \int \rho dV = -\int \rho \overrightarrow{u}.\overrightarrow {dS} $$ Applying gauss divergence theorem [[Fundamental Theorems]] on RHS
$$\dfrac{\partial}{dt} \int \rho dV - \int \nabla.(\rho \overrightarrow{u}){dV} $$
$$\int (\dfrac{\partial{\rho}}{dt}   - \nabla.(\rho \overrightarrow{u}\ ))\ {dV} = 0$$
This is in eulerian form 

**In general the conservative form of any quantity goes as ==Partial derivative of that quantity is + divergence of flux of that quatity==**      

Alternatively, using Lagrangian derivative 
$$\dfrac{d\rho}{dt} + \rho \nabla.u =0$$
or,                                                  $$\dfrac{1}{\rho}\dfrac{d\rho}{dt} +  \nabla.u =0$$ often the first term is approximated to 0

$\dfrac{1}{\rho}\dfrac{d\rho}{dt} \approx0$

therefore, $\nabla.u = 0$ => this is the condition for incompressibily ;
- in reality ther is no perfectly incompressible fluid and the above equation are applicable only for flow speed << sound speed 

## Momentum Conservation
- Note: The momnentum conservation is for the entire fluid parcel
* Momentum conservation is essentially the Newton's 2nd law of motion i.e
$\overrightarrow{F}= m \overrightarrow{a}$   or $\overrightarrow{F}= m\dfrac {d\overrightarrow{V}}{dt}$
- The Force is on the LHS and the rate of change of momentum is on the RHS. 

### The rate of rate of change of momentum(RHS) of the fluid parcel can be due to two reasons
1. internal inherent/intrensic change of momentum flux wrt to time in the given volume V.
$\int\dfrac{\partial{(\rho u )}}{\partial{t}}dV$
2. due to the momentum flux leaking out or seeping in through surface.
$\int {(\rho u) u.}dA$ = $\int \nabla.(\rho u u)dV$ by using GDT([[Fundamental Theorems]])

#### The LHS is due to 2 forces that is body forces and surface forces 
1. Body forces : body forces also have volume component => $\int \rho \overrightarrow{g}dV$ 
$\overrightarrow{g}$  is the proxy for any force example accleration due to gravity
2. surface forces are basically normal(Pressre) or tangential(Stress) and both of these are considered under one unbrella.
- Check this video out https://www.youtube.com/watch?v=uO_bW2zzrNU
this video describes the stress tensor
![[Pasted image 20220317151620.png]]
$$d\overrightarrow{F}_{i}=-P_{ij}A_j$$ $$dF_{surface} = -\int P_{ij}dA_j  $$
By GDT [[Fundamental Theorems]] for tensors;
$$= -\int \frac{\partial{P_{ij}}}{\partial{A_j}}dV $$
$$=-\int (\nabla.\overrightarrow{P} ) dV$$
Now the equation F = ma becomes
LHS ,$$\int \rho \overrightarrow{g}\ dV-\int \rho d\overrightarrow{a}= \int \rho \overrightarrow{g}\ dV-\int (\nabla.\overrightarrow{P} ) dV $$

$$=\int (\rho \overrightarrow{g}\ - (\nabla.\overrightarrow{P} ))\ dV$$
RHS ;
$$\int\dfrac{\partial{(\rho u )}}{\partial{t}}dV +  \int \nabla.(\rho u u)dV = \int(\dfrac{\partial{(\rho u )}}{\partial{t}} + \nabla.(\rho u u))\ dV$$
therefore LHS = RHS or;
$$\int (\rho \overrightarrow{g}\ - (\nabla.\overrightarrow{P} ))\ dV = \int(\dfrac{\partial{(\rho u )}}{\partial{t}} + \nabla.(\rho u u))\ dV$$
=> $$\dfrac{\partial{(\rho u )}}{\partial{t}} + \nabla.(\rho u u)\ = \rho \overrightarrow{g}\ - \nabla.\overrightarrow{P}   ----(1)$$
Now to get the conservative form of the equation; 
say the body forces are 0;
$$\dfrac{\partial{(\rho u )}}{\partial{t}} + \nabla.(\rho u u +\overrightarrow{P}) = 0 $$
from eqn 1
$$\rho\dfrac{\partial{( u )}}{\partial{t}} +u\dfrac{\partial{( \rho )}}{\partial{t}} + \nabla.(\rho u) u + \rho(u.\nabla)u = \rho \overrightarrow{g}\ - \nabla.\overrightarrow{P}$$
but wkt mass continuity eqn in $$\dfrac{\partial{\rho}}{dt}   - \nabla.(\rho \overrightarrow{u}\ ) = 0 ----(2)$$
put (2) in (1)
$$\rho\dfrac{\partial{( u )}}{\partial{t}}  + \rho(u.\nabla)u = \rho \overrightarrow{g}\ - \nabla.\overrightarrow{P}$$
Consider an [[invisscid fluid]],
for an [[inviscid fluid]] $P_{ij} = p \ \delta{ij}$ ;

Therefore;
$$\rho\dfrac{\partial{( u )}}{\partial{t}}  + \rho(u.\nabla)u = \rho \overrightarrow{g}\ - \nabla p$$
This  equation is called the Euler Lagrange equation