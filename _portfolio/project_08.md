---
title: Manufacturing of Composites<hr>
subtitle: 
image: assets/img/portfolio/proj8/p1.png
alt: 

caption:
  title: Manufacturing of Composites
  subtitle: Manufacturing
  thumbnail: assets/img/portfolio/proj8/Picture4.jpg
---
<h6 style="text-align:left">Overview</h6>
<p style="text-align:justify">
During the Spring of 2017, I enrolled in a manufacturing of advanced composites course taught by my former advisor, Professor Pipes, which really changed how I viewed manufacturing of composites.
Before the course, I had very little knowledge on composite manufacturing, equipment, and most importantly the physics understanding driving the phenomena observed during processing.
The class was very unique in structure, we attended lectures on Mondays to review relevant theories and experimentation plan, attended the composites laboratory on Wednesdays to conduct planned experiments, and presented our findings on Fridays and provided a ~15-20 page report on the results by the following Monday.
At the end of the course, my class was required to compile all of our reports into a book (~277 pages) and I couldn't have been more proud of the work accomplished by the end of the semester.
In this section, I provide a brief overview of the relevant theories learned, the experiments conducted, and composite parts manufactured.
</p>

<h6 style="text-align:left">Contents</h6>
<ol style="text-align:left;margin-left:30px">
<li>Cure kinetics and rheology</li>
<li>Polymer transitions</li>
<li>Heat transfer</li>
<li>Heat transfer simulations</li>
<li>Consolidation and compaction</li>
<li>Darcy's law</li>
<li>Vacuum assisted resin transfer molding</li>
<li>Thermosetting prepreg residual thermal response</li>
<li>Molding flow simulation</li>
<li>Manufacturing pin bracket</li>
</ol>

<h6 style="text-align:left">Cure Kinetics and Rheology</h6>
<p style="text-align:justify">
There are many types of polymers, linear, branched and cross-linked. 
Linear and branched can be further classified into thermoplastic or thermoset polymer types.
Thermoplastics can be reshaped by melting; however, thermosets are infusible.
Epoxies are common polymers found in composites, they have low shrinkage and excellent mechanical, chemical and adhesion properties.
Epoxies are cured by primary or secondary amines, and it is fully cured when bonds have formed at all epoxides and all amine bonding sites.
Most notably, every time a bond occurs, a consistent amount of energy is released, this physical phenomenon is what allows us to quantify how much an epoxy has cured.
The cured quantity is referred to as degree of cure, where it is the measure of the amount of heat released with time divided by the total heat released at full degree of cure.
From this definition, its value ranges between zero and one, where zero denotes uncured and one denotes fully cured.
Predicting the degree of cure allows us to plan the manufacturing cure cycle of composites to determine the temperature we must set and its duration. 
Moreover, such models can be a useful tool for determining storage temperature and track a prepreg's state at any given time, provided its history.
Phenomenological models allows us to predict degree of cures, these include models like the n<sup>th</sup> order and autocatalytic among many others.
Figure 1 illustrates the Differential Scanning Calorimeter (DSC) used for the experiments, the mounted samples, and measured heat flow to compute degree of cure.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i3.png" alt="" width="100%">
<figcaption>Fig. 1 - Differential Scanning Calorimeter (DSC) (top-left), samples inside of DSC (top-right), heat flow and degree of cure measurements obtained from experiments</figcaption>
</figure>
<p style="text-align:justify">
Rheology is the study of deformation and flow of matter, by analyzing a fluid that deforms continuously under the action of a shearing force.
Generally, Newton's law describes the relationship between the fluid's strain rate and shear stress, with the proportionality defined as viscosity.
Polymers are complex fluids and do not necessarily follow Newton's law as one would expect because a polymer's viscosity can be dependent on the strain rate.
Moreover, viscosity is also related to temperature, time, and degree of cure.
When a polymer cures, there are two important phases; namely, gelation and vitrificaiton.
After cure is complete, the polymer will exhibit a glass transition temperature.
For certain manufacturing processes that involve the flow of polymer, special attention is made to its viscosity and degree of cure.
Figure 2 is the instrument used for measuring viscosity properties of polymers.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i5.png" alt="" width="100%">
<figcaption>Fig. 2 - Rheometer (top-left) and samples inside of rheometer to measure viscosity as a function of temperature, time and shear rate</figcaption>
</figure>

