---
title: Short Fiber Composite Micromechanics<hr>
subtitle: 
image: assets/img/portfolio/proj6/p1.png
alt: 

caption:
  title: Short Fiber Composite Micromechanics
  subtitle: Research/Simulation
  thumbnail: assets/img/portfolio/proj6/g3.gif
---
<h6 style="text-align:left">Introduction</h6>
<p style="text-align:justify">
Discontinuous fiber reinforced polymers provide ease of manufacturing complex geometries at the penalty of strength and stiffness compared to traditional laminates.
However, the specific stiffness and strength are appealing in industries that benefit from lightweight alternative materials such as aerospace and automotive.
The use of short fiber reinforced polymers requires detailed characterization of their material properties, and an understanding of damage modes and fracture behavior.
For manufacturing processes such as additive manufacturing, detailed characterization data is limited in literature.
The scope of this project was to develop a finite element micromechanical model capable of predicting mechanical properties of discontinuous composites.
</p>
<p style="text-align:justify">
<strong>Highlights</strong>:<br>
<ul style="text-align:left;margin-left:30px">
	<li>Extracted micro-constituent properties of composites from literature</li>
	<li>Conducted experiments to characterized short fiber composite microstructure and studied its morphology</li>
	<li>Developed a finite element micromechanics model using Digimat for model creation and Abaqus for material modeling</li>
	<li>Developed a framework for using morphological features and micro-constituent data to inform micromechanical model</li>
	<li>Verified micromechanical model by conducting several simulation trials to check for consistent behavior between load-bearing loss and crack propagation</li>
	<li>Validated micromechanical model by conducting uniaxial tensile tests of 3D printed composite and comparing the results of experiments to model</li>
</ul>
</p>

<h6 style="text-align:left">Introduction</h6>
<figure>
<img src="/assets/img/portfolio/proj6/i1.png" alt="" width="100%">
<figcaption>Fig. 1 - (a) Processing of feedstock through an extruder and extrusion deposition of printed beads compacted by a tamper; 
(b) Reference coordinate system adopted in EDAM bead(s)</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i2.png" alt="" width="100%">
<figcaption>Fig. 2 - Multiscale nature of additively manufactured short fiber composite</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i3.png" alt="" width="100%">
<figcaption>Fig. 3 - Analysis methods for short fiber composites with direct numerical analysis highlight for emphasis on desireable method</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i4.png" alt="" width="100%">
<figcaption>Fig. 4 - Illustration of stress strain behavior with key segments illustrated to show evolution of damage correlated to nonlinear stress-strain behavior</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i5.png" alt="" width="100%">
<figcaption>Fig. 5 - Depiction of combination of parameters that can be varied to show the impracticality of studying each variable through experimentation and show the need for modeling</figcaption>
</figure>

<h6 style="text-align:left">Experimentation</h6>

<video width="100%" autoplay muted loop>
  <source src="/assets/img/portfolio/proj6/m1.mp4" type="video/mp4">
Your browser does not support the video tag.
</video><br>
<figcaption style="margin-top:-50px;margin-bottom:25px">Vid. 1 - Process for extrusion deposition additive manufacturing of short fiber reinforced polymer parts</figcaption>

<figure>
<img src="/assets/img/portfolio/proj6/i6.png" alt="" width="100%">
<figcaption>Fig. 6 - Fibers extracted from matrix carbonization process (schematic) and fibers
dispersed over a glass slide (image from an optical microscope)</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i7.png" alt="" width="100%">
<figcaption>Fig. 7 - Microstructure region of interest (ROI) with thresholding of fibers and voids</figcaption>
</figure>

<h6 style="text-align:left">Experimentation</h6>
<p style="text-align:justify">
</p>

