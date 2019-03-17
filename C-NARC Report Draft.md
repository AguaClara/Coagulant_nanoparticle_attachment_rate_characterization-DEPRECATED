#Coagulant-Nanoparticle Attachment Rate Characterization, Spring 2019
#### Ada Lian, Valentine Starnes, Yeonjin Yun
#### March 15, 2019



## Abstract
The Spring 2019 Coagulant-Nanoparticle Attachment Rate Characterization (C-NARC) team’s objective was to continue the previous team’s work in determining the rate of coagulant nanoparticle attachment, specifically the rate constant of that relationship, which the team hypothesized to be first order. In order to determine the rate at which nanoparticles are adhering to the flocculator wall the team utilized the data the previous team collected. This will in turn determine the rate at which the nanoparticles are attaching to clay. Through determining the rate the nanoparticles attach to clay, the team gains a better understanding of how the coagulant nanoparticles behave during flocculation.

## Introduction
The fundamental goal of AguaClara plants is to develop resilient, gravity-powered drinking water and wastewater treatment technologies that will provide clean and safe drinking water to 2 billion people who currently do not have access to it. The main challenges to achieve this goal are financial, technological and political barriers. In regard to the technological barrier, the goal of C-NARC’s team for Spring 2019 is to reduce the excess coagulant that does not adhere to the particles of influent. Coagulant is one of the most expensive parts of the water treatment process in AguaClara plants and if there is dissipation, a higher dosage of coagulant to compensate the loss could be required. The underlying problem is that the attachment process between coagulant and nanoparticles in influent is unknown. Without this information, reducing the amount of headloss to the flocculator walls by changing certain variables becomes a challenge. To solve this problem, C-NARC team will quantify the rate of attachment between coagulant, the walls and the clay particles. The team hypothesizes that the headloss accumulation in the flocculator is first order with respect to distance along the flocculator. The rate constant from the first order relationship will be calculated utilizing experimental data obtained by Fall 2018 team. Once this relationship is established, AguaClara plants will be able to alter the variables depending on the specific situation, whether it is at low turbidity or at low flow rate.

## Literature Review
####Coagulation and Flocculation
In untreated water, there are numerous inorganic and organic particles that are too small to be removed by a filter. Therefore, coagulation and flocculation are important steps in the water treatment process to aid the removal of those particles. AguaClara plants use polyaluminium chloride (PACl), which is a coagulant that precipitates in water to create sticky nanoparticles [(Gebbie, 2006)](http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf). During flocculation, the fluid deformation caused by baffles–or coiled tubing in the lab setting–induces collisions between the coagulant nanoparticles and inorganic/organic particles in the untreated water. Those collisions form flocs, which are easier to remove later during the sedimentation process [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Flocculation/Floc_Intro.html). The issue, however, is that the nanoparticles are not only sticking to particles but also attaching to the flocculator wall or remaining in suspension. Using that information, the team will be able to find the rate at which coagulant nanoparticles attach to the three locations.

