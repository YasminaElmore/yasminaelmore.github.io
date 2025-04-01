---
layout: yasmina_default
title: "Simulating Interactions between a Shock and a Perturbed Gas Cylinder using CFD"
date: 2023-08-01
description: Verification and validation a CFD code. Study on vortex dipole formation in supernovae, resulting in a co-authored publication in Physics of Plasmas
---

<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/sketch.png" alt="shockperturbgas" style="width:30%; object-fit:cover; border-radius:10px;">
</div>

This project was conducted at the Scientific Computing and Flow Physics Laboratory at the University of Michigan and led to my co-authorship of the paper <a href="https://pubs.aip.org/aip/pop/article/31/6/062103/3298197"> Feasibility of an Experiment on Clumping Induced by the Crow Instability Along a Shocked Cylinder</a>, published in Physics of Plasmas. The goal was to validate and verify a patch-based adaptative mesh refinement CFD code developed in the lab and to study the physical phenomena leading to the formation of vortex dipoles in supernovae by reviewing the literature and analyzing simulation data.

# Role and Contribution 

<ul>
    <li>Conducted numerical simulations to analyze vortex ring dynamics using a <strong>C++-based Navier-Stokes solver</strong> with <strong>Adaptive Mesh Refinement (AMR)</strong>.</li>
    <li>Developed a personal methodology for the <strong>verification and validation</strong> of <strong>PATCH-based AMR</strong> and tested it on the lab’s numerical solver.</li>
        <li>Verified and validated the lab-developed solver by comparing numerical results with theoretical reference models.</li>
    <li>Optimized mesh resolution to balance data accuracy and computational efficiency, achieving a refined resolution of <strong>r = 512</strong> for reliable vortex evolution analysis.</li>
    <li>Investigated the evolution of <strong>circulation deposition</strong> on a shocked gas cylinder by examining the impact of <strong>Mach number, density ratio, and time.</strong></li>
    <li>Identified the influence of <strong>misalignment between pressure and density gradients</strong> on circulation growth rates after shock interaction.</li>
    <li>Analyzed <strong>2D geometrical parameters</strong> of the vortex dipole by defining vortex regions using the <strong>Q-criterion</strong> and tracking the evolution of key geometric properties.</li>
    <li>Discovered trends in vortex core spacing and size variations based on shock strength and density ratios, contributing to the understanding of <strong>vortex formation in supernova remnants.</strong></li>
    <li>Reviewed and compared existing <strong>literature models</strong> (Haas & Sturtevant, Samtaney & Zabusky), identifying limitations and proposing refinements based on simulation findings.</li>
</ul>

<h3>Methodology for Verification and Validation of PATCH-Based AMR</h3>
<ol>
    <li><strong>Selection of refinement indicators:</strong> Determined refinement criteria based on simulation parameters.</li>
    <li><strong>Choice of reference model:</strong> Identified a theoretical model to define an optimal mesh resolution.</li>
    <li><strong>Comparison of mesh results:</strong> Analyzed simulation results across different mesh resolutions against the reference model.</li>
    <li><strong>Verification step:</strong> Ensured algorithmic convergence by evaluating numerical consistency.</li>
    <li><strong>Validation step:</strong> Selected a second reference model and compared its results with simulation data to confirm the solver’s accuracy.</li>
</ol>

<br>
<strong> Comparison between a properly defined mesh refinement and an incorrect one.</strong>

<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/example of choice of mesh.png" alt="shockperturbgas" style="width:75%; object-fit:cover; border-radius:10px;">
</div>

<br>
<strong> CFD simulation of the interaction</strong>


<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/simluations2.png" alt="shockperturbgas" style="width:75%; object-fit:cover; border-radius:10px;">
</div>


# Skills developped 

Verification and Validation of code, PATCH-based AMR, fluid dynamics, MATLAB for data representation, Computational Fluid Dynamics (CFD), Simulations, Shock wave, Vortex dipole, Circulation, Q-criterion

# Project images 

### Sketch representing the interation between the shock and the interface at a small scale and equation estimating the approximation of the circulation generated at the interface: 

<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/samtaney_zab.png" alt="magniseffectlift" style="width:50%; object-fit:cover; border-radius:10px;">
</div>
<br>

<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/expression.png" alt="magniseffectlift" style="width:50%; object-fit:cover; border-radius:10px;">
</div>
<br>

### Plot showing the strong correlation between the reference value obtained by using Samtaney and Zabusky equation and the simulations values obtained by data exploitation 

<div style="text-align: center;">
    <img src="/assets/projects/shockperturbgas/data_circulation.png" alt="magniseffectlift" style="width:50%; object-fit:cover; border-radius:10px;">
</div>

# Abstract

The interaction between a gas cylinder and a shock wave has been subject to studies in the literature and
has often appeared in a couple of problems in physics. It has been proved that the shock wave passing through
a cylinder leads to a deformation of the latter, forming a vortex dipole. In this project, we start by studying
the interaction by looking at the evolution of circulation deposition around the cylinder during and mostly
after the shock passage. We show that the circulation increases even after the shock passage, and the slope of
this increase grows with the Mach number. We point out that the reason for the increase in slopes is linked
to the misalignment between the pressure gradient and the density gradient. Secondly, we study the impact of
the shock on the cylinder’s geometry by looking at the distance between the two vortices of the formed dipole
and their size. We pointed out that the growth of the Mach number or the reduction of the ratio of density
between the cylinder and the ambient gas leads to a decrease in the distance between the two vortices. This
study was realized through simulations based on adaptive mesh refinement. 

# Report

Final Report:

<iframe src="/assets/projects/shockperturbgas/PROJET_PRE (18).pdf" width="100%" height="600px"></iframe>