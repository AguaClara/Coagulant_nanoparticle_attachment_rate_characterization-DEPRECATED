#Coagulant-Nanoparticle Attachment Rate Characterization, Spring 2019
#### Ada Lian, Valentine Starnes, Yeonjin Yun
#### February 22, 2019



## Abstract
The Spring 2019 Coagulant-Nanoparticle Attachment Rate Characterization (C-NARC) team’s objective was to continue the previous team’s work in determining the rate of coagulant and nanoparticle attachment, specifically the rate constant of that relationship. The team utilized the data the previous team collected to determine the rate at which nanoparticles are adhering to the flocculator wall and in turn determine the rate at which the nanoparticles are adhering to clay.

## Introduction
The fundamental goal of AguaClara plants is to develop resilient, gravity-powered drinking water and wastewater treatment technologies that will provide clean and safe drinking water to 2 billion people who currently do not have access to it. The main challenges to achieve this goal are financial, technological and political barriers. In regard to the technological barrier, the goal of C-NARC’s team for Spring 2019 is to reduce the excess coagulant that does not adhere to the particles of influent. Coagulant is one of the most expensive parts of the water treatment process in AguaClara plants and if there is dissipation, a higher dosage of coagulant to compensate the loss could be required. The underlying problem is that the attachment process between coagulant and nanoparticles in influent is unknown. Without this information, reducing the amount of headloss to the flocculator walls by changing certain variables becomes a challenge. To solve this problem, C-NARC team will quantify the rate of attachment between coagulant, the walls and the clay particles. The team hypothesizes that the headloss accumulation in the flocculator is first order with respect to distance along the flocculator. The rate constant from the first order relationship will be calculated utilizing experimental data obtained by Fall 2018 team. Once this relationship is established, AguaClara plants will be able to alter the variables depending on the specific situation, whether it is at low turbidity or at low flow rate.

## Literature Review
####Coagulation and Flocculation
Flocculation is an important step in the water treatment process because it causes collisions between the coagulant and inorganic/organic particles in the untreated water [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Flocculation/Floc_Intro.html). The fluid deformation caused by baffles–or coiled tubing in the lab setting–form flocs, which can easily be removed later in the sedimentation process. The coagulant and particles in the untreated water are able to stick together because the coagulant precipitates in water to create nanoparticles which are sticky. The inorganic and organic particles in the water sticks to the nanoparticles rather than the water molecules because the nanoparticles are more polar than water [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Rapid_Mix/RM_Intro.html). AguaClara plants use polyaluminium chloride (PACl) instead of the more commonly used alum coagulant because although alum is cheaper and more accessible, alum is only suitable for treating low pH water and a smaller dosage of PACl is needed [(Gebbie, 2006)](http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf).
####Headloss
Headloss is defined as the loss of energy of a fluid as it flows through space. Headloss is mainly caused by the friction between the fluid and the inside of the tubing but it is also caused by the internal friction between the fluids in the tube [(Weber-Shirk et al., 2018)](https://aguaclara.github.io/Textbook/Review/Review_Fluid_Mechanics.html#headloss). The Darcy-Weisbach equation (as shown below) explains the major losses.

$$ h_{f} = f\frac{L}{D}\frac{\overline{v}^2}{2g} = f\frac{8}{g\pi^2}\frac{LQ^2}{D^5} $$
Such that,
$$\small {h_{f}=major\:loss \\
f=Darcy\:friction\:factor\\
L=pipe\:length\\
Q=pipe\:flow\:rate\\
D=pipe\:diameter}
$$


This equation also provides the technical reasoning behind the negative effect of coagulant buildup on the flocculator walls. The relationship between headloss and the tube diameter is inversely proportional. In other words, as the tube diameter decreases due to coagulant sticking to the wall, the headloss increases.
####Drag Force
As mentioned above, the headloss is mainly caused by the friction between the surface
and the fluid, therefore, headloss is also caused by the friction between the surface of the coagulant nanoparticles stuck to the flocculator wall. By determining the drag force, we can also determine the headloss caused by one coagulant nanoparticle. The nanoparticle is extremely small, therefore we assumed that the shape is a sphere. The drag force of a sphere is shown as
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

##Previous Work
Previous research from the Fall 2018 C-NARC team focused on determining the rate at which free coagulant attached to the flocculator wall. The team connected four pressure sensors along the coiled flocculator at equal distances to observe the rate of headloss accumulation in each section. The results showed that the rate of headloss accumulation decreased along the length of the flocculator (ref). These results reflected that the coagulant had attached either to clay or to the first sections of the wall. Additionally, the relationship between clay concentrations and rate of headloss accumulation was unclear. The first section of the flocculator showed a direct relationship between turbidity and head loss accumulation in which a decrease in clay concentration resulted in a decrease in headloss accumulation. Conversely, the second and third section showed an inverse relationship between turbidity and rate of headloss accumulation while the fourth section showed no relationship [(Sausele & Shah, 2018)](https://github.com/AguaClara/Coagulant_nanoparticle_attachment_rate_characterization/blob/master/C-NARC%20final%20report.pdf). It was hypothesized that the inverse relationship occurred because as turbidity decreased, the amount of clay for coagulant to attach to decreased, thus there were more free coagulant nanoparticles to attach to the flocculator walls. It is unknown why in the first section a decrease in turbidity resulted in less headloss accumulation. This result may suggest that a clay-coagulant mixture was sticking to the flocculator walls as well as free coagulant particles.

The C-NARC team aims to measure the first order rate constant for the loss of coagulant to flocculator walls as well as the first order rate constant for the loss of coagulant to clay surfaces. In order to find the amount of coagulant nanoparticles on the flocculator walls, the team will first find the velocity at the center of one coagulant particle on the wall, then find the drag force and head loss accordingly. These calculations will be compared to last semester’s headloss accumulation results to estimate the total number of coagulant nanoparticles on the walls. Furthermore, the team will calculate the amount of coagulant left in suspension and attached to the clay as a function of position. Experiments will be conducted to verify these calculations and will be repeated at varying velocities and turbidity levels.

## References
Gebbie, P. (2006). An Operator's Guide to Water Treatment Coagulants [PDF file]. Retrieved from http://wioa.org.au/conference_papers/06_qld/documents/PeterGebbie.pdf

Weber-Shirk, M., Guzman, J., O'Connor, C., Pennock, W., Lion, L. & Du, Y. (2018). *Aguaclara Textbook*. Retrieved from https://aguaclara.github.io/Textbook/index.html.

Sausele D., Shah, M., (2018). Coagulant Nanoparticle Attachment Rate Characterization, Fall 2018
