---
title: Large Scale Additive Manufacturing
subtitle: Increasing the efficiency of printing large scale composite parts<hr>
image: assets/img/portfolio/proj4/i23.png
alt: Additive3D

caption:
  title: Large Scale Additive Manufacturing
  subtitle: Data/Simulation
  thumbnail: assets/img/portfolio/proj4/p1.jpg
---
<p style="text-align:justify">
<strong>Team</strong>: Eduardo Barocio, Alan Franc, Vasudha Kapre, Pasita Pibulchinda, Miguel A. Ramirez, Jason Susnjara
</p>
<h6 style="text-align:left">Overview</h6>
<p style="text-align:justify">
Extrusion deposition additive manufacturing (EDAM) process has enabled fabrication of complex three-dimensional geometries in the scale of meters. 
This manufacturing process leverages fiber-reinforced polymer composites to produce tooling or molds to be utilized in conventional composite manufacturing processes (e.g., autoclave, compression molding, stamping etc.).
Processing fiber-reinforced polymer composites is not a trivial task, these materials are highly anisotropic and viscoelastic; moreover, the highly non-isothermal conditions throughout the EDAM process engenders residual stresses.
Consequently, the accumulation of residual stresses can cause the printed part to warp, delaminate, or fracture. 
The purpose of this project is to predict residual stresses and deformations of parts printed using EDAM with three different composite materials.
Prediciton of residual stresses and deformations will save manufacturing time and costs by increasing the efficiency of the design process.
Details of the simulation capability, including modeling approach, material models, implementation, verification and validation exercises can be found in the following reference [1]
</p>

<p style="text-align:justify">
<strong>Highlights</strong>:<br>
<ul style="text-align:left;margin-left:30px">
	<li>Successfully manufactured complex-shaped composite parts using large scale additive manufacturing system</li>
	<li>Characterized mechanical, thermal, and thermophysical properties of new composite material systems tailored for additive manufacturing</li>
	<li>Conducted verification of analysis of material models updated with characterized material properties</li>
	<li>Performed validation exercise to compare printed experiments (e.g., curved wedge, saddle plates, etc) with simulation results</li>
	<li>Demonstrated simulation capabilities are able to provide predicted deformations within experiment error</li>
	<li>Facilitated further development of commercial software tool, Additive3D, with additional verified and validated material cards</li>
</ul>
</p>

<h6 style="text-align:left">Mission</h6>
<p style="text-align:justify">
Figure 1 illustrates the flowchart of EDAM process and performance simulations, which requires an AM system card and a material card before any simulation commences.
To enable prediction of stresses and deformation in EDAM simulations, we need to obtain material model parameters for the material card.
To obtain these material model parameters, we need to perform material characterization which involves thermal, thermophysical, and mechanical experiments. 
The goal of this project was to demonstrate EDAM predictive capabilities by developing new material cards (i.e., integrate new composite materials) and comparing simulation results to experiment for validation.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i4.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 1 - Flowchart of EDAM process and performance simulation</figcaption>
</figure>
<h6 style="text-align:left">Material Characterized</h6>
<ol style="text-align:left;margin-left:30px">
<li>50% wt. carbon fiber reinforced polyphenylene sulfide (25% wt. CF-PPS)</li>
<li>25% wt. carbon fiber reinforced polysulfone (25% wt. CF-PSU)</li>
<li>25% wt. carbon fiber reinforced polyethersulfone (25% wt. CF-PESU)</li>
</ol>
<h6 style="text-align:left">Additive Manufacturing Systems</h6>
<p style="text-align:justify">
Two additive manufacturing systems were used; namely, the composites additive manufacturing research instrument (CAMRI) and the large scale additive manufacturing (LSAM) systems, shown in Figure 2. 
Geometries were printed for extracting samples to be used for material characterization.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i3.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 2 - EDAM systems</figcaption>
</figure>
<video width="100%" autoplay muted loop>
  <source src="/assets/img/portfolio/proj4/Media1c.mp4" type="video/mp4">
