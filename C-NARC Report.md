# Coagulant Nanoparticle Attachment Rate Characterizaion, Fall 2018
#### Desiree Sausele and Meera Shah
#### November 20, 2018
[Shuo: Hello C-NARC! I'll be writing my comments in the square brackets like this. Please feel free to delete this after revising or updating your report. Overall the report looks good but you can still improve your report in the following ways:
First, when you try to analyze your results or the figures you have shown, fit your data with some mathematical models and show the numbers. They are more convincing than words. Second, in your conclusion part, state why your results are important to AguaClara. Those can be found in the grading rubric, and before submitting your report, you can do a self-check. Looking forward to your final report!]

## Abstract
Attachment of free coagulant nanoparticles to the flocculator wall decreases the amount of coagulant available for flocculation of clay particles. However, coagulant bounded to clay cannot attach to the flocculator wall. The Fall 2018 Coagulant - Nanoparticle Attachment Rate Characterization (C-NARC) team’s goal was to determine the rate at which free coagulant attached to the flocculator wall and to calculate the rate at which the coagulant attached to clay. The objective was to determine the first order rate constants for loss of free coagulant nanoparticles to the flocculator walls and for attachment of coagulant to clay particles at varying clay concentrations and velocity gradients.

## Introduction
Attachment of coagulant nanoparticles to the wall of the flocculator perpetuates several complications within an AguaClara plant. Firstly, it decreases the efficiency of the flocculator by increasing the rate at which head loss accumulates as water progresses through the plant, and thus, increases the energy demands of the plant. Attachment of the nanoparticles to the flocculator walls also increases coagulant wastage, resulting in higher doses of expensive coagulant being required to compensate for the loss.


