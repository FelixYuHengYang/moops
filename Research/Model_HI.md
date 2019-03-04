```python
from aguaclara.core.units  import unit_registry as u
u.define('equivalent = mole = eq')
import aguaclara.research.environmental_processes_analysis as epa
from scipy import optimize
from aide_design.play import*
from aide_design.physchem import*
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
from scipy import stats
from scipy.interpolate import make_interp_spline, BSpline
from math import*

Temp=20*u.degC
V=10*u.mL
C_init_glyphosate=.240*u.g/u.L
C_init_S_metolachlore=.193*u.g/u.L
Amt_mulch_residence=758*u.g/u.m**2
ID_Column=15.4*u.cm
Ratio_Mass_Water_Mass_mulch=1*u.g/u.g

A_Column=(ID_Column**2*u.pi/4).to(u.m**2)
Mass_Mulch=(Amt_mulch_residence*A_Column).to(u.g)
M_init_glyphosate=(C_init_glyphosate*V).to(u.mg)
M_init_S_metolachlore=(C_init_S_metolachlore*V).to(u.mg)
Volume_Water_Mulch=14*u.cm**3
Concentration_glyphosate_mulch=M_init_glyphosate/Volume_Water_Mulch
Concentration_S_metolachlore_mulch=M_init_S_metolachlore/Volume_Water_Mulch
Concentration_glyphosate_mulch.to(u.mg/u.L)
Concentration_S_metolachlore_mulch.to(u.mg/u.L)

C_out_glyphosate=M_init_glyphosate*u.g/(1000*u.mg*A_Column)
C_out_S_metolachlore=M_init_S_metolachlore*u.g/(1000*u.mg*A_Column)
C_out_glyphosate
C_out_glyphosate_per_Liter=(C_out_glyphosate/(8*u.mm)).to(u.g/u.L)
C_out_glyphosate_per_Liter
C_out_S_metolachlore
x C_out_S_metolachlore_per_Liter=(C_out_S_metolachlore/(8*u.mm)).to(u.g/u.L)
C_out_S_metolachlore_per_Liter
```
