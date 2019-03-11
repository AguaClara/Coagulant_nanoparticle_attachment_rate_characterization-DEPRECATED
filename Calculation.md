```python
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import physchem as pc
import numpy as np
R=((0.17/2)*u.inch).to(u.m)
mu=pc.viscosity_dynamic(293*u.degK)
SedTank_Flow=2*u.mm/u.second
WaterPumpRPM=76*u.revolution/u.minute
Size16TubingFlow=0.8*u.mL/u.revolution
TubeFlow=(WaterPumpRPM*Size16TubingFlow).to(u.m**3/u.s)
um=TubeFlow/(np.pi*R*R)
PressureGradient=(8*mu*(0.5*um)/(R*R))
vm=(1/(4*mu))*PressureGradient*R*R

def laminarvelocity(r,R,v):
    laminarvelocity = v*(1-((r**2)/(R**2)))
    return laminarvelocity
    print(laminarvelocity)

testr=(0.084*u.inch).to(u.m)

laminarvelocity(testr,R,vm)

```

```python
Diam=2*R
nu=pc.viscosity_kinematic(293*u.degK)
Re=pc.re_pipe(TubeFlow, Diam, nu)
CD=24/Re
rho=pc.density_water(293*u.degK)
rcoagulant=(90/2)*u.nm
veloncoag=laminarvelocity((R-rcoagulant),R,vm)
Fdrag=-(CD*np.pi*(rcoagulant**2)*rho*(veloncoag**2)/2).to_base_units()
Fdrag

```

```python
g=9.8*u.m/(u.s**2)
coagheadloss=(-Fdrag/(np.pi*R*R*rho*g)).to(u.centimeter)
coagheadloss
```
Used headloss data at 20NTU measured by Fall 2018.
```python
HLavg0=1.420*u.cm/u.hr
HLavg1=0.736*u.cm/u.hr
HLavg2=0.389*u.cm/u.hr
HLavg3=0.264*u.cm/u.hr

npwall0=HLavg0/coagheadloss
npwall1=HLavg1/coagheadloss
npwall2=HLavg2/coagheadloss
npwall3=HLavg3/coagheadloss
```

```python
from aide_design.play import*
import math as m

#Inputs
Q_reactor=(4/3) *(u.mL/u.s) # flow rate of the system
Gtheta_goal=20000 #target G*theta to design flocculator to
Diam_floctube=(0.17)*(u.inch)
R_c=5*u.cm #radius of curvature (the radius of the tube the flocculator is wrapped around)
Re_pipetransition=2100
v=(1*10**-6)*(u.m**2/u.s)
e_pvc=0.12*u.mm #roughness of PVC Re_pipetransition

#Calculations
Re_f= ((4*Q_reactor)/(np.pi*Diam_floctube*v)).to(u.dimensionless)


print(Re_f)


#def fric_function(Q_reactor,Diam_floctube,v,e_pvc)
if Re_f > Re_pipetransition:
  print('Re_f is greater than Re_pipetransition')
  fric=0.25/((m.log((e_pvc/3.7*Diam_floctube)+(5.74/(Re_f**0.9))))**2)
else:
  fric=64/(Re_f)
  print('Re_f is not greater than Re_pipetransition')
  print(fric)
L=1
h_f=fric*(8/(pc.gravity*np.pi**2))*((L*Q_reactor**2)/(Diam_floctube**5))



R=R_c.to(u.inch)

De=(((Diam_floctube/R)**2)*Re_f)
print(De)

friction_ratio=1+(0.33*m.log(De)**4)
print(friction_ratio)

h_friction=h_f*friction_ratio
Area=(np.pi/4)*Diam_floctube**2
theta=(Area*L)/Q_reactor

ED_floc=(h_friction*pc.gravity)/theta

epsilon=ED_floc.to(u.mW/u.kg)
print('Energy dissipation rate is',epsilon)

G_floc=((epsilon/v)**(1/2)).to(u.second**-1)
print(G_floc)

theta_goal=(Gtheta_goal/G_floc).to(u.minute)
print(theta_goal)

L_goal=theta_goal*(Q_reactor/Area)

L_floc=L_goal
print('The length of flocculator tubing should be', L_floc.to(u.ft))
```

```python
FlocculatorL=(42*u.foot).to(u.cm)
FlocSegL=FlocculatorL/4
TotalResTime=(theta_goal).to(u.hr)
SegResTime=TotalResTime/4

```
