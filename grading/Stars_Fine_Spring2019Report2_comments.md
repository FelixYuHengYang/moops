# StaRS FInE, Spring 2019
#### Lily Falk, Sam Hertle, and Whitney Denison
#### March 15, 2019

## Abstract

StaRS FInE is critically important **[a bit redundant no? I would just choose either critical or important]** because the subteam deals with one of the last steps in the AguaClara process - filtration **[Aren't all the steps important? Would consider the clause after "because" and go straight into the next sentence]**. The outtake pipes used in vertical filtration before considering StaRS FInE were problematic because over time they became clogged with chemical deposits. In order to clean the filters and wash away the deposits, clean water was emptied from the larger outlets to increase outflow velocity through the slots to dislodge the chemicals. In the process, clean water was wasted. StaRS FInE worked on a design that had the potential to combat this problem by ~~making use~~ **[using]** ~~of~~ a “Christmas tree” design. The design relied on larger openings to prevent clogs, as well as the gravity exclusion principle to prevent sand from exiting the outlet pipes. The focus of StaRS FInE in the spring of 2019 was to test the three dimensional model printed the previous semester with sand and find what velocity leads to failure in this model.

## Introduction

The spring of 2019 was StaRS FInE's second semester since the fall of 2015. The subteam was brought back in the fall of 2018 because of its continued relevance to AguaClara plants **[So third semester overall? Wording is a little confusing]**. The filter system [used then] became clogged throughout the day with chemical deposits **[which chemicals? PaCl?]** , ~~and~~ **[but]** there was no sustainable solution **[to the clogging]**. Chemical deposits built up on the small slots of the filters, and eventually the plant had to be temporarily shut off for clean water to be pulled through and disposed of **[Last part of this sentence is confusing. Is there a term for that specifically? I think in Honduras they called that purging but I may be wrong. If there isn't rephrase "pulled through"]**. Alternatively, buckets of acid could be poured into the filter to clean them, which was also not ideal. In both of these scenarios, the filter could not be used while it was cleaned, and there was unnecessary waste of clean water whether it was being used to purge the pipe or to divert water from the filters while they were being cleaned. The goal of StaRS FInE was to develop and test an outlet system that did not clog with chemical deposits and prevented sand from escaping. Past teams failed because of issues with sand getting into their outlet pipes during filtration. The past team did develop designs that worked during backwash, however the filtration velocity was too large for the parameters of their design and the water effluent contained a significant amount of sand. Because this problem occurred at the filtration outtake, the team was very conscious of head loss and the major and minor losses coming from the outlet pipe and the design geometry.

The goals of this semester were to test the apparatus **[,]** designed and 3D printed in the Fall 2018 **[,]** with sand, discover the failure velocity for this apparatus, and make changes to the spacing of the branches and angles if necessary. These changes were based on the some of the research of Horizontal Filtration (another AguaClara subteam), the results of [HorFi testing or testing done by past FInE teams?] testing, and the library of AguaClara fluid mechanics calculations. The team also had to discover the possible modes of failure. Failure modes may be caused by flow that is too fast, which may lead to sand moving up as a solid plug or small grains of sand getting into the outlet pipe. Fall 2018's design was promising, but before it was ready to be proposed as a solution **[,]** a lot more tests had to be run.

## Literature Review and Previous Work

The work of StaRS FInE has not been investigated outside of AguaClara **[,]** making the project exciting, ~~and~~ requiring innovation on the part of each team member. In the past **[,]** the team has found examples related to filters from aquaponics and various filtering methods. That being said, the alternate systems are more complicated, and would encounter the same issues that AguaClara filters already face. The StaRS FInE team members are the same this semester as last semester, however last semester the team worked mainly on research, ~~and~~ **[while/whereas]** this semester the project has shifted to fabrication.

Last semester the team encountered **["discovered" may be more fitting]** a few key insights. First, the team tested ~~at what~~ **[the]** angle **[at which]** sand falls in a pipe filled with water to determine an optimal angle where sand escaping the gravity exclusion zone is still likely to fall back down. The optimal angle was determined to be 26.64 degrees.  

