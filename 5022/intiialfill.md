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


Area_1105=9780*(u.ft**2)
Area_1104=6195*(u.ft**2)
Area_1103=3323*(u.ft**2)
Area_1102=1719*(u.ft**2)
Area_in_existing_wetland=(84+316+229)*(u.ft**2)
Area_in_existing_wetland
Wetland_Area=Area_1105-Area_in_existing_wetland
Wetland_Area.to(u.acres)