Your browser does not support the video tag.
</video><br>
<h6 style="text-align:left">Material Characterization</h6>
<p style="text-align:left">
There are seven important categories needed for the development of the material card. 
These include characterizing the glass transition temperature, micromechanical descriptors, mechanical properties, thermophysical properties, thermoviscoelastic properties, and micromechanical predictions. 
</p>
<p style="text-align:left"><strong>Glass Transition Temperature</strong></p>
<p style="text-align:justify">
The glass transition temperature, T<sub>g</sub>, defines the transition of a polymer from a "glassy" to a rubbery state.
The T<sub>g</sub> can be measured using a dynamic mechanical analyzer (DMA) or differential scanning calorimetry (DSC), this work opted to used a DMA instrument, TA Instruments<sup>&copy;</sup> Q800.
The procedure to carry out the experiment to measure the T<sub>g</sub> was obtained from ASTM D7028. 
Figure 3 illustrates the instrument's fixture with a sample loaded for bending application. 
The plot of storage and loss modulus with temperature allows us to extract the T<sub>g</sub>, where it is determined at the point where a the storage modulus begins to rapidly decrease. 
To determine this value, two tangent curves are superimposed onto the measured storage modulus curve, the first tangent occurs before the decay in storage modulus, and the second tangent at the inflection point or when the loss modulus is maximum.
An example is illustrated in Figure 4.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i5.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 3 - DMA experimental setup for measuring T<sub>g</sub></figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj4/i6.png" alt="EDAM systems" width="90%">
<figcaption>Fig. 4 - Determination of T<sub>g</sub></figcaption>
</figure>

<p style="text-align:left"><strong>Mechanical Properties</strong></p>
<p style="text-align:justify">
The in-plane tensile and shear properties (e.g., the print and stacking directions) were characterized using the procedure outline in ASTM D638 and ASTM D5379, respectively.
A mechanical test system (MTS) with digital image correlation were used to apply the load and measure the specimen's surface strain field. 
In Figure 5, an illustration is shown demonstrating the experimental setup for tension test, with the DIC system shown on the left and mounted specimen on the right.
Figure 6 shows the in-plane shear experimental setup, the Iosipescu fixture was used which requires a v-notch specimen mounted as shown.
In both figures, the white section contains fine black speckles that are tracked by the DIC cameras to determine its relative movement, displacement and strain. 
An example of the tensile strain field is shown in Figure 7 alongside the stress versus strain plot obtained after post-processing the load and strain data.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i9.png" alt="EDAM systems" width="90%">
<figcaption>Fig. 5 - Tension testing setup with DIC and MTS</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj4/i12.png" alt="EDAM systems" width="90%">
<figcaption>Fig. 6 - Shear testing setup with DIC and MTS</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj4/i13.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 7 - DIC computed strain field for tension specimen (left) and material behavior (right)</figcaption>
</figure>


