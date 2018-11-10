# Coagulant Nanoparticle Attachment Rate Characterizaion, Fall 2018
#### Desiree Sausele and Meera Shah
#### September 28, 2018

[EM: Hello! Similar to last report, I will be putting my comments in brackets below the paragraph in which I am referring to. Thx!]

## Abstract
Attachment of free coagulant nanoparticles to the flocculator wall decreases the amount of coagulant available for flocculation of clay particles. However, coagulant bounded by clay cannot attach to the flocculator wall. The Fall 2018 Coagulant - Nanoparticle Attachment Rate Characterization (C-NARC) team’s goal was to determine the rate at which free coagulant attached to the flocculator wall and to calculate the rate at which the coagulant attached to clay. The objective was to determine the first order rate constants for loss of free coagulant nanoparticles to the flocculator walls and for attachment of coagulant to clay particles at varying clay concentrations and velocity gradients.

## Introduction
Attachment of coagulant nanoparticles to the wall of the flocculator perpetuates several complications within an AguaClara plant. Firstly, it decreases the efficiency of the flocculator by increasing the rate at which head loss accumulates as water progresses through the plant, and thus, increases the energy demands of the plant. Additionally, the attachment of the nanoparticles to the flocculator walls increases the wastage of coagulant, resulting in higher doses of coagulant being required to compensate for the loss.

[EM: Side note, coagulant is also really expensive! It wastes a lot of money to continuously be buying it.]