A "Christmas tree" design was created in OnShape and 3D printed to fit inside of a 4-inch tube. Unlike previous teams dating back to 2015, the fall 2018 team ensured that the flow rate, velocity, and wing area of the apparatus all work together to prevent sand from exiting during backwash. This apparatus is still being used this semester as a main tool for research.

**[What are the other insights?? The last paragraph seems disconnected from the paragraph before it. What happened in the 2015 team?]**

## Methods

### Experimental Apparatus Design
#### Trial 1
The apparatus was designed in OnShape last semester, first including a 3D-printed horizontal filter, and then ~~the~~ **[a]** 4-Inch diameter PVC pipe that ~~will~~ **[would]** become the prototype for StaRS FInE testing of the gravity exclusion method for extraction. For more information on this ~~infrastructure~~ **[apparatus]**, reference the Fall 2018 Report. Below are the OnShape part studio, the OnShape drawings, and the photo of the newly fabricated apparatus. After assembling the apparatus, it was designed to have outlet holes in the filter and in the prototype that match tubing size for the outlet flow rate.

**[What is gravity exclusion method? This was not explained in the intro]**
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusOnshape.png" width= "350"> </p>
<p align="center">
  Figure 1. The OnShape Drawing of the prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/FIlterDrawing.png" width= "350"> </p>
<p align="center">
  Figure 2. The part studio design of the 3D printed filter.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusDrawing.png" width= "350"> </p>
<p align="center">
  Figure 3. The part studio design of the whole prototype.
</p>
<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/ApparatusReal.png" width= "500"> </p>
<p align="center">
  Figure 4. The apparatus setup with peristaltic pumps and tubing.
</p>

**[Any way to get these photos bigger? They are pretty but hard to see in the report. ]**

The experiments up to this point have tested the filter's ability to form sand exclusion zones. Monroe suggested that the team simulate real life AguaClara filter conditions as best as possible. Therefore, it was designed so that the inlet, below the filter would simulate filtration. **[What are sand exclusion zones?Explain either in previous work/introduction]**

The design also considered the rate at which injection and extraction would occur. Essentially, the respective injection and extraction rates were calculated based on backwash velocity and the respective design of the team's apparatus. This is calculated in the Python code in the [manual](#Manual) below. The values for the first trial were as follows:
| Injection Flow Rate     | Extraction Flow Rate
|---------------------------|-----------------------|
| 36.67 mL/s | 18.36 mL/s      |

**[What is injection flow? What is extraction flow? Is it just inlet and outlet?]**

In the first trial, the team allowed the injection flow to fill the tube to the top before the extraction pump was turned on. The extraction would pull water until the prototype was halfway drained and then the extraction would be turned off again. This would allow gravity to act as the flow from above the filter, as well as the injection as the flow below.

