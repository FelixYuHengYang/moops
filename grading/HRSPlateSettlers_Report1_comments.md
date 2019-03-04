# High Rate Sedimentation: Plate Settlers, Spring 2019
#### Leena Sen, Carmen Ortega, Luke Meyer
#### February 20th, 2019

## Abstract
Previous High Rate Sedimentation (HRS) teams have observed that the floc blanket is denser at the top ~~versus~~ [than] the bottom of the recirculator at higher upflow velocities. This inconsistency in the floc blanket led former subteams to take multiple calculated approaches in attempts to improve floc blanket longevity and increase overall reactor performance. The Spring 2019 team has worked to replace old tubing and clean the laboratory sedimentation tank. The team is also ~~in the process of~~ designing and incorporating plate settlers within the sedimentation tank to determine whether doing so will improve floc blanket longevity. In the future, the team will explore the effects of varied plate orientation at various upflow velocities.

## Introduction
Sedimentation is the process by which coagulated contaminant particles are removed from water via gravitational settling. In a sedimentation tank, water flows upward as flocs settle downward. Those flocs settle into a "floc blanket" at the bottom of the sedimentation tank. A floc blanket is a fluidized bed of suspended solids with a high rate of collisions. The particles in the floc blanket collide with coagulant particles and other flocs, coming together to form heavier flocs that settle to the basin of the recirculator. These heavier flocs remain in the reactor as part of the floc blanket. This process cleans the water, resulting in a lower effluent NTU (Nephelometric Turbidity Unit, a measure of clarity).

In the AguaClara lab sedimentation tank setup, a section of PVC piping known as the "tube settlers" simulates a life-size sedimentation tank's plate settlers. Multiple other tubing systems model the floc hopper and floc weir, as well as the inlet jet tube and influent and effluent lines that carry water in and out of the system. Since the behavior of a section of fluid is representative of the entire tank, tubing can be used to simulate a simple pathway in the reactor. This allows for a practical method of experimentation on a smaller scale. Refer to Figure 1 for a cross-sectional view of the sedimentation tank in an AguaClara plant to the sedimentation tank, and to Figure 2 for a visual representation of the model used by the HRS: Plate Settlers team.

