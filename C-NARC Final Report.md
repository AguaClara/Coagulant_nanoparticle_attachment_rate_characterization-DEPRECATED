# Coagulant-Nanoparticle Attachment Rate Characterization, Spring 2019
#### Ada Lian, Valentine Starnes, Yeonjin Yun
#### May 10th, 2019

**[Felix: Hello! I will be making comments in these bolded square brackets.]**

**[After addressing any comments please write within the brackets "-Addressed __" with the individual's initials in the __ space. They will be deleted them in the next report.]**


## Abstract
The Spring 2019 Coagulant-Nanoparticle Attachment Rate Characterization (C-NARC) team’s objective was to continue the previous team’s work in determining the rate of coagulant nanoparticle attachment, specifically the rate constant of that relationship, which the team hypothesized to be first order. In order to determine the rate at which nanoparticles are adhering to the flocculator wall, the team utilized the data the previous team collected. This will in turn determine the rate at which the nanoparticles are attaching to clay. Through determining the rate the nanoparticles attach to clay, the team gains a better understanding of how the coagulant nanoparticles behave during flocculation.

## Introduction
The fundamental goal of AguaClara plants is to develop resilient, gravity-powered drinking water and wastewater treatment technologies that will provide clean and safe drinking water. The main challenges to achieve this goal are financial, technological and political barriers. In regards to the technological barrier, the goal of C-NARC’s team for Spring 2019 is to reduce the excess coagulant that does not adhere to the particles of influent. Coagulant is a nanoparticle that is added to untreated water to make dirty particles that attach to each other, causing them to increase in size and therefore to be more easily removed. Coagulant is one of the most expensive parts of the water treatment process in AguaClara plants and if coagulant sticks to the wall, a higher dosage of coagulant to compensate the loss could be required. The underlying problem is that the attachment process between coagulant and nanoparticles in influent is unknown. Coagulant particles either attach to the particles in untreated water, stay in suspension, or attach to the walls of the flocculator. Without clear relationship, reducing the amount of coagulant lost to the flocculator walls by changing certain variables becomes a challenge.

To solve this problem, C-NARC team will quantify the rate of attachment between coagulant, the walls and the clay particles. The C-NARC team will first compute theoretical calculations of our hypothesis and later conduct experiments to confirm the calculations. The team hypothesizes that the headloss accumulation in the flocculator is first order with respect to distance along the flocculator. The rate constant from the first order relationship will be calculated utilizing experimental data obtained by Fall 2018 team. Once this relationship is established, AguaClara plants would be able to alter the variables depending on the specific situation, whether it is at low turbidity or at low flow rate. Through determining the rate of nanoparticle attachment to clay, the C-NARC gains a better understanding of coagulant behavior based off of varying turbidity levels and flow rates. This is important for AguaClara since optimizing the amount of coagulant needed will decrease input costs, directly tackling the financial barrier that AguaClara faces. **[, directly tackling the financial barrier that AguaClara faces-AddressedAL].**

**[What is dissipation? You used that term only once in this report. -AddressedVS. Also would recommend separating into two paragraphs here. It's a huge chunk of text.-AddresedVS]**
## Literature Review
#### Coagulation and Flocculation
In untreated water, there are numerous inorganic and organic particles that are too small to be removed by a filter. Therefore, coagulation and flocculation are important steps in the water treatment process to aid the removal of those particles. AguaClara plants use polyaluminium chloride (PACl), which is a coagulant that precipitates in water to create sticky nanoparticles [(Gebbie, 2006)](http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf). During flocculation in treatment plants, the fluid flows through baffles, which are plastic sheets that cause obstructions in the flow of fluid. In lab settings, the fluid flows through coiled tubing. Both methods induce collisions between the coagulant nanoparticles and inorganic/organic particles in the untreated water. Those collisions form flocs, which are particle aggregates that are easier to remove later during the sedimentation process [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Flocculation/Floc_Intro.html). The issue, however, is that the nanoparticles are not only sticking to particles but also attaching to the flocculator wall or remaining in suspension. Using that information, the team will be able to find the rate at which coagulant nanoparticles attach to the three locations.

#### Headloss
As stated earlier, the attachment of nanoparticles to the flocculator wall is an issue because it increases the headloss along the flocculator. Headloss is defined as the loss of energy of a fluid as it flows through space, which is mainly caused by the friction between the fluid and the inside of the tubing [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Review/Review_Fluid_Mechanics.html#headloss). The Darcy-Weisbach equation (as shown below) explains the major losses.

$$ h_{f} = f\frac{L}{D}\frac{\overline{v}^2}{2g} = f\frac{8}{g\pi^2}\frac{LQ^2}{D^5} $$
Such that,
$$\small {h_{f}=major\:loss, \\
f=Darcy\:friction\:factor,\\
L=pipe\:length,\\
Q=pipe\:flow\:rate,\\
D=pipe\:diameter}
$$

[(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Review/Review_Fluid_Mechanics.html#headloss)
This equation also provides the technical reasoning behind the negative effect of coagulant buildup on the flocculator walls. As there is more coagulant nanoparticles sticking to the wall, the diameter of the tubing decreases. ![Headloss_diagram](/Images/Headloss_diagram.png)
**Figure 1: Coagulant buildup leds to a decrease in diameter, which causes an increase in headloss along the flocculator** [(Sausele & Shah, 2018)](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20final%20report.pdf).

**[Excellent picture!]**

The relationship between headloss and the tube diameter is inversely proportional. In other words, as the tube diameter decreases due to coagulant sticking to the wall, the headloss increases. The amount of headloss, in other words, is proportional to the number of coagulant nanoparticles that are sticking to the wall. As more coagulant nanoparticles are attached to the wall, there is more force pulling the water against the water flow, which in turn increases the headloss. Using that relationship and the headloss data collected from last semester, we will be able to find the number of nanoparticles sticking to the wall in each of the four sections of the flocculator.

#### Drag Force
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
[("Velocity Profile for Tube Flow", n.d.)](http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html)
The velocity can be calculated by the fact that the water flow is laminar due to the small diameter of the tubing.

![Velocity_Profile](/Images/Velocity_Profile.png)
**Figure 2: Velocity Profile of laminar flow.** [("Velocity Profile for Tube Flow", n.d.)](http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html)

## Previous Work
Previous research from the Fall 2018 C-NARC team focused on determining the rate at which free coagulant attached to the flocculator wall. The team connected four pressure sensors along the coiled flocculator at equal distances to observe the rate of headloss accumulation in each section. The results showed that the rate of headloss accumulation decreased along the length of the flocculator. These results reflected that the coagulant had attached either to clay or to the first sections of the wall. Additionally, the relationship between clay concentrations and rate of headloss accumulation was unclear. The first section of the flocculator showed a direct relationship between turbidity and head loss accumulation in which a decrease in clay concentration resulted in a decrease in headloss accumulation. Conversely, the second and third section showed an inverse relationship between turbidity and rate of headloss accumulation while the fourth section showed no relationship [(Sausele & Shah, 2018)](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20final%20report.pdf). It was hypothesized that the inverse relationship occurred because as turbidity decreased, the amount of clay for coagulant to attach to decreased, thus there were more free coagulant nanoparticles to attach to the flocculator walls. It is unknown why in the first section a decrease in turbidity resulted in less headloss accumulation. This result may suggest that a clay-coagulant mixture was sticking to the flocculator walls as well as free coagulant particles.

The C-NARC team aimed to measure the first order rate constant for the loss of coagulant to flocculator walls as well as the first order rate constant for the loss of coagulant to clay surfaces. In order to find the amount of coagulant nanoparticles on the flocculator walls, the team found the velocity at the center of one coagulant particle on the wall, then found the drag force and head loss accordingly. These calculations were compared to last semester’s headloss accumulation results to estimate the total number of coagulant nanoparticles on the walls. Furthermore, the team calculated the amount of coagulant left in suspension **[suspension-AddressedYY]** and attached to the clay as a function of position. Experiments were conducted to verify these calculations and repeated at varying velocities and turbidity levels.

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

**Table 1: Shows the list of constants used in various calculations to find the number of coagulant particles on the flocculator wall.**

The initial goal was to calculate the velocity at the center of one coagulant nanoparticle on the wall of the tubing. The first step towards this was to find the flow of the solution through the tubing. The water pump was set to turn 76 revolutions per minute and peristaltic pump tubing size 16 allows 0.8 mL of solution per revolution. The formula for the tube flow is given below:
$$ Tube Flow = RPM * V_{f}$$

Therefore, the tube flow represents the amount of solution per time that has flowed through the tube. The mean velocity is then calculated from the tube flow divided by the cross sectional area of the tubing.
 $$u_{m} = \frac{TubeFlow}{\pi R²}$$

This mean velocity represents the average velocity of one coagulant nanoparticle flowing through the tube. Finally, the maximum velocity in fully developed velocity profile is given by the following formula:
$$ v_{m} = 2u_{m} $$

This shows the maximum velocity of a coagulant nanoparticle which would be in the middle of the tube due to the least amount of drag or shear force. This maximum velocity is then used to find the velocity at the center of one coagulant nanoparticle on the wall of the tubing which was calculated by the following formula:
$$ V(r) = v_{m}[1- \frac{r^2}{R^2}]$$
Since the radius of the coagulant nanoparticle is $0.45nm$ and the radius of the tube is $0.002159m$, the value of “r” is the difference between these which is $0.002158955m$. Given this radius, the velocity of one particle was calculated to be $5.7692×10^-6$ $m/s$.

The next step was to find the drag force on one coagulant nanoparticle on the tubing. First, the drag coefficient is given by:
 $$ Cd = \frac{24}{Re}$$
where the Reynolds number is $Re = \frac{\rho vD}{μ}$
 and $\rho$ is the density, v is the velocity, D is the diameter of the tubing and μ is the dynamic viscosity. Then, the drag force is calculated by:
$$ F_{d} = \frac {1}{2} C_{d} A \rho v^2$$
Given a velocity of $5.769×10^{-6} m/s$, the calculated drag force was $-8.55*10^{-24}$ $\frac{kg*m}{s^2}$. The next step was to find the headloss from one coagulant nanoparticle on the tubing. The headloss was given by the formula:
$$ H_{L} = \frac{-F_{d}}{\pi R² \rho g}
$$
The head loss was calculated as $5.968×10^{-21} cm$. This was compared to last semester’s results from 20 NTU.  Last semester’s hypothesis was that more coagulant will attach to the wall of the tubing due to less clay particles in the solution. Since the second and third pressure sensor had the expected inverse relationship, we picked the lowest NTU available (Sausele & Shah, 2018). The data from 2 separate experiments ran at 20 NTU were averaged to give $H_{L,avg}$. In order to calculate the number of coagulant particles attached to the walls of the tubing, the average headloss at each pressure sensor was divided by the headloss of one coagulant particle obtained from above calculations.
$$	Nanoparticles\:on\:wall = \frac {H_{L,avg}\:at\:one\:sensor}{H_{L}\:from\:1 \:coagulant}$$

**[Is H_L,avg and H_L the same? Use one or the other if this is the case-AddressedVS]**

This equation shows the number of nanoparticles from each section of the flocculator. The total number of nanoparticles attached to the whole flocculator tubing would be the sum of each total at the four pressure sensors. The total number of coagulant nanoparticles on the whole flocculator was $4.71 * 10^{20} \frac{particles}{hour}$.

### Experimental Apparatus
The Fall 2018 team conducted experiments with four different iterations of the experimental design. The three initial iterations were modified and improved upon before arriving at the current version.

The experimental setup, shown in Figure 3 and Figure 4, included the following: three pumps to introduce water, clay, and coagulant to the system; a flow accumulator; an influent turbidimeter;  a modified coiled flocculator; and an air pump for cleaning the system between each experimental trial. See the manual for more information on the setup.

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

**Figure 3: Experimental setup showing the flow of water, coagulant, and clay. Included in the experimental setup was the coiled flocculator with four attached pressure sensors.**
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/exptsetup2.jpg?raw=true" >

**Figure 4: Image of the bench setup, including the modified coiled flocculator.**
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

A stock solution of PACl coagulant with the concentration of 0.1418 g/L was prepared. The coagulant was introduced into the clay-water mixture, at a constant rate of 0.05 mL/sec, after the clay-water mixture was pumped out of the turbidimeter. The flow rate contributions by the coagulant and clay pump were neglected since microbore tubing, which has a negligible flow rate contribution, was used. The water-clay-coagulant mixture was then pumped into the coiled flocculator.

The coiled flocculator was made of tubing wound around a cardboard tube. This was the section where the clay particles collide with coagulant particles to form flocs [(Selimgir, M., Lo, R., Matai, K., 2018)](https://github.com/AguaClara/high_g_flocculation/blob/master/HighGFlocculation_Spring2018_ResearchReportFinalDraft.md). Four pressure sensors were attached, at equal distances, to the flocculator. The sensors measured the difference in pressure between the two points where they were attached. Four sensors were used in order to determine how the pressure, and thus, head loss changed along the length of the flocculator. Finally, the water was pumped out of the system through the effluent line. See the manual for a detailed image of the flocculator.

#### Cleaning
After each experimental trial, air bubbles were introduced into the system at 1 rpm by the air pump. Water was also continually pumped at 76 rpm by the water pump to carry the air bubble through the flocculator. This cleaning system was used to scrape and clean any coagulant buildup on the flocculator wall in preparation for the next trial. Any fluids that entered the microbore tubing during the experiment, while the air pump was off, was contained in the 1L bottle attached to the air pump.

### Procedure
The system was fully automated through Process Control and Data Acquisition (ProCoDA) to run at the target turbidity, 20 NTU. PID CONTROL turned on the clay pump and ran for 15 minutes to allow for the system to reach and maintain the target turbidity. The next state, EXPERIMENT, started the coagulant pump and ran for three hours. This was the state from which the team collected the data. After EXPERIMENT, CLEANING (AIR) ran for four minutes. This state stoped the coagulant and clay pump, and started the 1 RPM air pump to introduce air into the system. The last state was CLEANING (WATER), which ran for five minutes and turned off the air pump to allow the water to force the air bubbles through the system. For more details on the team's ProCoDA method file, refer to the manual.

<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/ProCoDa_setup.PNG?raw=true" >
<div style = "text-align:center; font-weight:bold">
Figure 5: ProCoDA setup
</div>

To run a experiment, the C-NARC ProCoDA method file was first opened and the blue influent valve was set to the open position. In manual operation, ProCoDA's state was changed to ON, which turned on the mixer and the water pump. The water pump was manually started at 76rpm and the red effluent valve was set to the open position after a brief delay to prevent back-flow of wastewater. Then, ProCoDA was switched from manual to automatic operation, after which the clay pump automatically turned on. Fifteen minutes later, before ProCoDA switched to the EXPERIMENT state, the pressure sensors were zeroed through ProCoDA. The experiment was left to run for three trials at the target turbidity **[turbidity-AddressedAL]**. Finally, the change in pressure and the accumulation of head loss in the flocculator were observed for each trial.

## Results and Analysis
The velocity of flow at one coagulant particle adhered on the wall was calculated to be $5.769×10^{-6} m/s$. Compared to the maximum velocity in the velocity profile, the velocity seemed too low, but the assumption behind the calculation was a fully developed laminar flow velocity profile assuming no-slip condition, which is that velocity is 0 at the walls of the tubing. Since the particle is $5*10^{4}$ times smaller than the tube radius, the velocity lined up with expectation that it would be close to 0. Also, the **[the-AddressedAL]** low velocity value **[value-AddressedAL]** matches with the hypothesis that the  coagulant nanoparticles would not detach from the wall due to the flow. If the particles detach from the wall, then there would have been no headloss due to the coagulant particles on the wall.

The calculated drag force was $-8.55*10^{-24}$ $\frac{kg*m}{s^2}$. The hypothesis was that at the team's experimental setup, the velocity was slow enough not to cause the formed flocs to dissociate, and **[and-AddressedAL]** consequently not to detach the coagulant particles on the wall ~~as well~~. Low velocity at ~~the~~ the nanoparticle resulted in low drag force on the nanoparticle. The sign on the drag force was negative, because drag force against the flow. Then the headloss caused by one coagulant particle on the wall was calculated to be $5.968×10^{-21} cm$ taking the size and density of the coagulant particle into account. Then the team utilized the experimental results from Fall 2018 at 20 NTU. The 20 NTU data was used not other turbidities, because the team's goal was to investigate coagulant nanoparticle attachment rate characterization rate at relatively low turbidity, which would better represent an actual plant NTU on normal days. Number of particles at each segment was calculated and organized in the table below.

| Segment |  Total Headloss in segmant Average over 2 experiments/hour [cm/hr]   | Number of nanoparticles on the wall |
|:------- |:--------:|:-----:|
| 0  |  1.260  |$2.111×10^{20}$ |
| 1  |  0.728 | $1.220×10^{20}$|
| 2  |  0.353    | $5.915×10^{19}$ |
| 3  | 0.243    | $4.072×10^{19}$|
| Total  |  2.584   | $4.330×10^{20}$|

**Table 2: Shows the average headloss and calculated number of nanoparticles on the flocculator wall.**

**[Table requires units for headloss avg! Perhaps use the full name of average headloss per nanoparticle or average headloss for one nanoparticle_AddressedYY]**

<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Headloss_Graph_fin.png?raw=true">
<div style = "text-align:center; font-weight:bold">
Figure 6: Headloss change over time at 20 NTU, 2 Trials averaged.
</div>

The total number of particles on the wall throughout the entire flocculator was calculated to be $4.330 * 10^{20} \frac{particles}{hour}$. To explicitly compare, the number of particles in the initial inflow was calculated. In order to calculate that number, molecular formula of the coagulant was found to be $\left  [ Al_{10}\left ( OH \right )_ {21} Cl_{\left ( 3n-m \right )} \right ]_ {x}$ using the basicity value of 0.7, which is the basicity of coagulant used in Ithaca water plant and aguaclara lab. m and n could be varied, but in our calculation, n value of 10 was used. The concentration of Aluminum in stock is calculated from the concentration of aluminum in stock solution. From that, number of coagulant particles in inflow was calculated to be $1.155 * 10^{21} \frac{particles}{hour}$ based on tube flow.
 This also **[also_addressedYY]** lined up with the expectations that coagulant particles should not adhere to the wall, but should adhere to the clay particles in water. However, there was no clear distinction identified between particles in suspension and particles attached to the clay particles.

The position in the flocculator and headloss increase rate were plotted to identify the relationship.

<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Headloss_Rate_Graph.png?raw=true">

<div style = "text-align:center; font-weight:bold">
Figure 7: Headloss increase rate throughout position change in flocculator at 20 NTU.
</div>

As shown in the graph, although the segments of the flocculator have equal length, the rate did not decrease linearly. The assumption was that the rate of headloss increase will linearly decrease as going through the flocculator, because there will be less particles to attach to the walls of the flocculator. However, this graph shows that the rate of headloss increase, actually decreases. The reason might be that there was an unknown relationship between headloss and position in the flocculator. This should be further investigated in the next semester.

However, when the total headloss change from the beginning of the flocculator to the end of the flocculator was plotted over time, it was shown that the relationship was still linear. This linearity resulted from higher increase rate in the beginning of the flocculator and lower increase rate in the end of the flocculator as shown above. Therefore, when the total headloss is plotted over time, the relationship is linear when the rates are summed.
**[If this confirms your original assumption that rate of headloss increase will linearly decrease then you should state that explicitly, because the last figure seems to contradict that assumption! If I don't know what I'm talking about just ignore this haha.x _addressedYY]**

<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Total_Headloss_Graph.png?raw=true">
<div style = "text-align:center; font-weight:bold">
Figure 8: Total Headloss change in flocculator over time at 20 NTU.
</div>

All calculations are compiled in [Calculation.md file](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Calculation.md) in the C-NARC team's repository and as python codes in manual.

## Conclusions
The C-NARC team focused on the theoretical calculations to find the headloss from one coagulant nanoparticle attached to the walls on the flocculator for the first half of the semester. This was then compared to the average headloss from each pressure sensor to find the total number of coagulant nanoparticles on the tubing. This value is important to AguaClara in the lab because if coagulant is attaching to the walls, the rate and total amount of attachment to clay particles will be decreased. The number of coagulant nanoparticles on the walls also varies with respect to turbidity levels in which rate attachment to the walls are higher at lower NTUs. **[This is because_addressedYY]** This is because at lower turbidity levels, there are fewer clay particles in solution and therefore the coagulant will attach to the walls faster than if there were more clay particles to attach to.

In the second half of the semester, the C-NARC team focused on finding the attachment rate of coagulant nanoparticles to clay particles. The number of coagulant nanoparticles in the inflow was calculated as 1.155 * $10^{21}$/hour. The number of coagulant nanoparticles attached to the wall was found to be 4.330 * $10^{20}$/hour. By subtracting the coagulant nanoparticles on the wall from the inflow, the number of coagulant nanoparticles in suspension and attached to clay was found to be 7.218 * $10^{20}$/hour. This is important for decreasing costs in AguaClara plants because we will find optimal flow rates and coagulant doses to decrease headloss.

## Future Work
Currently, the team was able to find out the number of nanoparticles sticking to the flocculator wall, however, the team still needs to figure out the number of nanoparticles sticking to clay and in suspension.

Although the team figured out the total number of coagulant nanoparticles in suspension and stuck **[stuck-AddressedAL]** to the clay, the issue the team **[has-AddressedAL]** has is that the team is not sure how to differentiate those attached to clay versus those in suspension.

An additional challenge for the future team has would be figuring out how the difference in NTU affects the number of nanoparticles in the three different locations **[Why at the 3 different locations? It isn't clear from the next sentence that NTU would affect the three locations differently, since it seems to apply universally. And is the next sentence a valid assumption or something that is just used as an example that may not be true?-AddressedAL]**. For example, at higher NTU there would be less coagulant in suspension and on the flocculator wall because there are more clay particles for the coagulant nanoparticles to attach to.

Furthermore, it would be interesting to see the data on experiments with only water and coagulant. While it is expected that there will be a linear change in slopes between the different sections in the flocculator, it may show a nonlinear decrease in the particles on the wall. This could be explained by the fact that some clay particles attached to coagulant are sticking to the flocculator wall together. Additionally, before running any additional experiments, it is important to calibrate the pressure sensors to ensure that the experimental data is accurate.

## References
Gebbie, P. (2006). An Operator's Guide to Water Treatment Coagulants [PDF file]. Retrieved from http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf

Weber-Shirk, M., Guzman, J., O'Connor, C., Pennock, W., Lion, L. & Du, Y. (2018). *AguaClara Textbook*. Retrieved from https://aguaclara.github.io/Textbook/index.html.

Sausele D., Shah, M., (2018). Coagulant Nanoparticle Attachment Rate Characterization, Fall 2018 Retrieved from https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20Report.md

Kinetic Energy of Tube Flow. (n.d.). Retrieved February 22, 2019, from http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html

Velocity Profile for Tube Flow. (n.d.) Retrieved March 15, 2019, from http://hyperphysics.phy-astr.gsu.edu/hbase/pfric2.html

## Manual
**[Label this section as the "Manual"-AddressedAL]**
### Experimental Apparatus

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

**Figure 9: Experimental setup including the coiled flocculator with four attached pressure sensors.**
</div>


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/flocculator.jpg?raw=true" >

**Figure 10: Modified coiled flocculator with four pressure sensors attached.**
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

### ProCoDa Method File
#### States
##### OFF
The default state when no data is being collected from the pressure sensors.
In this state, all the pumps are off.

##### ON
The state that powers the mixer and turns on the water pump.

##### PiD Control
The state that powers the clay pump.
The flow rate of the clay pump is controlled by the PiD controller to reach the target turbidity determined by the turbidimeter.

##### Experiment
The state that starts the coagulant pump. The flow rate is set by the PumpControl (coag) variable. The state runs for three hours.

##### Cleaning (air)
The state that turns off the coagulant and clay pumps and starts the air pump to introduce bubbles into the system. The bubbles scour away any build up along the flocculator walls.

##### Cleaning (water)
The state that turns off the air pump. Just water flows through the system at this point, flushing out any remaining air bubbles.

#### Set Points
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

#### Graphical Data Analysis
```Python
import aguaclara.research.procoda_parser as pp
data_path= "Data"
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
import scipy.stats as stats

columns1 = pp.get_data_by_time(path=data_path, columns=[0,1,2,3,4], start_date="11-28-2018", start_time="13:49", end_time="16:42")

time1 = columns1[0]
pressure11 = columns1[1]
pressure12 = columns1[2]
pressure13 = columns1[3]
pressure14 = columns1[4]

columns2 = pp.get_data_by_time(path=data_path, columns=[0,1,2,3,4], start_date="11-28-2018", start_time="13:49", end_time="16:42")

time2 = columns2[0]
pressure21 = columns2[1]
pressure22 = columns2[2]
pressure23 = columns2[3]
pressure24 = columns2[4]

elapsed_time = ((np.array(time1)-time1[0])+(np.array(time2)-time2[0]))*24/2
pressure1 = ((np.array(pressure11)-pressure11[0])+(np.array(pressure21)-pressure21[0]))/2
pressure2 = ((np.array(pressure12)-pressure12[0])+(np.array(pressure22)-pressure22[0]))/2
pressure3 = ((np.array(pressure13)-pressure13[0])+(np.array(pressure23)-pressure23[0]))/2
pressure4 = ((np.array(pressure14)-pressure14[0])+(np.array(pressure24)-pressure24[0]))/2

plt.xlabel("Time (hours)")
plt.ylabel("Headloss (cm)")
line1,=plt.plot(elapsed_time,pressure1, color="blue")
line2,=plt.plot(elapsed_time,pressure2, color="red")
line3,=plt.plot(elapsed_time,pressure3, color="orange")
line4,=plt.plot(elapsed_time,pressure4, color="green")
plt.legend((line1,line2,line3,line4),("7kPa1","7kPa2","7kPa3","7kPa4"))
plt.title('Headloss over Time 2 Trials Averaged')
plt.savefig('Headloss_Graph_fin.png')

linreg1 = stats.linregress(elapsed_time, pressure1)
slope1, intercept1, r_value1 = linreg1[0:3]
linreg2 = stats.linregress(elapsed_time, pressure2)
slope2, intercept2, r_value2 = linreg2[0:3]
linreg3 = stats.linregress(elapsed_time, pressure3)
slope3, intercept3, r_value3 = linreg3[0:3]
linreg4 = stats.linregress(elapsed_time, pressure4)
slope4, intercept4, r_value4 = linreg4[0:3]

print("Slope1:", slope1)
print("R-squared1:", r_value1 ** 2)
print("Slope2:", slope2)
print("R-squared2:", r_value2 ** 2)
print("Slope3:", slope3)
print("R-squared3:", r_value3 ** 2)
print("Slope4:", slope4)
print("R-squared4:", r_value4 ** 2)


plt.xlabel("Position in flocculator")
plt.ylabel("Headloss increase rate (cm/hr)")
lines=plt.plot([1,2,3,4],[slope1,slope2,slope3,slope4], 'o')
plt.title('Headloss increase rate throughout the flocculator')
plt.savefig('Headloss_Rate_Graph.png')

pressuretot=pressure1+pressure2+pressure3+pressure4
plt.xlabel("Time (hours)")
plt.ylabel("Headloss (cm)")
linetot=plt.plot(elapsed_time,pressuretot, color="blue")
plt.title('Total Headloss change over entire flocculator')
plt.savefig('Total_Headloss_Graph.png')
```

#### Python Calculation for Data Analysis
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
veloncoag
Fdrag=-(CD*np.pi*(rcoagulant**2)*rho*(veloncoag**2)/2).to_base_units()
Fdrag

```

```python
g=9.8*u.m/(u.s**2)
coagheadloss=(-Fdrag/(np.pi*R*R*rho*g)).to(u.centimeter)
coagheadloss
```
Used headloss data at 20 NTU measured by Fall 2018.
```python
HLavg0=1.420*u.cm/u.hr
HLavg1=0.736*u.cm/u.hr
HLavg2=0.389*u.cm/u.hr
HLavg3=0.264*u.cm/u.hr

npwall0=HLavg0/coagheadloss
npwall1=HLavg1/coagheadloss
npwall2=HLavg2/coagheadloss
npwall3=HLavg3/coagheadloss

npwall0
npwall1
npwall2
npwall3

npwalltot=npwall0+npwall1+npwall2+npwall3
npwalltot
```

```python
FlocL=(9*u.foot+9*u.inch).to(u.m)
volcoagtot=npwalltot*(4/3)*np.pi*(rcoagulant**3)
surfAfloc=2*np.pi*R*FlocL

coagthickness=(volcoagtot/surfAfloc).to_base_units()

volcoagtot.to(u.m**3/u.hr)

surfAfloc

coagthickness.to(u.inch/u.hr)

```

$$Molecular\ Formula\ of\ coagulant = \left  [ Al_{n}\left ( OH \right )_ {m} Cl_{\left ( 3n-m \right )} \right ]_ {x}$$
```Python
basicity=0.7
basicity=m/3n
assumption
n=10
m=basicity*3*n
```

```python
concAl=0.1418*(u.g/u.liter)
molarmassAl=26.981539*(u.g/u.mol)
molconcAl=concAl/molarmassAl
molconcAl
molconccoag=molconcAl/10
molarflowcoag=(molconccoag*TubeFlow).to_base_units()
numcoagflow=(molarflowcoag*((6.023*10**23)/u.mol)).to(1/u.hour)
numcoagflow
numcoagflow.to(1/u.second)

numcoagflow-npwalltot
```
molconcAl=0.00526 mol/L
numcoagflow=1.155*10^21 particles/hour
npwalltot =4.71*10^20 particles/hour
numcoagflow-npwalltot=6.84*10^20 particles/hour