<h6 style="text-align:left">Polymer Transitions</h6>
<p style="text-align:justify">
Understanding polymer transitions helps us determine the maximum temperature a polymer matrix composite part can withstand, how processing conditions affect the thermal stability of composites, and factors limiting the processing speed of composites.
Polymers used in composites are thermoplastics and thermosets, thermoplastics can be further classified as amorphous or semi-crystalline.
As the temperature increases, amorphous and semi-crystalline polymers behave differently and undergo different types of changes.
A DSC and DMA are used for measuring the change in heat flow to determine the change in crystallinity in semi-crystalline polymers.
Non-isothermal experiments are conducted from the melt temperature to a lower temperature to obtain crystallization range, isothermal experiments to characterize isothermal crystallization, and modulated DSC allow us to obtain the glass transition temperature and heat capacity.
The glass transition temperature was extracted from DMA experiments, running non-isothermal trials at constant frequency and displacement. 
Phenomenological models such as the Avrami equation or Velisaris and Seferis kinetics model allow us to predict changes in crystallization.
By predicting crystallization changes, we can account for crystallization shrinkage or transitions.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i6.png" alt="" width="100%">
<figcaption>Fig. 3 - DMA instrument for measuring glass transition temperature and plots depicting heat flow and degree of crystallinity from semi-crystalline polymer</figcaption>
</figure>


<h6 style="text-align:left">Heat Transfer</h6>
<p style="text-align:justify">
Polymer composites are processed in elevated temperature environments, which are transient and static during certain periods.
Heat transfer affects shape deviation due to residual stresses generated during the cure.
Anisotropic thermal strain are common sources of residual stresses.
Figure 4 illustrates the experiments conducted to measure temperature profile of laminates manufactured using an autoclave.

</p>
<figure>
<img src="/assets/img/portfolio/proj8/i7.png" alt="" width="100%">
<figcaption>Fig. 4 - Fabrication of laminates in autoclave for temperature measurements</figcaption>
</figure>


<h6 style="text-align:left">Heat Transfer Simulations</h6>
<p style="text-align:justify">
A matlab script was developed to understand the effect of various parameters in the cure kinetics and heat transfer models.
Figure 5. shows an example of the prediction generated to study the effects of autoclave temperature profile and the temperature within a laminate.
Heat transfer simulations reveal the extent of the lag between autoclave temperature and part temperature, and how different heat transfer coefficients and part thickness affect the lag.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i8.png" alt="" width="100%">
<figcaption>Fig. 5 - Example plots generated with Matlab script to predict  </figcaption>
</figure>

<h6 style="text-align:left">Consolidation and Compaction</h6>
<p style="text-align:justify">
In resin transfer molding, dry fiber layers are compacted as the mold closes or vacuum bag compresses it before injection of a curable resin matrix.
A pressure is applied to the dry fiber layers, and this pressure compacts the fibers by decreasing the fiber-to-fiber spacing.
Evidently, the more compaction you exert onto dry fiber reinforcement, the greater the fiber volume fraction you obtain after the resin cures.
Fiber bed compaction was measured for woven prepreg and dry fabric, and compared to theoretical values by assuming fibers act as bending beams between contacts and deriving the stiffness of a fiber in a box to show how dimensions changed as fiber bundle is compressed.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i9.png" alt="" width="100%">
<figcaption>Fig. 6 - Compaction experiment of dry fabric</figcaption>
</figure>

<h6 style="text-align:left">Darcy's Law</h6>
<p style="text-align:justify">
Darcy's law predicts the flow of viscous fluids in a porous media. 
The flow rate is related to the coefficient of permeability, gross cross-sectional area of flow, pressure, length of flow path, and viscosity of fluid.
For resin transfer molding, the polymer fluid travels through dry fiber reinforcements.
We can use this law to predict how long it will take the polymer fluid to travel a required distance, and couple this information with prediction of degree of cure to estimate whether the flow rate is sufficient for the resin transfer process.
To make use of this law, we need to measure what the permeability of the dry fabric is and Figure 7 illustrates experiments to measure this quantity.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i10.png" alt="" width="100%">
<figcaption>Fig. 7 - Experiment to measure dry fabric permeability for Darcy's law</figcaption>
</figure>

