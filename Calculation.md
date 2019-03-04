```python
import pandas as pd
import numpy as np
from aguaclara.core.units import unit_registry as u
from aguaclara.core import physchem as pc
import numpy as np
R=((1/16)*u.inch).to(u.m)
mu=pc.viscosity_dynamic(293)
SedTube_Flow=2*u.mm/u.second
WaterPumpRPM=76*u.revolution/u.minute
Size16TubingFlow=0.8*u.mL/u.revolution
TubeFlow=(WaterPumpRPM*Size16TubingFlow).to(u.m**3/u.s)
um=TubeFlow/(np.pi*R*R)
PressureGradient=8*mu*(0.5*um)/(R*R)
vm=(1/(4*mu))*PressureGradient*R*R

def laminarvelocity(r):
    r=r*u.inch
    R=((1/16)*u.inch)
    laminarvelocity=vm*(1-((r*r)/(R*R)))
    print(laminarvelocity)

laminarvelocity((1/16))
```
