---
layout: default
title: Projects
permalink: projects/
---

## Ongoing work

### Unraveling sequence effects on copolymer phase behavior using SHAP values

Using gradient-boosted decision trees and SHAP values to determine the effect
of monomer sequence on the phase behavior of sequence-defined charged polymers.
<p align="center">
  <img
    src="/projects/assets/imgs/Nchi-vs-eta.pdf"
    alt="Ongoing work"
    width="80%"
  />
</p>

---

## Selected projects

### Phase behavior of polyzwitterion-polyelectrolyte complex coacervates

Developed theory to investigate the effects of a dynamic pH environment on the
phase stability of polyzwitterion-polyelectrolyte complex coacervates.
Validated earlier hypothesis on the switching between charge-dipole and
dipole-dipole electrostatic interactions as the determining factor for
coacervate stability.
<p align="center">
  <img
    src="/projects/assets/imgs/system-schematic.pdf"
    alt="System schematic"
    width="80%"
  />
</p>

[Check out the paper!](https://pubs.rsc.org/en/content/articlelanding/2024/sm/d4sm00575a)

### ZeoNet

Applied convolutional neural networks on volumetric data to predict adsorption
properties in nanoporous materials. Published in *Journal of Materials
Chemistry A*. I developed the pipelines and learning framework. I also found
that simple geometric descriptors cannot reliably predict adsorption properties
and that more rich data is needed.
<p align="center">
  <img
    src="/projects/assets/imgs/saliency-maps.png"
    alt="Saliency map from last layer of convolutional neural network"
    width="80%"
  />
</p>

[Check out the paper!](https://pubs.rsc.org/en/content/articlelanding/2023/ta/d3ta01911j)

### Monte Carlo suite

The [Monte Carlo method](https://en.wikipedia.org/wiki/Monte_Carlo_method) is a
straightforward and useful technique when analytical solutions are nonexistent
or difficult to compute. Below are two particularly important cases for the
physical sciences. You can find more examples, implemented in Rust, in this
[repository](https://github.com/samuelhoover/rusty-monte-carlo). I find
implementing these examples to be helpful when learning a new language or
numerical computing beginners as they cover the basics of arithmetic, looping,
(pseudo)random number generators, slicing/indexing, *etc*.

#### 2D Ising model

4 million element 2D array, 1 billion steps, 6 seconds, in Rust. Employed integer
calculation and numerical tricks for improved computational efficiency. The
[Ising model](https://en.wikipedia.org/wiki/Ising_model) is important to a
variety of scientific fields, namely for the study of spin glasses in
statistical mechanics.

| Initial lattice | Final lattice|
| -- | -- |
| ![Input lattice](/projects/assets/imgs/t_0.png) | ![Final lattice](/projects/assets/imgs/t_1e9.png) |

[(repo)](https://github.com/samuelhoover/ising-rust)

#### Percolation threshold estimation

There is no solution for determining the exact [percolation
threshold](https://en.wikipedia.org/wiki/Percolation_threshold) limit, the
fraction of open sites to closed sites that are required for one cluster to be
connected to opposite ends (top to bottom, left to right) of a lattice. One
can use the Monte Carlo method to randomly open lattice sites until percolation
occurs. Running many trials and with a large enough lattice should warrant an
estimated percolation threshold limit of around 0.593.

Below, black squares represent closed sites, blue for open sites, and green for
the percolated cluster.
<p align="center">
  <img
    src="/projects/assets/imgs/percolated_array.png"
    alt="Percolated array"
    width="40%"
  />
</p>

[(repo)](https://github.com/samuelhoover/percolation)

### Spinodal decomposition

Simple Python script for solving the
[Cahn-Hilliard](https://en.wikipedia.org/wiki/Cahn–Hilliard_equation) equation
using the Forward Euler method. [Spinodal
decomposition](https://en.wikipedia.org/wiki/Spinodal_decomposition) occurs in
thermodynamically unstable mixtures, with the mixture spontaneously decomposing
into two phases. In the case of unequal mixtures (*e.g.* 70/30 mixture on the
right), [Ostwald ripening](https://en.wikipedia.org/wiki/Ostwald_ripening)
occurs where droplets of the lesser phase coalesce into progressively larger
droplets. Eventually, one should expect both scenarios (50/50 and 70/30
mixtures) to undergo macrophase separation into two bulk phases.

| 50/50 mixture | 70/30 mixture |
| -- | --|
| ![50/50 mixture](/projects/assets/gifs/spinodal-decomposition_D-100_gamma-0.5_p-0.gif) | ![70/30 mixture](/projects/assets/gifs/spinodal-decomposition_D-100_gamma-0.5_p-0.4.gif) |

[(repo)](https://github.com/samuelhoover/spinodal-decomposition)

### Molecular dynamics

Molecular dynamics simulations of protein-ligand binding, biomolecules,
heterogeneous systems, and polymer systems.
<p align="center">
  <img
    src="/projects/assets/imgs/complex.png"
    alt="Protein-ligand complexation using GROMACS"
    width="40%"
  />
  <img
    src="/projects/assets/imgs/heterogeneous.png"
    alt="Protein in a biphasic system"
    width="40%"
  />
</p>
<p align="center">
  <img
    src="/projects/assets/imgs/free_energy.png"
    alt="Solvation energy calculation"
    width="80%"
  />
</p>

[(repo)](https://github.com/samuelhoover/gromacs-tutorials)

### ChE Senior Lab peer critique automation script

(Nearly) Pure Python script to automate some of the tedious work of a Teaching
Assistant for ChE Senior Lab at UMass Amherst. Automatically handles the peer
feedback forms: anonymizing, aggregating based on presenter, and then
distributing *via* email. Saved 8 hours over the course of the semester and
allowed me to focus on the important things. Only requires
[pandas](https://pandas.pydata.org) and
[openpyxl](https://openpyxl.readthedocs.io/en/stable/).

[(repo)](https://github.com/samuelhoover/ChE-401-402-peer-critiques-anonymizer)