<h6 style="text-align:left">Vacuum Assisted Resin Transfer Molding</h6>
<p style="text-align:justify">
Vacuum Assisted Resin Transfer Molding (VARTM) has many advantages and is a common method to manufacture composites.
It can be used to fabricate very large parts (e.g., ship hulls, wind turbine blades etc.), parts can be complex, including integrated stiffeners, relatively low tooling and processing costs, and generally has better properties than wet layup.
However, the inlet and outlet design is critical and difficult to determine, fiber volume fractions are usually lower than prepreg, have greater propensity for voids, and control of resin uniformity is difficult (e.g., resin-rich regions).
To mitigate the difficulties, we make use of compaction understanding, permeability analysis, and flow and kinetics relations to successfully manufacture composites.
Figure 8 illustrates the VARTM process used for fabricating a radial dome, NACA duct, and wind blade. 
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i11.png" alt="" width="100%">
<figcaption>Fig. 8 - VARTM process used for fabricating several composite parts</figcaption>
</figure>

<h6 style="text-align:left">Thermosetting Prepreg Residual Thermal Response</h6>
<p style="text-align:justify">
A thermosetting resin expands/shrinks upon applied temperature change, due to thermal expansion and cure chemical shrinkage.
Laminates can have lamina oriented in such a way that residual stresses can form due to mismatching properties.
For example, a laminate of stacking sequence [0/90<sub>4</sub>] will bend after processing because of the mismatching properties.
We can observe this type of bending from Figure 9 below.
We can control how much residual stress forms, and hence the amount of bending or deformation by controlling the manufacturing temperature profile.

</p>
<figure>
<img src="/assets/img/portfolio/proj8/i12b.png" alt="" width="100%">
<figcaption>Fig. 9 - Bending of laminate due to mismatching lamina properties</figcaption>
</figure>

<h6 style="text-align:left">Molding Flow</h6>
<p style="text-align:justify">
Molding processes are those such as injection molding, transfer molding, and compression molding.
These processes may involve flowing a fiber filled polymer fluid, and the flow of a composite is complex as the fluid is not isotropic.
The fiber orientation affects the flow characteristics, that is, flow or viscosity may be directionally dependent.
To understand this phenomenon, experiments were conducted to study the flow of composite charges.
A composite charge is an uncured prepreg stacked in a predefined manner that is then compressed into a cavity.
Figure 10 shows the cavity or volume the charge will flow in (left), it is a wide open round space. 
The charge is the round puck seen to the right of the cavity mold, it is compressed into the cavity through application of pressure with a plunger.
The cavity, charge and platens are heated to ensure the polymer's viscosity decreases to allow for flow.
After consolidation and cooldown, we can see the ellipsoidal shape the charge took, the major axis is the direction where the fibers are least aligned and hence has the greatest viscosity.
This phenomenon is important to consider when attempting to manufacture a composite via transfer molding means, it can be predicted by using computational tools such as Moldex3D.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i13b.png" alt="" width="100%">
<figcaption>Fig. 10 - Molding of a center gated disk</figcaption>
</figure>

<h6 style="text-align:left">Manufacturing of Pin Bracket</h6>
<p style="text-align:justify">
Two pin brackets were manufactured, one pin bracket was manufactured poorly to demonstrate the importance of predictive tools for understanding the manufacturing process, and the second was manufactured successfully with aid of predictive tools.
The thermal history and cure kinetics were used to determine the degree of cure and viscosity throughout the manufacturing cycle based on thermocouple readings.
With the use of the models, it became clear what changes needed to be made to improve the manufacturing process and obtain a final part with high quality.
</p>
<figure>
<img src="/assets/img/portfolio/proj8/i14.png" alt="" width="100%">
<figcaption>Fig. 11 - Transfer molding of thermoset for fabricating pin bracket</figcaption>
</figure>