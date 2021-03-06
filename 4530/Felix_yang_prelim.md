  # Prelim 2019

Name:Felix Yang

This prelim is open book and open internet. You are not allowed to discuss the questions are related concepts with anyone while you are taking this prelim. You are not allowed to post questions on discussion boards. If you have questions, send an email to Monroe (monroews@gmail.com). If the question is relevant for the whole class he will post it as an issue on the course website.

For each question make sure to use units and to give variables names that are easily understood. Use print statements to **print the answers in a sentence** (except for the multiple choice!).

Name your file "yournamePrelim.md" (2 points for this!)
Send your file to the [course email](cee_4530@cornell.edu).

Each question is worth 7 points.

```python
from aguaclara.core.units import unit_registry as u
import aguaclara.research.environmental_processes_analysis as epa
import aguaclara.core.physchem as pc
import aguaclara.core.utility as ut
import numpy as np
import matplotlib.pyplot as plt
from scipy import stats
```

## Design a sand column experiment.
A sand column has an inner diameter of 1 inch and 20 cm total internal height. The sand porosity is 0.4 (40% of the column is filled with water, 60% is filled with sand). The sand density is $2650 kg/m^3$. The target approach velocity (the velocity of the water in the column if there were no sand) is 1 mm/s. The water is pumped with a peristaltic pump that delivers 2.8 mL per revolution.


1. What is the mass of sand (in grams) that must be added to the column?

 0.27 kilogram

2. What flow rate (in mL/s) is required?

 0.507 milliliter/second

3. What should the pump revolutions per minute be (in rev/min)? (Note that rev is a unit!)

10.86 turn/second

4. What is the hydraulic residence time of the water in the column (in seconds)?

80 seconds

```python
#put your code here! Remember to print your answer in a sentence.
Column_ID=1*u.inch
Column_Area=(u.pi*Column_ID**2)/4
Column_Area
Sand_Height=20*u.cm
Column_Volume=Column_Area*Sand_Height
Porosity=0.4
Volume_Water=Porosity*Column_Volume
Density=2650*u.kg/u.m**3
Velocity_Approach=1*u.mm/u.s
Q_per_rev=2.8*u.mL/u.revolution
Mass_sand=(Density*Column_Area*Sand_Height).to(u.kg)
print('The mass of sand that must be added to the column is '+str(Mass_sand))
Q_Column=(Velocity_Approach*Column_Area).to(u.mL/u.s)
print('The flow rate is '+str(Q_Column))
Pump_rev=(Q_Column/Q_per_rev).to(u.revolution/u.min)
print('The pump revolutions per minute is '+str(Pump_rev)) ##Turn is the same as revolution it seems
HRT=(Volume_Water/Q_Column).to(u.s) ##Only 40% of the space is filled with water and is taking all of the flow. If there were no sand, residence time should theoretically be higher. And if the sand were very porous (.8 porosity instead of .4, then there would be more space for water to occupy, increasing the volume of water and increasing HRT)
print('The HRT is '+str(HRT))
```

## Acid Neutralizing Capacity

A 50 mL water sample that contains some carbonates is titrated with 0.05 N HCl. The equivalent volume of the titrant was 2 mL.

5. What was the ANC of the sample (in meq/L)?

2 meq/L

```python
V_s=50*u.mL
N_t=.05*u.equivalent/u.L
V_e=2*u.mL
ANC=V_e*N_t/V_s
print('The ANC is '+str(ANC.to(u.mequivalent/u.L))) ##5
  ```



## Photometer calibration
The photometer that we use in lab measures absorbance using the following equation.

$$A = -log_{10} \frac{V_{Sample} - V_{Dark}}{V_{Blank} - V_{Dark}}$$

where $$log_{10}$$ is log base 10.

The relationship between concentration of a dissolved species and the absorbance will follow Beer's law.

$$ A = \epsilon b C $$

where $\epsilon$ is the extinction coefficient that is a property of the chemical species.

