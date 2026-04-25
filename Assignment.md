# Assignment

## Materials Simulation for Quantum and Molecular Optics Assignment

**Format:** Jupyter Notebook submitted via Blackboard.   
**Further Details:** Available on Blackboard.

---

## Overview

This assignment asks you to conduct a computational study of a **solid-state quantum emitter** of your choice from the list below. You will use ASE, DFT and MLIPs to characterise the host material and defect structure and investigate how strain can be used to tune the defect energy level. You will present your findings in a **well-documented** Jupyter Notebook and video walkthrough. 

You will work in small groups to produce the Jupyter Notebook (one notebook per group). All asynchronous discussion and code-sharing must be done through a dedicated Teams channel. 

---

## Choose One System

| System | Host | Defect | ZPL (approx.) |
|--------|------|--------|----------------|
| **A** | Diamond | NV⁻ centre | 637 nm |
| **B** | hBN (monolayer) | Boron vacancy (V_B) | ~800 nm |
| **C** | GaN (wurtzite) | Carbon antisite (C_N) | ~500 nm |
| **D** | AlN | Rare-earth substitutional (Eu³⁺ on Al site) | ~580 nm |
| **E** | SiC (4H polytype) | Divacancy (V_Si V_C) | ~1100 nm |

All defects should be considered in their neutral charge state. You may propose an alternative defect system with approval from the course instructor. For structural relaxations you may use MACE MP-0. For electronic structure calculations you are encouraged to use DFT with the lcao basis set and gamma-point sampling.

---

## Tasks

### Part 1: Host Material (20 marks, jupyter notebook, group work)

1. Build the primitive unit cell of your chosen host material using ASE. Print out a summary of the structural properties (crystal structure, space group, and lattice parameters).
2. Create a supercell appropriate for a defect calculation. Justify your choice of supercell size by estimating the distance between periodic defect copies. 
4. Compute the equation of state and extract the equilibrium lattice constant and bulk modulus. Compare to experimental or literature values.
5. Compute the bandstructure for your host material and identify the location of the valence band maximum (VBM) and conduction band minimum (CBM). State whether the bandgap is direct or indirect and explain what this means for optical emission.

### Part 2: Defect System (20 marks, jupyter notebook, group work)

1. Introduce the defect into your supercell. 
2. Relax the defect supercell geometry and report: (a) the maximum residual force before and after relaxation, (b) displacement of the surrounding atoms as a function of distance from the defect.
3. Compute the bandstructure for your defect system and identify the localised energy level(s) associated with the defect.

### Part 3: Optical Properties — Analysis and Discussion (40 marks, powerpoint walkthrough, individual work)

1. Create a simple defect electronic level schematic, showing the host valence band, conduction band, and in-gap defect state(s) for your material. 
2. You use a number of approximations (e.g. DFT with a relatively small supercell, inexpensive basis functions, course sampling in reciprocal space, a machine-learnt surrogate model), and the defect is in a neutral charge state — which of these approximations do you think contributes most to any discrepancy with the experimental ZPL?

---

## Submission Requirements

### Lab Notebook - group work
- A single Jupyter Notebook (`.ipynb`) with all code, figures, and discussion
- All code cells must be executable
- References formatted consistently

### Video Walkthrough - individual work
- A video walkthrough (up to 5 minutes) 

## Code Quality - marked across both components

| Criterion | Marks |
|-----------|-------|

| Quality and clarity of figures | 10 |
| Code clarity, comments and reproducibility | 10 |

## Headings in mark scheme

- Physical understanding demonstrated in discussion 
- Engagement with primary literature
- Use of ASE for automation

---

*Good luck! Computational materials science is a powerful tool for connecting the microscopic and macroscopic, and the skills you develop here are directly transferable to research in quantum technologies.*