![SedTank](https://github.com/CarmenOrtega/aguaclara_tutorial/blob/master/ACSedTank.PNG?raw=true)

Figure 1: Design schematic of the sedimentation tank in the AguaClara plants.  

![SedTankDiagram](https://github.com/CarmenOrtega/aguaclara_tutorial/blob/master/SedTankDiagram.PNG?raw=true)

Figure 2: Design schematic of experimental apparatus. Influent enters the sedimentation tank from the flocculator via inlet jet tubes of variable size. Downward direction of the influent flow is redirected upward by the semicircular jet reverser bottom geometry. Small percentage of the flow is insufficient to supply an additional tube settler and was sent to waste (Garland (2017)). [Great diagrams]


The HRS team aims to design a tank that will yield an effluent of no more than 0.3 NTU while maintaining high upflow velocity. Operating at a higher upflow velocity will allow for [processing] a greater volume of water ~~processing~~ in a given period of time, which will decrease plant operating costs. However, when operating at a high upflow velocity in lab, the floc blanket is unstable. The floc blanket is dense near the top of the recirculator, but very thin near the bottom. HRS: Plate Settlers plans to remediate this issue by incorporating a second set of plate settlers within the sedimentation tank itself. As more particles enter through the manifold, flocs at the top of the blanket overflow into the floc hopper or floc weir. The smallest particles which make it past the floc blanket and floc hopper then enter the plate settlers. Plate settlers catch the smallest particles by increasing the horizontal space where particles can settle out. Plate settler length and width determines capture velocity, the lowest velocity at which plates can catch particles. By increasing the number of plate settlers, and thereby the area in which the flocs can settle, HRS: Plate Settlers intends to increase the capture velocity and therefore achieve a more stabilized floc blanket. If successful, this will allow future teams to continue researching the potential viability of high upflow velocities in AguaClara plants.



## Literature Review and Previous Work
Several past researchers have studied the process of sedimentation and the properties floc blankets. Their research gives valuable insight to the Fall Spring 2019 High Rate Sedimentation AguaClara team.

Culp et al. (1968) researched different angles to find the optimal slope of the tube settlers. Using normal laboratory conditions, a 60 degree angle with respect to the horizontal provided continuous sludge removal while showing effective sedimentation performance. This gives the team a starting condition that can be held constant and assumed as beneficial for plate settler designs.

Furthermore, Hurst (2010) noted that the presence of the floc blanket enhanced the removal of particles. Their experiments found that upflow velocities of 1.0 to 1.3 mm/s produced the best performance. Past HRS teams have been successful at establishing floc blankets at higher velocities than the range given by Hurst, up to 15 mm/s, but those floc blankets were not stable.

Swetland (2014) discovered that as larger flocs formed in the sedimentation tank, those flocs would settle due to their high density relative to the fluid. Additionally, they discovered that in order for particle removal to occur, flocs need to have a higher settling velocity than the capture velocity. As the flocs concentrate and fall to the bottom of the sedimentation tank, a floc blanket forms. These findings informed the High Rate Sedimentation teams' understanding of floc formation.

In a similar vein, Balwan (2016) explored how the length of the tube settlers effected effluent turbidity. He found that increasing the length of tube settler increased the amount of particles removed by the reactor. With tube settlers at an angle of 45 degrees and 60 cm length, turbidity removal was measured to be 80 percent. However, his experiments only had three length variables (40cm, 50cm, 60cm) and the effluent of longer tube settlers were unknown. [How does this affect HRS:PS's knowledge on the topic and experiments to come?]

Hurst (2016) derived that rather than just increasing the upflow velocity to increase the creation of the floc blankets, alum dosage must also be considered. The turbidity and upflow velocity work in tandem to determine the stability of a suspended floc blanket. In the experiments described in Hurst (2016), upflow velocity was held constant at 1.2 mm/s, but coagulant doses (ranging from 1.0 to 7.5 mg/L) were varied in 10 nephelometric turbidity units, 100 NTU, and 500 NTU[Do you mean 10NTU intervals between 100 and 500?]. That being said, 15 mg/L of alum was found to be a suboptimal dose, as the blankets would break in higher conditions. Hurst concluded that by increasing the ratio of influent turbidity to the dose, one could use a lower dose while still having the same rate of particle removal. The 2019 Spring HRS Plate Settlers team has considered the velocity and dose together. Hurst recommends a range of 1.0 to 7.5 mg/L of alum, so the team will use those values in a predictive model of the plate settlers.

Garland (2017) observed how the characteristics of flocs that enter a sedimentation tank influence the performance of the tank. [What is the connection between the paper and the next sentence? Maybe start with "In the experiment, G,...."]Therefore, G, the velocity gradient, was increased in a range of 74–251 s^−1 while residence time, θ, was decreased. A constant Gθ of ~20,000 improved the particle removal. Because of this, a residence time of 24 s with a G of 251 s^−1 resulted in 14 NTU; however, after varying G to s^-1[I think you're missing a number before s^-1. Also you can use latex for units like so $s^-1$], the minimum turbidity was found to be 0.15 NTU. Garland concluded that velocity gradients greater than the existing specifications could be applied to reduce the flocculation time.

The Summer 2018 Team observed that at higher upflow velocities, the floc blanket was much more dense at the top of the recirculator than at the bottom. They proposed that the Fall 2018 team design a recycle line to allow for flocs at the top of the recirculator to flow back to the bottom and re-establish a more uniform distribution. The Fall 2018 Team responded to this observation via incorporation of a recycle line along the recirculator to improve floc blanket longevity. The installation of a recycle line resulted in decreased reactor performance, as the effluent turbidity resulted in a consistent ~30 NTU increase versus the baseline trial throughout the test. Furthermore, water tended to flow up both the recirculator and recycle line rather than down the recycle line to oppose the movement of water along the recirculator. The Fall 2018 team decided that future work might involve incorporating a peristaltic pump along the recycle line to ensure proper direction of water flow for proof of concept. Currently, Flow Recycle has been placed on standby as HRS: Plate Settlers develops plates to incorporate into the sedimentation tank to achieve a similar initial goal as Flow Recycle. Thus, HRS: Plate Settlers is an extension of Flow Recycle. Therefore it is imperative that the subteam considers density of the blanket as a function of the plate geometry. [These last few sentences are a bit clunky]


## Bibliography
Balwan, K. (2016). Study of the effect of length and inclination of tube settler on the effluent quality. Journal (International Journal of Innovative Research and Advanced Engineering).

Culp, G., Hansen, S., & Richardson, G. (1968). High-Rate Sedimentation in Water Treatment Works. Journal (American Water Works Association), 60(6), 681-698. http://www.jstor.org/stable/41265352

Galantino, C., Oritz, A., & Zarecor, M. (2017). High Rate Sedimentation Fall 2017 Report.

Garland, C., Weber-Shirk, M., & Lion, L. W. (2016). Revisiting Hydraulic Flocculator Design for Use in Water Treatment Systems with Fluidized Floc Beds. Environmental Engineering Science, 34(2), 122–129. https://doi.org/10.1089/ees.2016.0174


Hong, A., Si, H. (2018). High Rate Sedimentation Summer 2018 Report.

Hurst, M. W. (2010). Evaluation of parameters affecting steady-state floc blanket performance. http://hdl.handle.net/1813/14755

Hurst M., Weber-Shirk M., & Lion L. W. (2017). Influence of Alum Coagulant Dose and Influence Turbidity on Floc Blanket Growth Rate, Steady-State Suspended Solids Concentration, and Turbidity Removal. Journal of Environmental Engineering, 143(2), 04016081. https://doi.org/10.1061

Swetland, K., Weber-Shirk, M., Lion, L. (2014). Flocculation-sedimentation performance model for laminar flow hydraulic flocculation with polyaluminum chloride and aluminum sulfate coagulants. Journal (Journal of Environmental Engineering).

Zarecor, M., Sharma, S., Conneely, J. (2018). High Rate Sedimentation Spring 2018 Report.

Sen, L., Conneely, J. (2018). High Rate Sedimentation Fall 2018 Report.