Although Fall 2018 is the first semester for C-NARC research, research conducted by the Rapid-Mix Contact Chamber (CC) teams have proven that free coagulant particles attach to the flocculator walls, effectively increasing the head loss through the flocculator by decreasing its diameter [(Tsang et. al., 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md).
The C-NARC team was created to quantify the relationships identified by the Rapid Mix CC teams. The team hypothesizes that head loss accumulation in the flocculator is first order with respect to distance along the flocculator. C-NARC seeks to determine the first order rate constants for the loss of coagulant to the flocculator walls by varying the velocity gradient and turbidity. The loss of coagulant to the flocculator walls is determined by measuring the rate of accumulation of head loss along the length of the flocculator tube. Head loss can be measured by attaching four pressure sensors at equal intervals along the length of the flocculator pipe.




## Literature Review
#### Coagulation and Flocculation
AguaClara plants are heavily reliant on coagulation and flocculation processes to ensure that treated effluent meets water quality standards. Flocculation is the process by which particles collide and attach to each other, forming an agglomeration of contaminants. Coagulant nanoparticles provide a sticky surface for the successful attachment and aggregation of contaminant particles [(Guzman, Weber-Shirk, O’Connor, Pennock, Lion, & Du, 2018a)](https://aguaclara.github.io/Textbook/).  Generally, highly polar aluminium and iron based coagulants are used in water treatment, and these coagulants precipitate in water to form nanoparticles. However, these coagulants are acidic and contribute to a decrease in the pH of water below the Environmental Protection Agency’s standards for safe drinking water. AguaClara plants use Polyaluminium Chloride (PACl) as an alternate because it is less acidic and can be added in smaller doses compared to other aluminium based coagulants, like alum [(Guzman et. al., 2018b)](https://aguaclara.github.io/Textbook/). The mechanism of flocculation is determined by the type of particle the coagulant is attaching to: Coagulant nanoparticles can attach to dissolved organic matter, organic suspended solids such as pathogens and inorganic suspended solids such as clay [(Guzman et. al., 2018b)](https://aguaclara.github.io/Textbook/). Upon the addition of the coagulant, the rate of coagulation is limited by how fast the precipitation of the coagulants in water to form nanoparticles occurs, how quickly the nanoparticles are transported to the contaminants, and the rate at which the contaminants adhere to the nanoparticles [(Guzman et. al., 2018c)](https://aguaclara.github.io/Textbook/).

#### Head Loss
In fluid mechanics, head refers to the energy of a fluid in terms of length and head loss is defined as the loss of energy of a fluid as it flows through a space [(Guzman et al., 2018d)](https://aguaclara.github.io/Textbook/).

As coagulant builds up on the flocculator walls, it effectively reduces the cross-sectional area through which water flows thus increasing head loss as seen in Figure 1.

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Headloss_diagram.png?raw=true" >

Figure 1: Coagulant build up on flocculator walls eventually leads to a reduced pipe diameter and causes head loss accumulation [(Tsang, Yun, & Delgado, 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md).
</div>


In the model coiled flocculators the cross sectional area is a circle and the relationship between pipe diameter and head loss can be described by the Darcy-Weisbach equation:
$$ \Delta h = \frac{f_DLV^2}{2Dg} $$
In this equation, $\mathrm{\Delta h}$ is the head loss due to friction in the pipe ($\mathrm{m}$), $\mathrm{f_D}$ is the Darcy friction factor, L is the length of the pipe ($\mathrm{m}$), V is the velocity of the fluid through the pipe ($\mathrm{\frac{m}{s}}$), D is the diameter of the pipe ($\mathrm{m}$), and g is the acceleration due to gravity ($\mathrm{\frac{m}{s^2}}$).
A change in pressure can be described by an alternate form of the Darcy-Weisbach equation that includes the fluid density, ($\mathrm{\rho}$):
$$ \Delta p = \frac{f_DLV^2\rho }{2D} = \rho g \Delta h$$
Using this formula the team can relate the observed pressure changes to head loss accumulation.

## Previous Work
Previous research conducted by AguaClara’s Rapid Mix CC team determined that once the clay particles bound to the coagulant, the nanoparticles did not attach to the flocculator walls. Moreover, increased coagulant accumulation to the walls of a straight-tube flocculator model resulted in an increase in the accumulation of head loss. This was because the cross-sectional area of the tubing through which the water flowed was reduced. Furthermore, it was determined that coagulant attachment increased at lower velocities of water since not enough torque was produced to prevent the coagulant from attaching to the walls [(Krishnamoorthysujatha, Moraes, & Escanciano, 2016)](https://github.com/AguaClara/contact_chamber/blob/master/rapid-mix-contact-fall2016.pdf). Coagulant buildup also increased at decreasing clay concentrations since the coagulant preferentially attached to the larger surface area of the flocculator wall [(Akpan, Teuffer, & Zhang, 2017)](https://github.com/AguaClara/contact_chamber/blob/master/rapid-mix-contact.pdf).

Other teams have calculated head loss by measuring the change in pressure before and after the flocculator.  This method returns the overall head loss in the flocculator, but the C-NARC team aims to measure how the rate of head loss accumulation changes over the length of the flocculator.  To achieve this, the team will employ the same method just at shorter intervals.  Installing four pressure sensors at equal intervals over the flocculator will allow the team to see how the rate of head loss accumulation changes and thus know the rate at which coagulant is sticking to the flocculator walls. The team expects the attachment of coagulant to the clay and flocculator surfaces to be first order with respect to time and thus distance along the flocculator.  It follows that head loss accumulation in the flocculator should be first order with respect to distance along the flocculator.

## Methods

### Experimental Apparatus

The team conducted experiments with four different iterations of the experimental design. The three initial iterations were modified and improved upon before arriving at the current version.

The current experimental setup, shown in Figure 2 and Figure 3, included the following: three pumps to introduce water, clay, and coagulant to the system; a flow accumulator; an influent turbidimeter;  a modified coiled flocculator; and an air pump for cleaning the system between each experimental trial. See the manual for more information on the setup.

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

Figure 2: Experimental setup showing the flow of water, coagulant, and clay. Included in the experimental setup is the coiled flocculator with four attached pressure sensors.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/exptsetup2.jpg?raw=true" >

Figure 3: Image of the bench setup, including the modified coiled flocculator.
</div>

The experiment setup shown models the water flow through a plant on a smaller, lab-sized scale as follows:
1. The blue influent line delivers water to the water pump.
2. A concentration of clay stock is prepared and introduced into the water.
3. The pumps deliver the water and clay mixture to the turbidimeter.
4. The turbidimeter measures the influent turbidity of the clay-water mixture.
5. The coagulant is added immediately before the clay-water mixture enters the coiled flocculator. The flocculator allows for collisions between clay particles and coagulant nanoparticles.
6. The flocculator has four pressure sensors attached at equal distances by push-to-connect fittings to measure the pressure differences across the length of the flocculator.
7. The red effluent line transports wastewater out of the system.

Water was introduced into the system through the influent line. The flow rate of the water was maintained at a constant rate of 76 rpm by the water pump. The water was then pumped into the inlet of flow accumulator, which is a reservoir that allows continuous water flow through the system by reducing fluctuations caused by the pump. It consisted of a bottle with two taps: one for the entry of water and the other for the exit. At the beginning of an experiment, the bottle was filled with water up to just above the two holes. The bottle was then capped to trap the air inside and pressurize itself, thus maintaining the water level at a steady state [(Tsang et. al., 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md). The water then flowed out of the flow accumulator, after which clay was pumped into the water.
A stock solution of clay with the concentration of 2.0g/L was prepared, and the concentration at which it was introduced into the water by the clay pump was determined by the turbidity, measured by the influent turbidimeter.  The speed of the clay pump was varied by the Proportional - Integral - Derivative (PID) control to reach the target turbidity.

A stock solution of PACl coagulant with the concentration of 0.1418g/L was also prepared and introduced into the clay-water mixture, after the clay-water mixture was pumped out of the turbidimeter, at a constant rate of 20 rpm. The flow rate contributions by the coagulant and clay pump were neglected since microbore tubing, which has a negligible flow rate contribution, was used. The water-clay-coagulant mixture was then pumped into the coiled flocculator.

The coiled flocculator was made of tubing wound around a cardboard tube. This was the section where the clay molecules collide with coagulant particles to form flocs [(Selimgir, M., Lo, R., Matai, K., 2018)](https://github.com/AguaClara/high_g_flocculation/blob/master/HighGFlocculation_Spring2018_ResearchReportFinalDraft.md). Four pressure sensors were attached, at equal distances, to the flocculator. The sensors measured the difference in pressure between the two points where they were attached. Four sensors were used in order to determine how the pressure, and thus, head loss changed along the length of the flocculator. Finally, the water was pumped out of the system through the effluent line.

#### Cleaning
After each experimental trial, air bubbles were introduced into the system at 1 rpm by the air pump. Water was also continually pumped at 76 rpm by the water pump to carry the air bubble through the flocculator. This cleaning system was used to scrape and clean any coagulant buildup on the flocculator wall in preparation for the next trial. Any fluids that entered the cleaning system's microbore tubing the experiment, while the air pump was off, was contained in the 1L bottle attached to the air pump. [Keep the font of "Cleaning" same as before and after.]

### Procedure

First, the C-NARC ProCoDa method file was opened and the blue influent valve was set to the open position. In manual operation, ProCoDa's state was changed to ON, which turned on the mixer and the water pump. The water pump was manually started at 76rpm and the red effluent valve was set to the open position after a brief delay to prevent back-flow of waste water. Then, ProCoda was switched from manual to automatic operation, after which the clay pump automatically turned on. Fifteen minutes later, before ProCoDa switched to the EXPERIMENT state, the pressure sensors were zeroed through ProCoDa. The experiment was left to run for a set number of trials. Finally, the change in pressure and the accumulation of head loss in the flocculator were observed for each trial.

The system was fully automated, through ProCoDa, to run three trials at each target turbidity (100, 80, 60, 40, and 20 NTU), starting at the highest target NTU and ending with the lowest. PID CONTROL turned on the clay pump, which ran for 15 minutes until the system reached and maintained the target turbidity. The next state, EXPERIMENT, started the coagulant pump and ran for three hours. This is the state from which the team collected data. After EXPERIMENT, the next state was CLEANING (AIR), which ran for four minutes. This state stopped the coagulant and clay pump, and started the 1 RPM air pump to introduce air into the system. The last state was CLEANING (WATER), which ran for five minutes. In this state, the air pump was turned off and only water was pumped through the system to force the air bubbles through and out of the system. For more details on the team's ProCoDa method file, refer to the manual.

## Results and Analysis

The trials for the current iteration were run in triplicates, with each triplicate containing 3 trials of the same NTU. The average of each triplicate was taken, and the results are shown in Figures 4 to 8. The graphs show that there is an increase in head loss over time for all sections of the flocculators. This increase is because over the course of the trial, coagulant nanoparticles accumulated on the flocculator wall, decreasing the tube's diameter and increasing the head loss.

The graphs also show that there is a decrease in the rate of change of head loss, depicted by the slope, across the length of the flocculator for all triplicates. The largest change in head loss was experienced by the first section of the flocculator because this was where nanoparticles accumulated the most. Across the length of the flocculator, the amount of free coagulant nanoparticles for attachment decreased because more coagulant had attached either to clay or to the first sections of the flocculator. Therefore, the rate of attachment of coagulant nanoparticles to the wall of the flocculator decreases, thus decreasing the rate of head loss along the length of the flocculator.

The team expected to see the overall head loss increase as turbidity decreased. This is because as turbidity decreases, there is less clay for coagulant to attach to and thus there are more free coagulant nanoparticles that can attach to the flocculator walls. However, aside from the 20 NTU trials, the team saw a decrease in head loss accumulation as turbidity decreased. This result suggests that perhaps it is the clay or a coagulant/clay mixture sticking to the flocculator.

</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/100NTU.png?raw=true" >

Figure 4: Average head loss of three trials over time at 100 NTU
</div>

</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/80NTU.png?raw=true" >

Figure 5: Average head loss of three trials over time at 80 NTU
</div>

</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/60NTU.png?raw=true" >

Figure 6: Average head loss of three trials over time at 60 NTU
</div>

</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/40NTU.png?raw=true" >

Figure 7: Average head loss of three trials over time at 40 NTU
</div>

The graph in Figure 8 shows a rapid increase and decrease in head loss at approximately 2.5 hours. C-NARC postulates that a disturbance to the apparatus, such as a sudden shake of the flocculator, could have caused these rapid changes.

</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/20NTU.png?raw=true" >

Figure 8: Average head loss of three trials over time at 20 NTU
</div>

For results of experiments run with the other experimental designs, refer to the manual.
[The figures are straightforward and easy to follow basically. You might noticed that the headloss over time somehow showed a linear relationship or quadratic some time. You can use linear regression to show the slope or the gradient of the line. In that case, readers can get a better understanding how the headloss varies with time.]

## Conclusions

The first half of the semester was focused on designing the experiment and assembling the modified coiled flocculator; however, only a few experiments were conducted and the team was not confident in the data obtained. Although the results support the hypothesis that the rate of head loss accumulation decreases over the length of the flocculator, the team wanted to troubleshoot address issues with the experimental design and conduct more experiments before attempting to characterize the rate of free coagulant nanoparticle attachment. Currently, the team is having trouble with the clay clogging in the microtubing and is working on trouble-shooting this issue.

Since changing the pressure sensors from 200kPA to 7kPA and automating the system, the team has only run one successful experiment. The results from this experiment clearly support the hypothesis that the rate of head loss accumulation is greatest in the first section of the flocculator and decreases over the length of the flocculator. More successful experiments need to be run to confirm these results before calculating the first order rate constants for coagulant attachment. 


## Future Work  

The C-NARC team will run several more experiments using the current version of the experimental design. The team still needs to run trials in which the velocity gradient is varied. Next, the team will calculate the first order rate constant for the transport of coagulant nanoparticles to the clay and flocculator surfaces.

A question arose during experimentation that can be explored in the future. After noticing that the coagulant was introduced into the system too far from the flocculator, the team questioned if other surfaces, such as the microbore tube through which coagulant was pumped, were also attaching free coagulant nanoparticles. This may become an issue in characterizing nanoparticle attachment rate if the the actual coagulant concentration entering the flocculator cannot be accurately determined. A future task is to determine if attachment is occurring to other surfaces of the tubing and the extent to which this is occurring.


## References

Akpan, P., Teuffer, K., & Zhang, G., (2017). Rapid Mix Contact Chamber, Spring 2017.

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018a). Flocculation Model. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018b). Rapid Mix Introduction. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018c). Rapid Mix Theory and Future Work. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018d). Review: Fluid Mechanics. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Krishnamoorthysujatha, M., Moraes, J. C., & Escanciano, J., (2016). Rapid Mix Contact Chamber, Fall 2016.

Selimgir, M., Lo, R., Matai, K., (2018). High G Flocculation, Spring 2018.

Tsang, C., Yun, Y., & Delgado, C., (2018). Contact Chamber, Spring 2018.



## Manual
### Experimental Apparatus

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

Figure 9: Experimental setup including the coiled flocculator with four attached pressure sensors.
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
The state that turns off the air pump. Just watr flows through the system at this point, flushing out any remaining air bubbles.

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

## Previous Iterations of Experimental Trials

### First Iteration

The first iteration of experimental trials include the first, second, and third trials. These trials comparing the change in head loss (cm) over time (hours), were set at influent target turbidity of 100 NTU. Figure 10, Figure 11, and Figure 12 show the results of the trials.

For trial 1, an increase in head loss over time was seen in the first and second sections of the flocculator, as shown by the data points for pressure sensors 0 and 1 on Figure 10. For trial 2, an increase in head loss over time was observed for all sections of the flocculator, as shown on the Figure 11. For trial 3, this trend was viewed in the first, second, and third section of the flocculator, as shown by the data for pressure sensor 0, 1, and 2 on Figure 12. This increase was because over the course of the experiment, coagulant nanoparticles accumulated on the flocculator wall, decreasing the tube’s diameter and increasing head loss over time.

Moreover, in the first hour of the experiment for all three trials, the rate of change of head loss, depicted by the slope of the graph, for the first section of the flocculator was lower than that for the second section of the flocculator. However, the rate increased and stabilized in the first section of the flocculator during the second hour of the trial. After the second hour, the rate of change of head loss remained positive, with some fluctuations caused by disturbances to the apparatus. For trial 1 and 2, the data for pressure sensors 0, 1, and 3 show that the rate of change of head loss decreased along the length of the flocculator, depicted by the different slope for each sensor. For trial 3, the data for pressure sensors 0, 1, and 2 show the same trend.


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_19_exp.png?raw=true" >

Figure 10: Graph of headloss (cm) over time (hours) for trial 1, showing a sharp spike after 1.5 hours.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_23_exp.png?raw=true" >

Figure 11: Graph of headloss (cm) over time (hours) for trial 2, showing head loss increasing over time.
</div>

In trial 1, a spike was observed between times 1.6 hours and 2 hours in the graph of all four pressure sensors. C-NARC postulated that the experimental apparatus may have been disturbed, causing rapid changes in the pressure as coagulant nanoparticles dislodged from the flocculator. In addition, trials 1 and 2 were cut short. The first trial was terminated when the coagulant stock was emptied and air was pumped into the system instead; C-NARC doubled the coagulant dose to ensure there was enough coagulant for running a full-length experiment for the remaining trials. The second trial was terminated after a disturbance of the apparatus. In order to minimize the disturbances, C-NARC secured the flocculator and pressure sensors with tape and zip-ties. The team also observed a buildup in the tubing after the introduction of coagulant and determined the addition point was too far from the entrance of the flocculator and moved it closer for the third trial.


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_25_exp.png?raw=true" >

Figure 12: Graph of headloss (cm) over time (hours) for trial 3, showing head loss increasing over time.
</div>

For trials 1 and 2, the results from the pressure sensor 2, which describes the third section of the flocculator, shows anomalies. The rate of change of head loss for this section of the flocculator was lower than that for the fourth section, marked by pressure sensor 3. C-NARC hypothesized that this could have been due to using a faulty pressure sensor or PID controller.
In order to test this hypothesis, C-NARC switched pressure sensors 2 and 3 for the third trial and compared the results with the trial 2. The results, shown by Figure 7, supported the hypothesis. The results for both the pressure sensors were expected to be the same since no components of the experiment were changed. However, the faulty pressure sensor, depicted by the grey data points, gave different results for both trials.  


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_comparing_sensors.png?raw=true" >


Figure 13: Comparison of results from trials 2 and 3 after switching pressure sensor 2 and 3, confirming pressure sensor 2 (grey) in trials 1 and 2 were faulty
</div>

### Second Iteration

The fourth trial was run for 15 hours. and the experimental results showed the first pressure sensor had the fastest rate of head loss accumulation, but the rest of the data has many disruptions, as seen in Figure 14. The team speculated that the disruptions may have been caused by a fluctuating influent turbidity, as seen in Figure 15, or by disturbances to the lab bench. Regardless, this data could not be used because the team needs a linear trend with minimal noise to determine the first order rate constants.

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/15hrexp.png?raw=true" >


Figure 14: Results from the 15 hour experiment. Note the jumps in data points for pressure sensors 1, 2, and 3.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/15hrturb.png?raw=true" >


Figure 15: Influent turbidity data for the 15 hour experiment. The cause of the spikes in turbidity is unknown to the team.
</div>

After this trial, the experiment time was shortened to 3 hours because the data needed to calculate the first order rate constants could be acquired within a shorter experimental time. The ProCoDa file was also changed to automate future experiments and allow the team to conduct more trials at once. To do this, four new states were created aside from ON and OFF. More information can be found in the ProCoDa Method File section of the manual.

### Third Iteration

Experiment 5 was conducted with the third iteration of the experimental design.

The team observed that a mixture of water and air had entered the tubing connecting the pressure sensors to the flocculator. In order to prevent this from occurring in future experiments, the tubing was shortened and the pressure sensors were oriented on the top of the flocculator.

To increase the accuracy of the results for future experiments, the pressure sensors were changed from 200kPa to 7kPa sensors since the 7kPa sensors are more sensitive to pressure changes.