The optical path length for the photometer is 19 mm. The raw voltage data for dark voltage, blank voltage, standards, and unknown are given below.

6. Use [stats.linregress](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html) to obtain the best fit line for the calibration with absorbance as a function of concentration.
7. What is the slope, $\epsilon b$, for this data set? (Make sure to attach the correct units after doing the linear regression!)
8. What is $\epsilon$? Make sure to simplify the units to $length^2/mass$
9. Create a function in python that returns the concentration given a sample voltage. You can derive this equation from the two equations above.
10. Plot the calibration data AND the calibration line showing absorbance as a function of concentration (note that that ProCoDA shows this plot with the axis flipped). Make sure to label the axis and include a legend. And make sure that you have the same units on both plots!
11. What is the absorbance of the unknown?
12. What is the concentration of the unknown?

```python
#write the code to answer questions 6-12 here
Dark_Volts = -1.3065 * u.V
Blank_Volts = 3.49727 * u.V
Unknown_Volts = 0.1 * u.V
Sample_C = np.array([0, 10, 20, 30, 40, 50])* u.mg/u.L
Sample_Volts = np.array([3.497270,0.554016,-0.611595,-1.045119,-1.252709,-1.283894])* u.volts
b=19*u.mm
Sample_Volts
Dark_Volts
A=-np.log10((Sample_Volts-Dark_Volts)/(Blank_Volts-Dark_Volts))
A
slope, intercept, r_value, p_value, std_err = stats.linregress(Sample_C,A) ##6
intercept
slope = slope * 1/Sample_C.units
slope
fig, ax = plt.subplots()
# plot the data as red circles
ax.plot(Sample_C, A, 'ro', )

  #plot the linear regression as a black line
ax.plot(Sample_C, slope * Sample_C + intercept, 'k-', )

  # Add axis labels using the column labels from the dataframe
ax.set(xlabel='Concentration (mg/L)')
ax.set(ylabel='Absorbance')
ax.legend(['Measured', 'Linear regression'])
ax.grid(True)
  # Here I save the file to my local harddrive. You will need to change this to work on your computer.
  # We don't need the file type (png) here.

plt.show()#10
print('The slope is '+str(slope)) ##7
epsilon=slope/b
print('The epsilon is '+str(epsilon.to(u.m**2/u.kg))) ##8
def Concentration(V_Sample): ##9
  Absorbance=-np.log10((V_Sample-Dark_Volts)/(Blank_Volts-Dark_Volts))
  print('The absorbance is '+str(Absorbance))
  print('The concentration is '+str(Absorbance/slope))

Concentration(Unknown_Volts) ##11 and 12
```


## Multiple Choice

Use *asterisks* to italicize the answers that you select.

13. A peristaltic pump is pumping a red dye solution from a tank on the floor through a column filled with sand and activated carbon with flow down through the column. The pump is on the laboratory bench and the column is held by clamps to a stand that is on the bench. The tube that exits from the bottom of the sand column is elevated and discharges to the atmosphere (it drips into the sink) at an elevation that is higher than the tubing entering the top of the sand column. There are air bubbles entering the sand column. Which explanation(s) for the source of the air bubbles is (are) consistent with the observed results? Use what you've learned in fluid mechanics to help guide your analysis.

    A) Sand column fittings at the top of the column are leaking.

    B) Sand column fittings at the bottom of the column are leaking.

    C) Instant tube fitting (push to connect fitting) between the tank and the pump is leaking.

    D) Instant tube fitting between the pump and the sand column is leaking.

    **E) The tank of red dye is nearly empty and the pump is beginning to pull air into the end of the inlet tube.**

14. ProCoDA is reporting a concentration of 10 mg/L of red dye with a calibrated photometer when students are pumping reverse osmosis water through the photometer. What might be causing the high readings? Which of the following explanations is (are) consistent with the observed results?

     **A) An air bubble is caught in the optical path of the photometer**

     B) The photometer LED is turned off

     C) The photometer is installed backwards
