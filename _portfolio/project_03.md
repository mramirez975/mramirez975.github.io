---
title: Viscoelastic Damage Mechanics<hr>
subtitle: 
image: assets/img/portfolio/proj3/p2.png
alt: 

caption:
  title: Viscoelastic Damage Mechanics
  subtitle: Research/Simulation
  thumbnail: assets/img/portfolio/proj3/p1.png
---
<p style="text-align:justify">
<strong>Highlights</strong>:<br>
<ul style="text-align:left;margin-left:30px">
	<li>Developed novel thermoviscoelastic damage model derived from thermodynamic principles with temperature-dependent behavior</li>
	<li>Implemented mathematical damage model as a user material subroutine (UMAT) for Abaqus/Standard (Implicit) using Fortran coding</li>
	<li>Conducted mechanical and viscoelastic experiments to characterized 3D printed composite material in ambient and elevated temperature environments</li>
	<li>Verified material model and provided insight in material model parameters and their sensitity to nonlinear behavior</li>
	<li>Validated material model by comparing the damage and failure of 3D printed composite u-shaped mold to simulated results</li>
	<li>Demonstrated the viability of accounting for damage and failure in 3D printed composites without significant computational expense penalties</li>
</ul>
</p>
<h6 style="text-align:left">Modeling Viscoelastic Damage in Extrusion Deposition Additive Manufacturing</h6>
<h6 style="text-align:left">Introduction</h6>
<p style="text-align:justify">
During the last decade, major breakthroughs in extrusion deposition additive manufacturing (abbreviated as EDAM) have been made. 
These breakthroughs are in printing of large-scale fiber reinforced polymer composite structures in a cost-effective way and in a short amount of time. 
Some of the types of structures that have been printed are also shown here: 
<ul style="text-align:left;margin-left:30px">
	<li>On the  left image, a molding tool for fabricating a section of a fuselage is shown. This was printed on the LSAM system.</li>
	<li>At the  center, a submarine hull is shown and this was printed on a BAAM for dive technologies </li>
	<li>Lastly, the Al Davis memorial torch in the Las Vegas Raiders stadium was printed using an LSAM</li>
</ul>
</p>
<p style="text-align:justify">
The application of this technology have demonstrated promising potential for molding or tooling, end-use parts, or for quickly prototyping or creating artistic structures
Despite these technological advances, analysis tools (to support process design and in-service application of 3D printed components) remain largely underdeveloped. This leads to trial-and-error (empirical) approach to manufacturing - that’s time and cost inefficient, this slows down a wider technology use. Example: when the raw material cost is $10-30/pound (high-end polymers), and you need to print a 500lb piece, the cost of trial-and-error becomes unacceptable
</p>

<figure>
<img src="/assets/img/portfolio/proj3/i1.png" alt="" width="100%">
<figcaption>Fig. 1 - 3D printed composite fuselage skin mold (left), 3D printed composite submersible hull (center), and 3D printed torch design (right)</figcaption>
</figure>

<p style="text-align:justify">
On the bottom left of Figure 2, we are looking at a typical feedstock used for printing, these are short fiber reinforced polymer pellets. These pellets contain fibers, voids, and a complex thermoplastic polymer
The question that naturally arises is: why use composite feedstock and not just the bulk polymer for printing? - this is because composite feedstock improve effective mechanical properties, such as stiffness and strength; the coefficient of thermal expansion along the print direction is significantly reduced, and this reduces the part warpage during print, this is what is shown on the right-hand image. Lastly, the neat polymer’s thermal conductivity is very low (compared to metals) - but when carbon fibers are used, the effective in-plane thermal conductivity is improved which can be beneficial for certain applications that require quick heating or cooling.
<ul style="text-align:left;margin-left:30px">
	<li>Adding fibers to a viscoelastic polymer produces a composite with anisotropic response that can invoke complex damage scenarios</li>
	<li>One scenario is illustrated in the case of a printed car made from CF/ABS where certain sections of the print has delaminated (see Figure 3). This shows that the stresses of printed parts during or post processing can indeed exceed the material strength. Efficiency is a key theme in the use of additive manufacturing; therefore, re-printing of structures in the hopes of printing a successful part defeats the purpose of the additive approach</li>
</ul>
</p>
<p style="text-align:justify">
With this in mind, the aim here is to develop a modeling tool that can predict in-manufacturing and in-service anisotropic damage development
</p>

<figure>
<img src="/assets/img/portfolio/proj3/g1.gif" alt="" width="100%">
<figcaption style="margin-top:-125px;margin-bottom:25px;">Fig. 2 - Illustration of feedstock used for 3D printing composites</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i2.png" alt="" width="100%">
<figcaption>Fig. 3 - Cracking of 3D printed composite car (left) and wall (right) due to long layer times, demonstrating the need for predictive tools</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i3.png" alt="" width="100%">
<figcaption>Fig. 4 - Print direction classification (top) and bead microscale morphological representation (bottom)</figcaption>
</figure>

<h6 style="text-align:left">Modeling background</h6>
<p style="text-align:justify">
The stress-strain curve is represented by the damage-informed hereditary integral shown here. 
The hereditary integral accounts for any prior deformation history, this influences the current stress state.
The time-dependent stiffness shown has an equilibrated part and un-relaxed part.
This integral includes damage through these so-called damage effect tensors that described the time-dependent stiffness state or how much softening has occurred.
Thermodynamic consistency is derived from the first and second laws of thermodynamics, it is a dissipation inequality, known as the Clausius-Duhem inequality, which material states must obey. 
The dissipation potentials are obtained from this inequality.
</p>