The last design consideration was converting between mL/s and RPM on the peristaltic pump that was connected to the inlet and outlet tubing. Using ProCoDa, the outlet and inlet flow in mL/s and the tubing sizes (16 for outlet and 18 for inlet), the team made new set points that converted into RPM values for the pump. More is detailed about the set points below in the [manual](#Manual).

**[Why was this a design consideration? Which unit is more desirable?]**

#### Trial 2
In the design of the second experimental apparatus, the team reconsidered the flow rates of injection and extraction. Understanding more about the application of the prototype to real Aguaclara Filters, the team calculated the following:

**[How did trial 2 resemble real AguaClara Filters more than trial 1?]**

| Injection Flow Rate | Extraction Flow Rate |
| ------------------- | -------------------- |
| 220.02 mL/s         | 36.67 mL/s           |

Again, more information about these number can be found in the Python code below in the [manual](#Manual).

The team used the same method of filling the prototype to the top before draining and turning off the extraction before the water level reached below the extraction tubes.

### Experimental Apparatus Fabrication
#### Trial 1
The current apparatus design was revisited. The team noted the small outlet pipe size and did the below calculation to determine that minimum pipe diameter was not met.

| Respective Flow Rate      | Minimum Tube Inner Diameter  
|---------------------------|-----------------------|
| 36.67 milliliter / second | 3.762 millimeter      |

<p align="center">
Reference manual below for Python code calculations of these values. </p>

**[After]** Shaving the glue from the previous tubes, the team detached the tubes. **[Glue was never mentioned before. You should clarify when and where it was used.]** Using the new calculated inner diameter, the team found tubing that ~~matched~~ met the minimum standard and considered ~~how it would affect~~ **[it's effect on]** the design of the 3D printed "pine-tree" filter which ~~was~~ already fit to the prototype PVC tube by **[drilled]** holes ~~drilled~~. In the OnShape drawing, the team determined that, if the filter was taken from the prototype, respective sized holes could be drilled with the drill press. The holes were designed to be offset from the original holes while still remaining in the bounds of the upper and lower wings. Holes were drilled to match these on the 4-Inch PVC prototype.

With three new outlet tubes of sufficient diameter glued water-tight, the team used two T-joint push-to-connect tubes to attach the outlet to a peristaltic pump of size 16 tubing. The inlet (lower cap) was tapped with push-to-connect that was attached to size 18 tubing in a peristaltic pump.

The team made the mistake of filling the apparatus with sand and then inverting so that exclusion zones were given no real chance to form.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/InvertedApparatus.png" width= "350"> </p>
<p align="center">
  Figure 5. The colored sand filling the exclusion zones as the apparatus was inverted.
</p>

**[Why was the sand colored?]**

#### Trial 2
In the second trial, the team drained the water and sand from the prototype. To better simulate plant conditions, Monroe suggested that the team first fill the prototype with water, and add sand from the top. This would create sand exclusion zones initially, that just needed to be maintained during water flow.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Water.JPG" width= "350"> </p>
<p align="center">
  Figure 6. Water filling the apparatus before the addition of sand.
</p>

Using newly calculated flow rates from the experimental design passage above, the apparatus was set up the same way as in the first trial, with detail in respect to the order of addition of sand and water. This also prevented the sand from entering the injection tubing because there was a constant water stream that made use of gravity exclusion. When the sand nearly filled the tube, the upper lid was secured and the extraction began.

### Feasibility of Design and Analysis
Before running the experiments, the team ensured that the prototype was watertight in order to collect accurate data regarding the flow rates of injection and extraction.

#### Trial 1

The initial mistake of inverting the apparatus was caused a limitation of the team's understanding of how the design would work in terms of water exclusion zone. The lower of the three triangular partitions was able to form the strongest exclusion zone, which was in fact pulling water without sand.

This trial gave the team an indication of how to move on, but should be noted that flow rates were not yet indicative of the Aguaclara filtration flow rates (of injection and extraction).

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Filter.jpg" width= "350"> </p>
<p align="center">
  Figure 7. The exclusion zone on the lower structure forming.
</p>

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial1Tubes.png" width= "350"> </p>
<p align="center">
  Figure 8. The extraction tubes pulling water without sand from the lower exclusion zone. Note the top tube was pulling sand from the most failed exclusion zone and the middle was pulling air.
</p>

#### Trial 2

The biggest issue with the second trial was that only the top tube pulled water out. This can be explained by a couple of possibilities. There was water leaking through the middle and bottom tubes, suggesting that they were not watertight and so they may have been pulling air only. The existence of air bubbles within the filter was also indication that there is flaw in the design.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Filter.JPG" width= "350"> </p>
<p align="center">
  Figure 9. The filter extraction zones during the second trial. Note the air bubbles in between the layers.
</p>

The top tube did not have any sand in it and the exclusion zones did exist, in a sense which is an essential insight moving forward. This means that at least one of the gravity exclusion zones formed and was capable of operating at the necessary velocity without failure. In agreement with the first trial, the lowest of the three "branches" was successfully pulling water.

<p align="center"> <img
src="https://raw.githubusercontent.com/AguaClara/StaRSFine/master/Images/Trial2Tubes.png" width= "450"> </p>
<p align="center">
  Figure 10. The extraction tubes during the second trial.
</p>

## Conclusions

Testing the apparatus with sand and water running at filtration speeds made the flaws in the apparatus used for experimentation clear, but not yet the problems with the "Christmas tree" design. The second trial showed that the top branch of the filter can handle high velocities of filtration without sand leaving in the outlet pipes, which is encouraging for predicting the success of this design.
## Future Work

Based on the two trials completed so far this semester, the most pressing goal was to have an experiment where water was pulled from all three tubes. Now that this has been achieved, the team could move forward to testing failure and finding the filtration velocity where sand begins to be pulled out with the water. If this velocity is reasonably high (i.e. much higher than any velocity expected in an AguaClara plant), the team will have a conversation about next steps necessary to implement the design in actual AguaClara plants. If the failure velocity is low or gravity exclusion zones don't form dependably, the team will need to try other designs. Variations of the design may include more or less branches, bigger spaces between branches, or potentially a new design entirely.

**[As someone who is not familiar with this subteam I had a really hard time understanding what the terms were, and why certain things were done. I think you guys can do a much better job at fleshing out the report, specifically at the introduction and previous work so that people who aren't as well versed can follow along better. I know that expanding it may seem self-evident, even redundant, to you but everything is neat and organized in your head, having connections between certain subjects that the audience, such as me, may not have. Overall I liked the report. Where the writing lacked, the diagrams helped me get a general idea of what was going on, but the writing could definitely improve.]**

# Manual
## ProCoDa

The ProCoDa used thus far in the semester has been limited to making sure the input and output peristaltic pumps are running at the correct velocity for their tube size. The team has not yet run an extended experiment regulated by ProCoDa.

For the peristaltic pump calculations, the states were as follows.

### States

#### OFF
The off state was used while the experiments were not run.

#### INJECT
The INJECT state used the set points *Just Water Flow* and *Water Tubing Size* to take into account the inlet flow rate in mL/s and the tubing size from inlet the peristaltic pump.

#### EXTRACT
The EXTRACT state used the set points *Outlet Flow* and *Outlet Tubing Size* to take into account the outlet flow rate in mL/s and the tubing size from the outlet peristaltic pump.

## Python Code
### Variables
$area$ : area of the sand bed

$areamm$ : area in mm

$backwashvelocity$ : velocity of water in the backwash stream

$filterflow$ : Minimum flow rate of the water

$headloss$ : Headloss

$temp$ : Temperature of operation

$\nu$ : Kinematic Viscosity of water based on temperature

$piperough$ : k, pipe roughness

$diamtube$ : tube diameter


```Python
import math
import numpy as np
import pandas as pd
from aguaclara.core.units import unit_registry as u
from aguaclara.core import pipes as pipe
from aguaclara.core import physchem as chem

area = 100*u.cm**2
#area of the filter bed for simulations
areamm = area.to(u.mm**2)
backwashvelocity = 11*u.mm/u.s
filterflow = (backwashvelocity*areamm*2)/6
#filterflow is the flow rate of water coming out of each filter
print(filterflow.to(u.ml/u.s))
injectionflow = filterflow*6
#injectionflow is the rate at which the water would come through the filter (all six layers that would be in an aguaclara plant)
print(injectionflow.to(u.ml/u.s))
extractionflow = filterflow*2
#extractionflow is the flow rate at which the team will extract water from the filter because water is coming from above and below the filter
print(extractionflow.to(u.ml/u.s))

headloss = 1*u.m
Length = 1*u.m
temp = 20*u.degC
Nu = chem.viscosity_kinematic(temp)
PipeRough = 0.1*u.mm
KMinor = 2
#to find the diameter of tube for the three tubes that will come out of our filter
diamtube = chem.diam_pipe((filterflow/3), headloss, Length, Nu, PipeRough, KMinor)
print(diamtube.to(u.mm)) #inner diameter of tube we would like to come out

```
## Onshape
Link to the full design:
https://cad.onshape.com/documents/2e536bd8940f20fc75058241/w/42817f17b88f823e779070ce/e/a78ef9a6ae52e13f92aed459?configuration=Angle%3D0.3839724354387525%2Bradian%3BList_NCIYbvAAUq0uK3%3DDefault%3BNumber%3D3.0%3BRadius%3D0.012700000000000001%2Bmeter%3BSpacing%3D0.01905%2Bmeter%3BThickness%3D0.0031750000000000003%2Bmeter%3Bdepth%3D0.10160000000000001%2Bmeter%3Blength%3D0.03429000000000001%2Bmeter