<figure>
<img src="/assets/img/portfolio/proj6/i8.png" alt="" width="100%">
<figcaption>Fig. 8 - ROIs for orientation analysis and measurement of local fiber orientations</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i9.png" alt="" width="100%">
<figcaption>Fig. 9 - Distribution of elliptic void major and minor axes measurements</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i10.png" alt="" width="100%">
<figcaption>Fig. 10 - Tensile coupon in hydraulic grips of an MTS and pre- and post-mortem of a
tensile coupon</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i11.png" alt="" width="100%">
<figcaption>Fig. 11 - DIC-measured surface strain fields and stress-strain plot for SFC</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i12.png" alt="" width="100%">
<figcaption>Fig. 12 - SEM images of the carbon fiber reinforced polycarbonate fracture surface with
fibers standing out from the cracked matrix surface</figcaption>
</figure>

<h6 style="text-align:left">Development of micromechanical model</h6>

<figure>
<img src="/assets/img/portfolio/proj6/i13.png" alt="" width="100%">
<figcaption>Fig. 13 - Preprocessing workflow step for generating a digital micro-structure of an additively
manufactured short fiber composite</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i14.png" alt="" width="100%">
<figcaption>Fig. 14 - Computational workflow from generating a meshed digital microstructure to solving
the analysis for obtaining the homogenized mechanical properties of the additively manufactured
short fiber composite</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i15.png" alt="" width="100%">
<figcaption>Fig. 15 - Representation of micro-structure of SFC from a unit cell forming a periodic structure</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/g1.gif" alt="" width="100%">
<figcaption>Fig. 16 - Inclusion of microstructural variables obtained from morphology experiments into micromechanical finite element model</figcaption>
</figure>

<h6 style="text-align:left">Viscoelastic damage model calibration & verification</h6>
<p style="text-align:justify">

</p>

<figure>
<img src="/assets/img/portfolio/proj6/g2.gif" alt="" width="100%">
<figcaption>Fig. 17 - Brief overview of random sequential adsorption algorithm used for fiber generation and placement within representative volume element</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i16.png" alt="" width="100%">
<figcaption>Fig. 18 - Finite element conformal mesh used for micromechanics model with extended finite element method (XFEM) and cohesive zone modeling (CZM) included</figcaption>
</figure>

<h6 style="text-align:left">Micromechanical model verification & validation</h6>

<figure>
<img src="/assets/img/portfolio/proj6/i17.png" alt="" width="100%">
<figcaption>Fig. 19 - Illustration of interfacial disbonding in a fiber within the RVE, red indicates the scalar
damage variable has reached a value of 1.0, and the fiber is disbonded from the matrix</figcaption>
</figure>

<h6 style="text-align:left">Damage model validation</h6>
<p style="text-align:justify">

</p>

<figure>
<img src="/assets/img/portfolio/proj6/g3.gif" alt="" width="100%">
<figcaption>Fig. 20 - Illustration of crack initiation and evolution of SFC as homogenized stress and strain evolves</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i18.png" alt="" width="100%">
<figcaption>Fig. 21 - Homogenized stress vs strain response for an RVE, and progression of damage
within RVE at three locations within the homogenized stress strain plot</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i19.png" alt="" width="100%">
<figcaption>Fig. 22 - Comparison between effective stiffness and ultimate strength of two RVE with
different morphological characteristics</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i20.png" alt="" width="100%">
<figcaption>Fig. 23 - Stochastic tensile properties of a short fiber composite: simulated and experimental</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i21.png" alt="" width="100%">
<figcaption>Fig. 24 - Selected fracture topology for virtually tested micro samples</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i22.png" alt="" width="100%">
<figcaption>Fig. 25 - Stress field of solely the matrix in two separate RVEs with different stochastic
morphologies, the contour plot indicates the level of stress concentration or localized stress
normalized to the homogenized stress</figcaption>
</figure>

<figure>
<img src="/assets/img/portfolio/proj6/i23.png" alt="" width="100%">
<figcaption>Fig. 26 - Observation of the fractured surface topology in the experimental tensile coupon and
comparison between experimental fracture topology and digital fracture topology</figcaption>
</figure>


