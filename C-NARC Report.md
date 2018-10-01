# Coagulant Nanoparticle Attachment Rate Characterizaion, Fall 2018
#### Desiree Sausele and Meera Shah
#### September 28, 2018

[CEO: Hi CNARC! This is a great first draft! Some small typo style fixes in a few places, but overall lots of good info here. I will throw my edits in inside square brackets like this comment, feel free to delete them once you've addressed them]

## Abstract
The attachment of free coagulant nanoparticles to the flocculator walls decreases the coagulant available for flocculation of the clay particles. The rate at which the coagulant attaches to clay particles was quantified by the Fall 2018 Coagulant - Nanoparticle Attachment Rate Characterization (C-NARC) team. The first order rate constants for loss of free coagulant nanoparticles to the wall of the flocculator and the attachment of coagulant to clay particles at varying clay concentrations and velocity gradients was calculated. [cEO:Each of these sentences works well on its own, though overall it reads very disjointedly. Try rephrasing or connecting them a little differently]

## Introduction
Attachment of coagulant nanoparticles to the wall of the flocculator perpetuates several complications for the AguaClara plant. [CEO: [perhaps plural plants? Plant singular reads oddly to me, or perhaps change to "within an AguaClara plant] Firstly, it decreases the efficiency of the flocculator by increasing the rate at which head loss accumulates as water progresses through the plant, and thus, increases the energy demands of the plant. Additionally, the attachment of the nanoparticles to the flocculator walls increases the wastage of coagulants, resulting in higher doses of coagulant being required to compensate for the loss.

Previous research conducted by AguaClara’s Rapid Mix Contact Chamber (CC) team determined that once the clay particles bound to the coagulant, the nanoparticles did not attach to the flocculator walls. Moreover, increased coagulant accumulation to the walls of a straight-tube flocculator model resulted in an increase in the accumulation of head loss. This was because the cross-sectional area of the tubing through which the water flowed was reduced. Furthermore, it was determined that coagulant attachment increased at lower velocities of water since not enough torque was produced to prevent the coagulant from attaching to the walls [(Krishnamoorthysujatha et al. 2016)](https://github.com/AguaClara/contact_chamber/blob/master/rapid-mix-contact-fall2016.pdf). Coagulant buildup also increased at decreasing clay concentrations since the coagulant preferentially attached to the larger surface area of the flocculator wall [(Akpan et al. 2017)](https://github.com/AguaClara/contact_chamber/blob/master/rapid-mix-contact.pdf).

The Coagulant - Nanoparticle Attachment Rate Characterization (C-NARC) team was created to quantify the relationships identified by the Rapid Mix CC teams. The first order rate constants for the loss of coagulant to the flocculator walls at a velocity gradient and at different concentrations of clay was calculated. The loss of coagulant to the flocculator walls was determined by measuring the rate of accumulation of head loss along the length of the flocculator tube. This was measured by attaching four pressure sensors at equal intervals along the length of the flocculator pipe.

## Literature Review
#### Coagulation and Flocculation
AguaClara plants are heavily reliant on coagulation and flocculation processes to ensure that treated effluent meets water quality standards. Flocculation is the process by which particles collide and attach to each other, forming an agglomeration of contaminants. Coagulant nanoparticles provide a sticky surface for the successful attachment and aggregation of contaminant particles [(Guzman Weber-Shirt, O’Connor, Pennock, Lion, Du, 2018a)](https://aguaclara.github.io/Textbook/). [Check spelling of Weber-Shirk] Generally, highly polar aluminium and iron based coagulants are used in water treatment, and these coagulants precipitate in water to form nanoparticles. However, these coagulants are acidic and contribute to a decrease in the pH of water below the Environmental Protection Agency’s standards for safe drinking water. Alternatively, the AguaClara plant uses Polyaluminium Chloride (PACl) because it is less acidic and can be added in smaller doses compared to aluminium based coagulants [(Guzman et. al, 2018b)](https://aguaclara.github.io/Textbook/). [Is PACl not aluminum based or is it somply a different kind? Ambiguous here] The mechanism of flocculation is determined by the type of particle the coagulant is attaching to. Coagulant nanoparticles can attach to dissolved organic matter, organic suspended solids such as pathogens and inorganic suspended solids such as clay [(Guzman et. al, 2018b)](https://aguaclara.github.io/Textbook/). Upon the addition of the coagulant, the rate of coagulation is limited by how fast the precipitation of the coagulants in water to form nanoparticles occurs, how quickly the nanoparticles are transported to the contaminants, and the rate at which the contaminants adhere to the nanoparticles [(Guzman et. al, 2018c)](https://aguaclara.github.io/Textbook/).

#### Head Loss
In fluid mechanics, head refers to the energy of a fluid in terms of length and head loss is defined as the loss of energy of a fluid as it flows through a space [(Guzman et al., 2018d)](https://aguaclara.github.io/Textbook/).

As coagulant builds up on the flocculator walls, it effectively reduces the cross-sectional area through which water flows thus increasing head loss as seen in Figure 1.

![Figure 1](/Images/Headloss_diagram.png)
Figure 1. Coagulant build up on flocculator walls eventually leads to a reduced pipe diameter and causes head loss accumulation [(Tsang, Yun, and Delgado, 2018](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md).

[great diagram!]

In the model coiled flocculators the cross sectional area is a circle and the relationship between pipe diameter and head loss can be described by the Darcy-Weisbach equation:
$$ \Delta h = \frac{f_DLV^2}{2Dg} $$
In this equation, $\mathrm{\Delta h}$ is the head loss due to friction in the pipe ($\mathrm{m}$), $\mathrm{f_D}$ is the Darcy friction factor, L is the length of the pipe ($\mathrm{m}$), V is the velocity of the fluid through the pipe ($\mathrm{\frac{m}{s}}$), D is the diameter of the pipe ($\mathrm{m}$), and g is the acceleration due to gravity ($\mathrm{\frac{m}{s^2}}$).
A change in pressure can be described by an alternate form of the Darcy-Weisbach equation that includes the fluid density, ($\mathrm{\rho}$):
$$ \Delta p = \frac{f_DLV^2\rho }{2D} = \rho g \Delta h$$
Using this formula the team can relate the observed pressure changes to head loss accumulation.

## Previous Work
Although this [Fall 2018]  is the first semester for C-NARC research, research conducted by the Rapid-Mix Contact Chamber teams have proven that free coagulant particles attach to the flocculator walls, effectively increasing the head loss through the flocculator by decreasing its diameter [(Tsang, Yun, and Delgado, 2018)](https://github.com/AguaClara/contact_chamber/blob/master/ContactChamber_Spring2018.md). The head loss was calculated by measuring the change in pressure before and after the flocculator.
This method returns the overall head loss in the flocculator, but the C-NARC team aims to measure how the rate of head loss accumulation changes over the length of the flocculator.  To achieve this, the team will employ the same method just at shorter intervals.  Installing four pressure sensors at equal intervals over the flocculator will allow the team to see how the rate of head loss accumulation changes and thus know the rate at which coagulant is sticking to the flocculator walls.


#Bibliography  [Add a space to make the heading work right!]
Akpan, P., Teuffer, K., & Zhang, G., (2017). Rapid Mix Contact Chamber, Spring 2017.

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018a). Flocculation Model. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018b). Rapid Mix Introduction. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018c). Rapid Mix Theory and Future Work. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Guzman, J., Weber-Shirk, M., O’Connor, C., Pennock, W., Lion, L., & Du, Y., (2018d). Review: Fluid Mechanics. AguaClara Textbook. Retrieved from https://aguaclara.github.io/Textbook

Krishnamoorthysujatha, M., Moraes, J. C., & Escanciano, J., (2016). Rapid Mix Contact Chamber, Fall 2016.

Tsang, C., Yun, Y., Delgado, C., (2018). Contact Chamber, Spring 2018.
