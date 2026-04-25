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

All defects should be considered in their neutral charge state. You may propose an alternative defect system with approval from the course instructor. For structural relaxations you are encouraged to use MACE MP-0. For electronic structure you are encouraged to use DFT with the lcao basis set and gamma-point sampling.

---

## Tasks

### Part 1: Host Material (30 marks)

1. Build the primitive unit cell of your chosen host material using ASE. Print out a summary of the structural properties (crystal structure, space group, and lattice parameters).
2. Create a supercell appropriate for a defect calculation. Justify your choice of supercell size by estimating the distance between periodic defect copies. 
4. Compute the equation of state and extract the equilibrium lattice constant and bulk modulus. Compare to experimental or literature values.
5. Compute the bandstructure for your host material and identify the location of the valence band maximum (VBM) and conduction band minimum (CBM). State whether the bandgap is direct or indirect and explain what this means for optical emission.

### Part 2: Defect System (30 marks)

1. Introduce the defect into your supercell. 
2. Relax the defect supercell geometry and report: (a) the maximum residual force before and after relaxation, (b) displacement of the surrounding atoms as a function of distance from the defect.
3. Compute the bandstructure for your defect system and identify the localised energy level(s) associated with the defect.

### Part 3: Optical Properties — Analysis and Discussion (40 marks, powerpoint walkthrough)

1. Create a simple defect electronic level schematic, showing the host valence band, conduction band, and in-gap defect state(s) for your material. 
1. You used DFT with a relatively small supercell, inexpensive basis functions, course sampling in reciprocal space and the defect is in a neutral charge state — which of these approximations do you think contributes most to any discrepancy with the experimental ZPL?
3. Discuss **two** key challenges for using this system in a real quantum optics device. For each challenge, describe one approach — experimental or computational — that is being pursued to address it. Reference at least **two recent papers** (2015-present) in your answer.

---

## Submission Requirements

### Lab Notebook - group work
- A single Jupyter Notebook (`.ipynb`) with all code, figures, and discussion
- All code cells must be executable
- References formatted consistently

### Video Walkthrough - individual work
- A video walkthrough (up to 5 minutes) highlighting: i) key design decisions; ii) outstanding challenges.

## Assessment Criteria

| Criterion | Marks |
|-----------|-------|
| Correct use of ASE to build and manipulate structures | 25 |
| Quality and clarity of figures | 20 |
| Physical understanding demonstrated in discussion | 30 |
| Engagement with primary literature | 15 |
| Code clarity, comments, and reproducibility | 10 |

---

*Good luck! Computational materials science is a powerful lens for understanding quantum systems, and the skills you develop here are directly transferable to research in quantum technologies.*