####Headloss
As stated earlier, the attachment of nanoparticles to the flocculator wall is an issue because it increases the headloss along the flocculator. Headloss is defined as the loss of energy of a fluid as it flows through space, which is mainly caused by the friction between the fluid and the inside of the tubing [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Review/Review_Fluid_Mechanics.html#headloss). The Darcy-Weisbach equation (as shown below) explains the major losses.

$$ h_{f} = f\frac{L}{D}\frac{\overline{v}^2}{2g} = f\frac{8}{g\pi^2}\frac{LQ^2}{D^5} $$
Such that,
$$\small {h_{f}=major\:loss, \\
f=Darcy\:friction\:factor,\\
L=pipe\:length,\\
Q=pipe\:flow\:rate,\\
D=pipe\:diameter}
$$


This equation also provides the technical reasoning behind the negative effect of coagulant buildup on the flocculator walls. As there is more coagulant nanoparticles sticking to the wall, the diameter of the tubing decreases. ![Headloss_Diagram](/Images/Headloss_Diagram.png)
Figure 1: Coagulant buildup leds to a decrease in diameter, which causes an increase in headloss along the flocculator [(Sausele & Shah, 2018)](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20final%20report.pdf).
The relationship between headloss and the tube diameter is inversely proportional. In other words, as the tube diameter decreases due to coagulant sticking to the wall, the headloss increases. The amount of headloss, in other words, is proportional to the number of coagulant nanoparticles that are sticking to the wall. As more coagulant nanoparticles are attached to the wall, there is more force pulling the water against the water flow, which in turn increases the headloss. Using that relationship and the headloss data from last semester, we will be able to find the number of nanoparticles sticking to the wall in each of the four sections of the flocculator.
####Drag Force
As mentioned above, headloss is mainly caused by the friction between the surface and the fluid, therefore, headloss is also caused by the friction between the surface of the coagulant nanoparticles stuck to the flocculator wall. By determining the drag force, the team can also determine the headloss caused by one coagulant nanoparticle. The nanoparticle is extremely small, therefore the team assumed that the shape is a sphere. The drag force of a sphere is shown as
$$F_{D}=0.5C_{d}\rho v^2A_{p}$$
where
$$\small
{F_{D}=Drag\: Force, \rho=fluid\:density,v=velocity,\\A_{p}=reference\:area\:and\:C_{d}=drag\:coefficient }$$
Before calculating the drag force, there are a few unknowns we would have to determine. The drag coefficient is calculated using Stokes law.
$$ C_{d} = \frac{24}{Re}$$
$$Re=\frac{\rho v D}{\mu} $$
$$\small
{\rho=fluid\:density,v=average\:velocity\:in\:the\:pipe,\\D=diameter\:of\:the\:pipe\:and\:\mu=dynamic\:viscosity\:of\:the\:fluid}$$
The velocity can be calculated by the fact that the water flow is laminar due to the small diameter of the tubing.

![Velocity_Profile](/Images/Velocity_Profile.png)
Figure 2: Velocity Profile of laminar flow. [("Velocity Profile for Tube Flow",n.d.)](http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html)

##Previous Work
Previous research from the Fall 2018 C-NARC team focused on determining the rate at which free coagulant attached to the flocculator wall. The team connected four pressure sensors along the coiled flocculator at equal distances to observe the rate of headloss accumulation in each section. The results showed that the rate of headloss accumulation decreased along the length of the flocculator (ref). These results reflected that the coagulant had attached either to clay or to the first sections of the wall. Additionally, the relationship between clay concentrations and rate of headloss accumulation was unclear. The first section of the flocculator showed a direct relationship between turbidity and head loss accumulation in which a decrease in clay concentration resulted in a decrease in headloss accumulation. Conversely, the second and third section showed an inverse relationship between turbidity and rate of headloss accumulation while the fourth section showed no relationship [(Sausele & Shah, 2018)](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20final%20report.pdf). It was hypothesized that the inverse relationship occurred because as turbidity decreased, the amount of clay for coagulant to attach to decreased, thus there were more free coagulant nanoparticles to attach to the flocculator walls. It is unknown why in the first section a decrease in turbidity resulted in less headloss accumulation. This result may suggest that a clay-coagulant mixture was sticking to the flocculator walls as well as free coagulant particles.

The C-NARC team aims to measure the first order rate constant for the loss of coagulant to flocculator walls as well as the first order rate constant for the loss of coagulant to clay surfaces. In order to find the amount of coagulant nanoparticles on the flocculator walls, the team will first find the velocity at the center of one coagulant particle on the wall, then find the drag force and head loss accordingly. These calculations will be compared to last semester’s headloss accumulation results to estimate the total number of coagulant nanoparticles on the walls. Furthermore, the team will calculate the amount of coagulant left in suspension and attached to the clay as a function of position. Experiments will be conducted to verify these calculations and will be repeated at varying velocities and turbidity levels.

## Methods
Before performing any experiments, the C-NARC team used Python to carry out theoretical calculations. The overall goal of these calculations was to find the total number of coagulant particles on the wall of the tubing. Shown below is a list of constants used for the calculations.

| Constant |  Definition   | Value |
|:------- |:--------:|:-----:|
| R     | Distance from center of tubing to tube wall |$0.085 in$ |
| $\mu$ (mu)    | Dynamic viscosity| $0.001005 \frac {kg}{m/s}$|
| RPM  | Water Pump rate per minute| $76 \frac{rev}{min}$ |
| $\nu$ (nu) | Kinematic Viscosity | $0.001005 \frac{kg}{ms}$|
| $\rho$ | Density of water | $998.2 \frac{kg}{m^3}$|
| g| Gravitational constant | $9.8 \frac {m}{s^2}$ |
| r| Distance from the center of the nanoparticle to the middle to the tube| $0.002134 m$|
| $V_{f}$| Volumetric Flow in size 16 tubing per revolution | $0.8 \frac{mL}{rev}$ |
The initial goal was to calculate the velocity at the center of one coagulant nanoparticle on the wall of the tubing. The first step towards this was to find the flow of the solution through the tubing. The water pump was set to turn 76 revolutions per minute and peristaltic pump tubing size 16 allows 0.8 mL of solution per revolution. The formula for the tube flow is given below:
$$ Tube Flow = RPM * V_{f}$$

Therefore, the tube flow represents the amount of solution per time that has flowed through the tube. The mean velocity is then calculated from the tube flow divided by the cross sectional area of the tubing.
 $$u_{m} = \frac{TubeFlow}{\pi R²}$$

<!-- Next, given that μ is the dynamic viscosity, the pressure gradient is found by the following formula:$$ \frac{ΔP}{ΔX} = \frac {8μU_{m}}{R²} $$ -->
<!-- This pressure gradient represents how the pressure will vary within the tubing due to viscosity, velocity and radius. -->
This mean velocity represents the average velocity of one coagulant nanoparticle flowing through the tube. Finally, the maximum velocity in fully developed velocity profile is given by the following formula:
$$ v_{m} = 2u_{m} $$

This shows the maximum velocity of a coagulant nanoparticle which would be in the middle of the tube due to the least amount of drag or shear force. This maximum velocity is then used to find the velocity at the center of one coagulant nanoparticle on the wall of the tubing which was calculated by the following formula:
$$ V(r) = v_{m}[1- \frac{r^2}{R^2}]$$
Since the radius of the coagulant nanoparticle is $0.45nm$ and the radius of the tube is $0.002159m$, the value of “r” is the difference between these which is $0.002158955m$. Given this radius, the velocity of one particle was calculated to be $5.7692×10^-6$ $m/s$.

The next step was to find the drag force on one coagulant nanoparticle on the tubing. First, the drag coefficient is given by:
 $$ Cd = \frac{24}{Re}$$
where the Reynolds number is $$ Re = \frac{pvD}{μ}$$
 and p is the density, v is the velocity, D is the diameter of the tubing and μ is the dynamic viscosity. Then, the drag force is calculated by:
$$ F_{d} = \frac {1}{2} C_{d} A pv^2$$
Given a velocity of $5.769×10^{-6} m/s$, the calculated drag force was $-8.55*10^{-24}$ $\frac{kg*m}{s^2}$. The next step was to find the headloss from one coagulant nanoparticle on the tubing. The headloss was given by the formula:
$$ H_{L} = \frac{-F_{d}}{\pi R²pg}
$$
The head loss was calculated as $5.968×10^{-21} cm$. This was compared to last semester’s results from 20 NTU. We picked the lowest NTU available because at a lower NTU, more coagulant will attach to the wall of the tubing due to less clay particles in the solution. In order to calculate the number of coagulant particles attached to the walls of the tubing, the average headloss at each pressure sensor was divided by the headloss of one coagulant particle.
$$	Nanoparticles\:on\:wall = \frac {H_{L,avg}\:at\:one\:sensor}{H_{L}\:from\:1 \:coagulant}$$

This equation shows the number of nanoparticles from each section of the flocculator. The total number of nanoparticles attached to the whole flocculator tubing would be the sum of each total at the four pressure sensors. The total number of coagulant nanoparticles on the whole flocculator was $4.71 * 10^{20} \frac{particles}{hour}$.




### Experimental Apparatus
The Fall 2018 team conducted experiments with four different iterations of the experimental design. The three initial iterations were modified and improved upon before arriving at the current version.

The experimental setup, shown in Figure 3 and Figure 4, included the following: three pumps to introduce water, clay, and coagulant to the system; a flow accumulator; an influent turbidimeter;  a modified coiled flocculator; and an air pump for cleaning the system between each experimental trial. See the manual for more information on the setup.

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

Figure 3: Experimental setup showing the flow of water, coagulant, and clay. Included in the experimental setup was the coiled flocculator with four attached pressure sensors.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/exptsetup2.jpg?raw=true" >

Figure 4: Image of the bench setup, including the modified coiled flocculator.
</div>

The experiment setup shown models the water flow through a plant on a smaller, lab-sized scale as follows:
1. The blue influent line delivers water to the water pump.
2. A concentration of clay stock is prepared and introduced into the water.
3. The pumps deliver the water and clay mixture to the turbidimeter.
4. The turbidimeter measures the influent turbidity of the clay-water mixture.
5. The coagulant is added immediately before the clay-water mixture enters the coiled flocculator. The flocculator allows for collisions between clay particles and coagulant nanoparticles.
6. The flocculator has four pressure sensors attached at equal distances by push-to-connect fittings to measure the pressure differences across the length of the flocculator.
7. The red effluent line transports wastewater out of the system.

Water was introduced into the system through the influent line. The flow rate of the water was maintained at a constant 1 mL/sec by the water pump. This flow rate was determined arbitrarily. The water was then pumped into the inlet of flow accumulator, which is a reservoir that allows a continuous flow of water  through the system by reducing fluctuations caused by the pump. It consisted of a bottle with two taps: one for the entry of water and the other for the exit. At the beginning of an experiment, the bottle was filled with water up to just above the two holes. The bottle was then capped to trap the air inside and pressurize itself, thus maintaining the water level at a steady state [(Tsang et. al., 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md). The water then flowed out of the flow accumulator, after which clay was pumped into the water.
A stock solution of clay was prepared, and the concentration at which it was introduced into the water by the clay pump was determined by the turbidity, measured by the influent turbidimeter.  The speed of the clay pump was varied by the Proportional - Integral - Derivative (PID) control to reach the target turbidity.  

A stock solution of PACl coagulant with the concentration of 0.1418g/L was prepared. The coagulant was introduced into the clay-water mixture, at a constant rate of 0.05 mL/sec, after the clay-water mixture was pumped out of the turbidimeter. The flow rate contributions by the coagulant and clay pump were neglected since microbore tubing, which has a negligible flow rate contribution, was used. The water-clay-coagulant mixture was then pumped into the coiled flocculator.

The coiled flocculator was made of tubing wound around a cardboard tube. This was the section where the clay particles collide with coagulant particles to form flocs [(Selimgir, M., Lo, R., Matai, K., 2018)](https://github.com/AguaClara/high_g_flocculation/blob/master/HighGFlocculation_Spring2018_ResearchReportFinalDraft.md). Four pressure sensors were attached, at equal distances, to the flocculator. The sensors measured the difference in pressure between the two points where they were attached. Four sensors were used in order to determine how the pressure, and thus, head loss changed along the length of the flocculator. Finally, the water was pumped out of the system through the effluent line. See the manual for a detailed image of the flocculator.

#### Cleaning
After each experimental trial, air bubbles were introduced into the system at 1 rpm by the air pump. Water was also continually pumped at 76 rpm by the water pump to carry the air bubble through the flocculator. This cleaning system was used to scrape and clean any coagulant buildup on the flocculator wall in preparation for the next trial. Any fluids that entered the microbore tubing during the experiment, while the air pump was off, was contained in the 1L bottle attached to the air pump.

### Procedure

The system was fully automated through Process Control and Data Acquisition (ProCoDA) to run at the target turbidity, 20 NTU. PID CONTROL turned on the clay pump and ran for 15 minutes to allow for the system to reach and maintain the target turbidity. The next state, EXPERIMENT, started the coagulant pump and ran for three hours. This was the state from which the team collected the data. After EXPERIMENT, CLEANING (AIR) ran for four minutes. This state stoped the coagulant and clay pump, and started the 1 RPM air pump to introduce air into the system. The last state was CLEANING (WATER), which ran for five minutes and turned off the air pump to allow the water to force the air bubbles through the system. For more details on the team's ProCoDA method file, refer to the manual.

To run a experiment, the C-NARC ProCoDA method file was first opened and the blue influent valve was set to the open position. In manual operation, ProCoDA's state was changed to ON, which turned on the mixer and the water pump. The water pump was manually started at 76rpm and the red effluent valve was set to the open position after a brief delay to prevent back-flow of wastewater. Then, ProCoDA was switched from manual to automatic operation, after which the clay pump automatically turned on. Fifteen minutes later, before ProCoDA switched to the EXPERIMENT state, the pressure sensors were zeroed through ProCoDA. The experiment was left to run for three trials at the target turibidity. Finally, the change in pressure and the accumulation of head loss in the flocculator were observed for each trial.

## Results and Analysis
Present an observation (results), then explain what happened (analysis).  Each paragraph should focus on one aspect of your results. In that same paragraph, you should interpret that result.  
In other words, there should not be two distinct paragraphs, but instead one paragraph containing one result and the interpretation and analysis of this result. Here are some guiding questions for results and analysis:

When describing your results, present your data, using the guidelines below:
* What happened? What did you find?
* Show your experimental data in a professional way.
```python
from aide_design.play import*
x = np.array([1,2,3,4,5])
y = np.array([1,2,3,4,5])
plt.figure('ax',(10,8))
plt.plot(x,y,'*')
plt.savefig('/Users/jillianwhiting/github/Jillian-Whiting/Images/linear')
plt.show()
```
![linear](https://github.com/jillianwhiting/Jillian-Whiting/blob/master/Images/linear.png?raw=true)
Figure 1: Captions are very important for figures. Captions go below figures.

After describing a particular result, within a paragraph, go on to connect your work to fundamental physics/chemistry/statics/fluid mechanics, or whatever field is appropriate. Analyze your results and compare with theoretical expectations; or, if you have not yet done the experiments, describe your expectations based on established knowledge. Include implications of your results. How will your results influence the design of AguaClara plants? If possible provide clear recommendations for design changes that should be adopted. Show your experimental data in a professional way using the following guidelines:
* Why did you get those results/data?
* Did these results line up with expectations?
* What went wrong?
* If the data do not support your hypothesis, is there another hypothesis that describes your new data?

## Conclusions
The C-NARC team focused on the theoretical calculations to find the headloss from one coagulant nanoparticle attached to the walls on the flocculator for the first half of the semester. This was then compared to the average headloss from each pressure sensor to find the total number of coagulant nanoparticles on the tubing. This value is important to AguaClara in the lab because if coagulant is attaching to the walls, the rate and total amount of attachment to clay particles will be decreased. The number of coagulant nanoparticles on the walls also varies with respect to turbidity levels in which rate attachment to the walls are higher at lower NTUs. At lower turbidity levels, there are fewer clay particles in solution and therefore the coagulant will attach to the walls faster than if there were more clay particles to attach to.

In the second half of the semester, the C-NARC team will be focused on finding the attachment rate of coagulant nanoparticles to clay particles. This will be important in finding optimal flow rates and turbidity levels in which minimal head loss occurs so the least amount of coagulant is wasted.



## Future Work
Currently, the team was able to find out the number of nanoparticles sticking to the flocculator wall, however, the team still needs to figure out the number of nanoparticles sticking to clay and in suspension. The first information the team needs to find out would be how many coagulant nanoparticles there are in total in the solution so the team can eliminate the amount sticking to the wall. To do that, the team will be using the information that there is 0.1418 g/L of Al and find out the molecular formula ([Al<sub>n</sub>(OH)<sub>m</sub>Cl<sub>3n-m</sub>]<sub>x</sub>) using the known basicity (m/3n). After that, the team can use the density of Al to figure out initial volume concentration of the coagulant stock solution.
After the team figures out the total number of coagulant nanoparticles in suspension and sticking to the clay, the issue the team is still having is that the team is not sure how to figure out the number of nanoparticles stuck to clay versus the number of nanoparticles in suspension.
An additional challenge for the team would be figuring out how the difference in NTU affects the number of nanoparticles in the three different locations. For example, at higher NTU there would be no coagulant in suspension because the coagulant would be mainly attaching to clay.



## References
Gebbie, P. (2006). An Operator's Guide to Water Treatment Coagulants [PDF file]. Retrieved from http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf

Weber-Shirk, M., Guzman, J., O'Connor, C., Pennock, W., Lion, L. & Du, Y. (2018). *Aguaclara Textbook*. Retrieved from https://aguaclara.github.io/Textbook/index.html.

Sausele D., Shah, M., (2018). Coagulant Nanoparticle Attachment Rate Characterization, Fall 2018

Kinetic Energy of Tube Flow. (n.d.). Retrieved February 22, 2019, from http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html

Velocity Profile for Tube Flow. (n.d.) Retrieved March 15, 2019, from http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html

### Experimental Apparatus

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

Figure 16: Experimental setup including the coiled flocculator with four attached pressure sensors.
</div>


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/flocculator.jpg?raw=true" >

Figure 17: Modified coiled flocculator with four pressure sensors attached.
</div>

#### Materials
- Pumps
  - Three (3) Masterflex 1.6-100 RPM pumps
  - One (1) Masterflex 1 RPM pump
- Turbidimeter
  - One (1) HF Scientific Inc MicroTOL Turbidimeter 0-1000 NTU
    - measures influent turbidity after clay additional
- Flow accumulator
  - 1L Nalgene bottle, fitted with two small push-to-connect openings
- Modified coiled flocculator
  - Cardboard tube (OD = 8cm, L = 50cm)
  - Four (4) 1/4" hard tubing (L = 9'9")
  - Three (3) 1/4" hard tubing (L = 2")
  - Five (5) 1/4" push-to-connect t-joints
  - Eight (8) small cable ties
  - Four (4) 200 kPa pressure sensors
- Tubings and Fitting
  - 1/4" hard tubing
  - Microbore tubing
  - Two (2) yellow-blue soft tubing
  - Size 16 soft tubing
  - Two (2) 1/4" push-to-connect t-joints
- Stock solution materials
  - 6L tank for clay stock, fitted with a small push-to-connect opening
  - 22L bucket fitted with a small push-to-connect opening
  - Distilled water
  - Kaolinite Clay
  - Polyaluminum chloride (PACl)


### Experimental Methods
#### Set up
1. Power all three pumps.
2. Open the blue influent valve.
3. Turn on the water pump at 100 rpm.
4. Open the red effluent valve.

#### Experiment
1. Set the water pump to 76 rpm.
2. Begin the ProCoDa program and set the PiD control from ON to OFF state.
3. Run until the turbidity is stabilized.
4. Manually turn on the coagulant pump at 20 rpm.
5. Track the pressure difference in the flocculator.

#### Cleaning Procedure
1. Run water through the system until the clay and coagulant is cleared out.
2. Set the PiD from ON state to OFF state.
3. Switch off all pumps.
4. Close the blue influent and red effluent valve.

## ProCoDa Method File
### States
#### OFF
The default state when no data is being collected from the pressure sensors.
In this state, all the pumps are off.

#### ON
The state that powers the mixer and turns on the water pump.

#### PiD Control
The state that powers the clay pump
The flow rate of the clay pump is controlled by the PiD controller to reach the target turbidity determined by the turbidimeter

#### Experiment
The state that starts the coagulant pump. The flow rate is set by the PumpControl (coag) variable. The state runs for three hours.

#### Cleaning (air)
The state that turns off the coagulant and clay pumps and starts the air pump to introduce bubbles into the system. The bubbles scour away any build up along the flocculator walls.

#### Cleaning (water)
The state that turns off the air pump. Just water flows through the system at this point, flushing out any remaining air bubbles.

### Set Points
| Set Point | Operation Type | Value |
|:--------    |:--------:|:----:|
| OFF      |         1     |             0 |
|ON   | 1  |  1 |
|Influent Turbidity Target  | Variable | increment rep function  |
|P   |  Constant |2.5m   |
| i  |Constant   | 45m  |
| D   |  Constant |0   |
|Influent Turbidimeter ID   |  Constant |  2 |
|Influent Turbidity   | Variable   | HF turbidimeter function  |
|Pump Control (Clay)   |  Variable |  PID setpoint no reset function |
|Coag flow rate| Constant | 49.6m |
|mL per rev YB| Constant | 149m |
|PumpControl (Coag)| Variable |  pump control function |
|Mixing time| Constant | 10 |
|PID clay time| Constant | 900 |
|Bubble time| Constant | 240 |
|Experiment time| Constant | 10.8k |
|Clean water time| Constant | 300 |
|slope| Constant |-20 |
|intercept| Constant |100 |
|max x| Constant  | 5 |
|reps| Constant | 3 |
|loop counter| Variable  | count states function |
|count target| variable | multiply function |
