---
layout: page
title: Projects
permalink: /projects/
mathjax: true
---

## Selected projects

### ZeoNet

Using convolutional neural networks on volumetric data to predict adsorption properties in nanoporous materials. Published in Journal of Materials Chemisty A. Main contributions come from Yachan Liu and Gustavo Perez. I contributed to the earlier stages of this project, developing the training and inference framework and finding that simple geometric descriptors cannot reliably predict adsorption properties.
<p align="center">
  <img src="/assets/projects/imgs/saliency-maps.png" width="95%" />
</p>

<a href="https://pubs.rsc.org/en/content/articlelanding/2023/ta/d3ta01911j">Check out the paper!</a>

### Spinodal decomposition via Cahn-Hilliard equation

Simple Python script for solving the <a href="https://en.wikipedia.org/wiki/Cahn–Hilliard_equation">Cahn-Hilliard equation</a> using the Forward Euler method. The animation on the left is for a 50/50 mixture of two phases while the right is a 30/70 mixture. For imbalanced mixtures such as the one on the right, <a href="https://en.wikipedia.org/wiki/Ostwald_ripening">Ostwald ripening</a> can occur. The lesser phase develops into spherical droplets and coalesces over time.

<p align="center">
  <img src="/assets/projects/gifs/spinodal-decomposition_D-100_gamma-0.5_p-0.gif" width="47%" />
  <img src="/assets/projects/gifs/spinodal-decomposition_D-100_gamma-0.5_p-0.4.gif" width="47%" />
</p>

<a href="https://github.com/samuelhoover/spinodal-decomposition">Check out the repo!</a>

---

## Ongoing work

### Unraveling sequence effects on charged heteropolymer phase behavior using SHAP values

Using gradient boosted decision trees and SHAP values to determine the effect of monomer sequence on the assembly of charged heteropolymers.

<p align="left">
  <img src="/assets/projects/imgs/Nchi_v2-vs-eta.svg" width="95%" />
</p>
<p align="center">
  <img src="/assets/projects/imgs/best_parity_plot.png" width="95%" />
</p>

### Phase behavior of polyzwitterion-polyelectrolyte complex coacervates

Developing theory to investigate the effects of a dynamic pH environment on the phase stability of polyzwitterion-polyelectrolyte complex coacervates.

<p align="center">
  <img src="/assets/projects/imgs/4-states_v4.png" width="95%" />
</p>
<p align="center">
  <img src="/assets/projects/imgs/example-pZ.png" width="95%" />
</p>
<p align="center">
  <img src="/assets/projects/imgs/system-schematic.png" width="95%" />
</p>

---

## Other projects

### Phase behavior of chains of dipoles

Generated phase diagrams from multidimensional free energy minimzation calculations to investigate the phase behavior of chains of dipoles and the influence of dipolar electrostatic interactions in complex coacervation. The free energy density expression we used can seen below,

$$ f = \frac{\phi_{p}}{N} \ln \phi_{p} + \phi_{s} \ln \left( \frac{\phi_{s}}{2} \right) + \phi_{0} \ln \phi_{0} + \frac{1}{2} v_{dd} \left( \frac{\phi_{p}}{2} \right)^{2} + \chi \phi_{p} \phi_{0} - \frac{1}{4 \pi} \left[ \ln (1 + \kappa \ell) - \kappa \ell + \frac{1}{2}(\kappa \ell)^{2} \right] $$

where $$\phi_{p}$$, $$\phi_{s}$$, and $$\phi_{0}$$ are the volume fractions of the polymer (chains of dipoles), salt, and solvent. The first three terms describe the mixing entropy. The fourth term describes the electrostatic contributions arising from dipolar interactions within and without each chain. The fifth term describes excluded volume contributions (hydrophobic effects if your solvent is water) between the polymer and solvent segments. The sixth and final term describes the electrostatic energy of correlations of ions.

### Forcefield development for small organic molecules

Computed <a href="https://doi.org/10.1021/acs.jctc.5b00864">OPLS3 forcefield</a> torsional parameters for trihalomethane (THM) molecules. THMs are disinfection by-products found in drinking water supplies as a result of the chlorination treatment. They are considered environmental pollutants and are possible carcinogens.
