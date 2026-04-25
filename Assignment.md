# Assignment

## Materials Simulation for Quantum and Molecular Optics Assignment

**Format:** Jupyter Notebook submitted via Blackboard.   
**Further Details:** Available on Blackboard.

---

## Overview

This assignment asks you to conduct a computational study of a **solid-state quantum emitter** of your choice from the list below. You will use ASE, DFT and MLIPs to characterise the host material and defect structure, and present your findings in a **well-documented** Jupyter Notebook and video walkthrough. 

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

You may propose an alternative system with approval from the course instructor.

---

## Tasks

### Part 1: Host Material (30 marks)

1. Build the primitive unit cell of your chosen host material using ASE. Print out the crystal structure, space group, and lattice parameters.
2. Create a supercell appropriate for a defect calculation. Print out the crystal structure, space group, and lattice parameters. Justify your choice of supercell size by estimating the distance between periodic defect copies. 
4. Compute the equation of state and extract the equilibrium lattice constant and bulk modulus. Compare to experimental or literature values.
5. Compute the bandstructure for your host material and identify the location of the valence band maximum (VBM) and conduction band minimum (CBM). State whether the bandgap is direct or indirect and explain what this means for optical emission.

### Part 2: Defect Structure (30 marks)

1. Introduce the defect into your supercell. 
3. Relax the defect supercell geometry and report: (a) the maximum residual force before and after relaxation, (b) the displacement of the nearest-neighbour atoms around the defect.
4. Sketch (or generate computationally) the defect electronic level diagram, showing the host valence band, conduction band, and in-gap defect states. 

### Part 3: Optical Properties — Analysis and Discussion (40 marks)

1. Draw the configuration coordinate diagram for your chosen emitter. Label: ZPL energy, Stokes shift, absorption energy, emission energy, and reorganisation energy. Use literature values if computation is not possible.
2. Explain the physical meaning of the Huang-Rhys factor $S$. Find a published value and comment on whether the ZPL fraction ($\approx e^{-S}$) is favourable for quantum optics applications.
3. Discuss **two** key challenges for using this system in a real quantum optics device. For each challenge, describe one approach — experimental or computational — that is being pursued to address it.
4. Identify **one recent paper** (published 2015–present) that uses computational methods to study this quantum emitter. Summarise the key computational method and result in your own words (200–300 words).

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
