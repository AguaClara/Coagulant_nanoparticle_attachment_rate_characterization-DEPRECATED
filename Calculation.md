```python
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import physchem as pc
import numpy as np
R=((1/16)*u.inch).to(u.m)
nu=pc.viscosity_dynamic(293)
SedTank_Flow=2*u.mm/u.second
WaterPumpRPM=76*u.revolution/u.minute
Size16TubingFlow=0.8*u.mL/u.revolution
TubeFlow=(WaterPumpRPM*Size16TubingFlow).to(u.m**3/u.s)
um=TubeFlow/(np.pi*R*R)
PressureGradient=(8*nu*(0.5*um)/(R*R))
vm=(1/(4*nu))*PressureGradient*R*R

def laminarvelocity(r):
    r=r*u.inch
    R=((1/16)*u.inch)
    laminarvelocity=vm*(1-((r*r)/(R*R)))

laminarvelocity((1/16))
```

```python
Diam=2*R
mu=pc.viscosity_kinematic(293)
Re=pc.re_pipe(TubeFlow, Diam, mu)
CD=24/Re
rho=pc.density_water(293)
rcoagulant=(90*u.nm).to(u.inch)
rcoagcalc=(R.to(u.inch)-rcoagulant)/(1*u.inch)
veloncoag=laminarvelocity(rcoagcalc)
Fdrag=CD*np.pi*rcoagulant*rcoagulant*rho*veloncoag*veloncoag/2
```

```python
g=9.8*u.m/(u.s**2)
Fdrag
coagheadloss=-Fdrag/(np.pi*R*R*rho*g)
coagheadloss
```