Although Fall 2018 is the first semester for C-NARC research, research conducted by the Rapid-Mix Contact Chamber (CC) teams have proven that free coagulant particles attach to the flocculator walls, effectively increasing the head loss through the flocculator by decreasing its diameter [(Tsang et. al., 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md).
The C-NARC team was created to quantify the relationships identified by the Rapid Mix CC teams. The team hypothesizes that head loss accumulation in the flocculator is first order with respect to distance along the flocculator and seeks to determine the first order rate constants for the loss of coagulant to the flocculator walls by varying the velocity gradient and turbidity. The loss of coagulant to the flocculator walls is determined by measuring the rate of accumulation of head loss along the length of the flocculator tube. Head loss can be measured by attaching four pressure sensors at equal intervals along the length of the flocculator pipe.

[EM: The sentence that starts with "The team hypothesizes.." is super long. Consider breaking it into two sentences for readability.]


## Literature Review
#### Coagulation and Flocculation
AguaClara plants are heavily reliant on coagulation and flocculation processes to ensure that treated effluent meets water quality standards. Flocculation is the process by which particles collide and attach to each other, forming an agglomeration of contaminants. Coagulant nanoparticles provide a sticky surface for the successful attachment and aggregation of contaminant particles [(Guzman, Weber-Shirk, O’Connor, Pennock, Lion, & Du, 2018a)](https://aguaclara.github.io/Textbook/).  Generally, highly polar aluminium and iron based coagulants are used in water treatment, and these coagulants precipitate in water to form nanoparticles. However, these coagulants are acidic and contribute to a decrease in the pH of water below the Environmental Protection Agency’s standards for safe drinking water. Alternatively, AguaClara plants use Polyaluminium Chloride (PACl) because it is less acidic and can be added in smaller doses compared to other aluminium based coagulants, like alum [(Guzman et. al., 2018b)](https://aguaclara.github.io/Textbook/). The mechanism of flocculation is determined by the type of particle the coagulant is attaching to. Coagulant nanoparticles can attach to dissolved organic matter, organic suspended solids such as pathogens and inorganic suspended solids such as clay [(Guzman et. al., 2018b)](https://aguaclara.github.io/Textbook/). Upon the addition of the coagulant, the rate of coagulation is limited by how fast the precipitation of the coagulants in water to form nanoparticles occurs, how quickly the nanoparticles are transported to the contaminants, and the rate at which the contaminants adhere to the nanoparticles [(Guzman et. al., 2018c)](https://aguaclara.github.io/Textbook/).

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
The experimental setup was similar to that of the Spring 2016 Contact Chamber subteam. However, C-NARC’s setup did not include the contact chamber and the needle valve. Additionally, four pressure sensors were attached at equal distances on the flocculator. See the manual for more information on the setup.

[EM: Unless you are specifically going to describe the SP16 CC's setup or refer to an imagine, this information is irrelevant. The reader would have to have previous knowledge of the subteam or have to go back and look for their report. Instead, briefly mention what is found in the current setup as a lead-in to the paragraphs below.]

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Exptsetup.jpg?raw=true" >

Figure 2: Experimental setup showing the flow of water, coagulant, and clay. Included in the experimental setup is the coiled flocculator with four attached pressure sensors.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/Expt-setup.jpg?raw=true" >

Figure 3: Image of the bench setup, including the modified coiled flocculator.
</div>

The experiment setup shown in Figure 2 and Figure 3 models the water flow through a plant on a smaller, lab-sized scale as follows:
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

### Procedure
First, all three pumps were powered and the blue influent valve was set to the open position. The water pump was turned on at 100 rpm, and the red effluent valve was set to the open position after a brief delay to prevent backflow of waste water. Water was pumped until the turbidimeter and flocculator were cleared out, after which the water pump was set to 76 rpm. The PID control was set from the OFF to ON state, automatically turning on the mixer. The state was then changed to PID Control, and the clay pump automatically turned on. Once the turbidimeter stabilized at 100 NTU, the pressure sensors were zeroed, and the coagulant pump was manually turned on at 20 rpm. The experiment was left to run for a set number of hours. Finally, the change in pressure and the accumulation of head loss in the flocculator were observed.

[EM: How were the pressure sensors zeroed?]

## Results and Analysis
The first, second, and third trials, comparing the change in head loss (cm) over time (hours), were set at influent target turbidity of 100 NTU. Figure 4, Figure 5, and Figure 6 show the results of the trials.

For trial 1, an increase in head loss over time was seen in the first and second sections of the flocculator, as shown by the data points for pressure sensors 0 and 1 on Figure 4. For trial 2, an increase in head loss over time was observed for all sections of the flocculator, as shown on the Figure 5. For trial 3, this trend was viewed in the first, second, and third section of the flocculator, as shown by the data for pressure sensor 0, 1, and 2 on Figure 6. This increase was because over the course of the experiment, coagulant nanoparticles accumulated on the flocculator wall, decreasing the tube’s diameter and increasing head loss over time.

Moreover, in the first hour of the experiment for all three trials, the rate of change of head loss, depicted by the slope of the graph, for the first section of the flocculator was lower than that for the second section of the flocculator. However, the rate increased and stabilized in the first section of the flocculator during the second hour of the trial. After the second hour, the rate of change of head loss remained positive, with some fluctuations caused by disturbances to the apparatus. For trial 1 and 2, the data for pressure sensors 0, 1, and 3 show that the rate of change of head loss decreased along the length of the flocculator, depicted by the different slope for each sensor. For trial 3, the data for pressure sensors 0, 1, and 2 show the same trend.


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_19_exp.png?raw=true" >

Figure 4: Graph of headloss (cm) over time (hours) for trial 1, showing a sharp spike after 1.5 hours.
</div>

<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_23_exp.png?raw=true" >

Figure 5: Graph of headloss (cm) over time (hours) for trial 2, showing head loss increasing over time.
</div>

In trial 1, a spike was observed between times 1.6 hours and 2 hours in the graph of all four pressure sensors. C-NARC postulated that the experimental apparatus may have been disturbed, causing rapid changes in the pressure as coagulant nanoparticles dislodged from the flocculator. In addition, trials 1 and 2 were cut short. The first trial was terminated when the coagulant stock was emptied and air was pumped into the system instead; C-NARC doubled the coagulant dose to ensure there was enough coagulant for running a full-length experiment for the remaining trials. The second trial was terminated after a disturbance of the apparatus. In order to minimize the disturbances, C-NARC secured the flocculator and pressure sensors with tape and zip-ties. The team also observed a buildup in the tubing after the introduction of coagulant and determined the addition point was too far from the entrance of the flocculator and moved it closer for the third trial.


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_10_25_exp.png?raw=true" >

Figure 6: Graph of headloss (cm) over time (hours) for trial 3, showing head loss increasing over time.
</div>

For trials 1 and 2, the results from the pressure sensor 2, which describes the third section of the flocculator, shows anomalies. The rate of change of head loss for this section of the flocculator was lower than that for the fourth section, marked by pressure sensor 3. C-NARC hypothesized that this could have been due to using a faulty pressure sensor or PID controller.
In order to test this hypothesis, C-NARC switched pressure sensors 2 and 3 for the third trial and compared the results with the trial 2. The results, shown by Figure 7, supported the hypothesis. The results for both the pressure sensors were expected to be the same since no components of the experiment were changed. However, the faulty pressure sensor, depicted by the grey data points, gave different results for both trials.  


<div style = "text-align:center">
<img
align = "center"
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/CNARC_comparing_sensors.png?raw=true" >


Figure 7: Comparison of results from trials 2 and 3 after switching pressure sensor 2 and 3, confirming pressure sensor 2 (grey) in trials 1 and 2 were faulty
</div>


## Conclusions
The first half of the semester was focused on designing the experiment and assembling the modified coiled flocculator; however, a few experiments were conducted. Trouble-shooting issues that arose during experimentation has stopped the team's work for now.  Up to this point, the team is not completely confident in the data obtained from the first three experiments. Although the results support the hypothesis that the rate of head loss accumulation decreases over the length of the flocculator, the team would like to address some of the issues with the experimental design and conduct more experiments before attempting to characterize the rate of free coagulant nanoparticle attachment.

[EM: Excited to see how this work will continue! Great research thus far despite the issues faced. A suggestion: consider testing the pressure sensors before using them in an experiment by having them measure over a distance of an already known pressure change. Most of the sensors in the lab are wonky, so always assume the worst.]

## Future Work  
Before continuing experiments, the team plans on replacing the unstable pressure sensor and recalibrating the PiD control. Once the team has finished troubleshooting the experimental design, experiments can be run again.  The team will begin by repeating the first three experiments to confirm whether or not the data is valid. After which we will begin varying the turbidity and velocity gradient in order to determine the first rate constants for the transport of coagulant nanoparticles to the clay and flocculator surfaces.

[EM: Avoid using "we."]

A question arose during experimentation that may be explored later. After noticing that the placement of where the coagulant was added was too far from the flocculator, the team questioned what other surfaces free coagulant nanoparticles were attaching to before entering the flocculator.  This may become an issue in characterizing nanoparticle attachment rate if the team does not know the actual coagulant concentration entering the flocculator.

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
src= "https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/Images/setup.png?raw=true" >

Figure 8: Experimental setup including the coiled flocculator with four attached pressure sensors.
</div>

#### Materials
- Pumps
  - Three (3) Masterflex 1.6-100 RPM pumps
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
  - Two (2) 1L Nalgene bottle, fitted with small push-to-connect opening
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
In this state, the clay mixer and clay pump are off

#### ON
The state that powers the mixer

#### PiD Control
The state that powers the clay pump
The flow rate of the clay pump is controlled by the PiD controller to reach the target turbidity determined by the turbidimeter

### Set Points
| Set Point | Operation Type | Value |
|:--------    |:--------:|:----:|
| OFF      |         1     |             0 |
|ON   | 1  |  1 |
|Influent Turbidity Target   | Constant | Varied  |
|P   |  Constant |2.5m   |
| i  |Constant   | 45m  |
| D   |  Constant |0   |
|Influent Turbidimeter ID   |  Constant |  2 |
|Influent Turbidity   | Variable   | N/A  |
|Pump Control (Clay)   |  Variable |  NA |