<figure>
<img src="/assets/img/portfolio/proj3/g2.gif" alt="" width="100%">
<figcaption>Fig. 5 - Viscoelastic damage constitutive relation</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/g2b.gif" alt="" width="100%">
<figcaption>Fig. 6 - Damage initiation and evolution formulation</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i4.png" alt="" width="100%">
<figcaption>Fig. 7 - Workflow of experimental methods needed for model calibration</figcaption>
</figure>

<h6 style="text-align:left">Experimentation</h6>
<p style="text-align:justify">
To understand how a printed material performs at elevated temperature, an experimental campaign is carried out to characterize its mechanical behavior.
Tension, compression, and shear deformation modes were studied to understand printed viscoelastic material stress-strain behavior.
Figure 8 illustrates the composite additive manufacturing research instrument used for 3D printing composite parts, to then extract mechanical and viscoelastic specimens.
Figure 9 illustrates the 3D printed parts used for extracting the samples, and the experimental setup to test for properties at room and elevated temperatures.
Figure 10 & 11 illustrates the time-dependent behavior of the 3D printed material, which is imperative for planning mechanical tests.
In other words, we must not allow the specimen to relax its stress state by more than 5% during the time-span of the test; otherwise, the nonlinear behavior becomes more complex.
Figure 11 shows us that at higher temperatures, the stresses relax substantially and most mechanical tests should be conducted in under 5 minutes.
Figure 12 & 13 shows us the shift factors used for characterizing the viscoelastic portion of the model, and its correlation to experiments.
Figure 14 - 16 present some of the results obtained during the experimental campaign. 
</p>

<figure>
<img src="/assets/img/portfolio/proj3/i5.png" alt="" width="100%">
<figcaption>Fig. 8 - Illustration of composites additive manufacturing research instrument used for printing parts and specimens</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i6.png" alt="" width="100%">
<figcaption>Fig. 9 - illustration of 3D printed parts used for extracting mechanical and viscoelastic specimens (top), mechanical experimental setup</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i7.png" alt="" width="100%">
<figcaption>Fig. 10 - Viscoelastic master curves obtained from dynamic mechanical analyzer (DMA)</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i8.png" alt="" width="65%">
<figcaption>Fig. 11 - Stress relaxation measurements obtained from DMA</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i9.png" alt="" width="75%">
<figcaption>Fig. 12 - Shift factors for master curves for time-temperature superposition application</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i10.png" alt="" width="100%">
<figcaption>Fig. 13 - Verification of viscoelastic predictions with experiments</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/g3.gif" alt="" width="100%">
<figcaption>Fig. 14 - Tensile performance of additive manufactured material along the print direction, with ASTM methodology shown for extracting tensile properties</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/g4.gif" alt="" width="100%">
<figcaption>Fig. 15 - Tensile performance along the in-plane (2) direction, and the stacking (3) direction, with statistical summary illustrating the decrease in properties with increasing temperature</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/g5.gif" alt="" width="100%">
<figcaption>Fig. 16 - In-plane shear performance with digital image correlation computed surface strain field shown on the right</figcaption>
</figure>

<h6 style="text-align:left">Viscoelastic damage model calibration & verification</h6>
<p style="text-align:justify">
The model is calibrated as shown in Figures 17 & 18, the process involves extracting nonlinear onset from the mechanical tests to solve for the damage surface function and obtain its uniaxial parameter.
The The parameters is plotted against temperature to understand how it varies with temperature and include it in the model.
The evolution parameters can be obtained by solving for the exponential function, which requires knowledge or estimation of the damage evolution quantity as a function of temperature.
Figure 19 illustrates the verification conducted to ensure the viscoelastic model works as intended, and to understand the significance of the parameters involved in the model. 
</p>

<figure>
<img src="/assets/img/portfolio/proj3/i11.png" alt="" width="100%">
<figcaption>Fig. 17 - Procedure for determining parameters of the temperature-dependent damage surface function</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i12.png" alt="" width="100%">
<figcaption>Fig. 18 - Determining the temperature-dependent parameters of the isotropic hardening/softening function</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i13.png" alt="" width="100%">
<figcaption>Fig. 19 - Verification of viscoelastic damage model demonstrating model parameter influence</figcaption>
</figure>

<h6 style="text-align:left">Damage model validation</h6>
<p style="text-align:justify">
The following figures show the comparison between the viscoelastic model and the experiments, at various temperatures. 
The model is capable of representing tensile behavior along all three principal print directions; moreover, the unilateral behavior can be observed by the model in compression.
Comparisons can be seen in Figures 20 - 22.
The model is validated by conceptualizing a u-shaped tool that is pressed along its vertical axis, this tool is subjected to compressive loads, while some of the infill features experience tensile stresses.
Damage is predicted at the sites shown in darker color, which represent regions where the damage variable indicator is greater than zero. 
As compared to the experiment, the predicted damage site is where the tool fails under this deformation mode.
</p>

<figure>
<img src="/assets/img/portfolio/proj3/i14.png" alt="" width="100%">
<figcaption>Fig. 20 - Comparison of model and experiment for tension and compression along the print (1) direction</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i15.png" alt="" width="100%">
<figcaption>Fig. 21 - Comparison of model and experiment for tension and compression along the in-plane transverse (2) direction</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i16.png" alt="" width="100%">
<figcaption>Fig. 22 - Comparison of model and experiment for tension and compression along the stacking (3) direction</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/g6.gif" alt="" width="100%">
<figcaption>Fig. 23 - Conceptual design of u-shaped mold used for 3D print compression experiment</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i17.png" alt="" width="100%">
<figcaption>Fig. 24 - Non-isothermal prediction of tool transferred to press, load-displacement prediction, and predicted damage sites</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj3/i18.png" alt="" width="100%">
<figcaption>Fig. 25 - Prediction of damage locations of 3D printed u-shaped tool, which agrees with experiment</figcaption>
</figure>

