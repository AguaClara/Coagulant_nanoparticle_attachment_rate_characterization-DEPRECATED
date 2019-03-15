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
uavg=TubeFlow/(np.pi*R*R)
vm=2*uavg
def laminarvelocity(r,R,v):
    laminarvelocity = v*(1-((r**2)/(R**2)))
    return laminarvelocity
    print(laminarvelocity)
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
FlocSegL=(9*u.foot+9*u.inch).to(u.m)
TotalResTime=(2.4*u.min).to(u.hr)
SegResTime=TotalResTime/4

```