<p style="text-align:left"><strong>Thermomechanical Properties</strong></p>
<p style="text-align:justify">
The coefficient of thermal expansion (CTE) measures the rate of strain with respect to temperature.
For printed fiber reinforced polymers, this rate also depends on the orientation of the sample, and generally has three distinct values.
Namely, along the print direction, in-plane transverse direction, and stacking direction.
To measure this rate, a sample is placed within a heated chamber, the sample is speckled with dots so that it can be tracked to obtain strain measurements with DIC.
The experimental setup is shown in Figure 8, as the temperature increases, the strain is simultaneously measured. 
After post-processing this information, we can obtain the coefficient of thermal expansion for all materials along all three principal print directions.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i14.png" alt="EDAM systems" width="90%">
<figcaption>Fig. 8 - Coefficient of thermal expansion experimental setup</figcaption>
</figure>
<p style="text-align:left"><strong>Thermoviscoelastic Properties</strong></p>
<p style="text-align:justify">
The thermoviscoelastic properties are obtained by using a DMA instrument as shown earlier.
Three-point bending samples were prepared within the dimensional specifications the instrument allows.
Stress relaxation experiments are performed, and each experiment yields a temporal modulus at an predetermined isothermal temperature.
The reference temperature is commonly taken at the glass transition temperature, this reference temperature is used for constructing the master curve.
The master curve behavior is a composition of the temporal modulus, shifted to generate a continuous curve to which a Prony series or generalized Maxwell model can be fitted.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i15.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 9 - Temporal modulus (left) and generated master curve (right)</figcaption>
</figure>
<p style="text-align:left"><strong>Micromechanics</strong></p>
<p style="text-align:justify">
Micromechanical tools are leveraged to reduce the number of mechanical tests and save on experimental costs.
Micromechanics models, Mori-Tanaka method, requires micro-constituent properties and micro-morphological characteristics.
Homogenous properties determined from tensile and shear tests are used for reverse engineering polymer micro-constituent properties and fibe orientation values.
The polymer is complex, often a blend of polymers and additives to tailor the properties for additive manufacturing, this complexity tends to deviate the mechanical properties of the polymer from its base property and reverse engineering allows for determination of these properties without incurring additional experimental costs.
The model allows us to obtain at least 5 elastic constants out of the 9 orthotropic material elastic constants required for the composite.
</p>
<h6 style="text-align:left">Validation Exercise</h6>
<p style="text-align:justify">
The conceptual model developed is a curved wedge, which represents the type of geometric complexity found in EDAM designs.
Moreover, the curved wedge geometry is designed using computer aided design (CAD) software, then transferred to a slicer software to convert the 3D model into layers with machine coordinates (gcode) to be interpreted by the printer.
The mathematical models included for validation are heat transfer, polymer kinetics, and conservation of momentum. 
Furthermore, the mathematical model is implemented using the finite element method in Abaqus/Standard with user-defined subroutines coded in Fortran. 
Pre-test calculations are performed to predict the temperature history and deformations as shown in Figure 10 and 11.
The results are then compared to the printed geometry to quantitatively compare and determine if agreement between both outcomes are acceptable.
</p>
<figure>
<img src="/assets/img/portfolio/proj4/i17.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 9 - Simulated print geometry with line path superimposed to extract time-temperature history (top), and time-temperature history plot (bottom)</figcaption>
</figure>
<figure>
<img src="/assets/img/portfolio/proj4/i18.png" alt="EDAM systems" width="80%">
<figcaption>Fig. 9 - Snapshot of the curve wedge experiment being printed (top) and finite element simulation to predict deformations (bottom)</figcaption>
</figure>
<figure>
<img src="/assets/img/portfolio/proj4/i22.png" alt="EDAM systems" width="100%">
<figcaption>Fig. 10 - Curved wedge geometry for LSAM print</figcaption>
</figure>
<video width="100%" autoplay muted loop>
  <source src="/assets/img/portfolio/proj4/Media2.mp4" type="video/mp4">
Your browser does not support the video tag.
</video><br>
<h6 style="text-align:left">Accomplishments</h6>
<p style="text-align:justify">
In this project, three material cards were successfully characterized, and the simulation framework was demonstrated as a viable tool to predict internal residual stresses, deformations, and relevant state variables on 3D printed geometries.
The material cards generated in this project has enabled simulating the printing process for three new material systems, and mitigates the empirical process of wasteful design iterations to obtain desired shape.
</p>
<h6 style="text-align:left">References</h6>
<ol style="text-align:justify;margin-left:30px">
<li>E. Barocio, V. Kapre, P. Pibulchinda, M. A. Ramirez, A. Franc, and J. Susnjara, “Material Characterization for Large Scale Additive Manufacturing (AM),” Institute for Advanced Composites Manufacturing Innovation, Knoxville, TN, PA16-0349-7.6–01, May 2022. [Online]. Available: <a href="https://iacmi.org/wp-content/uploads/2022/05/IACMI-7.6-Final-Project-Report-5-5-22-APPROVED.pdf">IACMI</a></li>
</ol>