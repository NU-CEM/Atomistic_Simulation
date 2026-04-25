# Assignment

## Materials Simulation Assignment

**Submission deadline:** Please check your course handbook.  
**Weighting:** See course handbook.  
**Format:** Jupyter Notebook submitted via the course portal.

---

## Overview

This assignment asks you to conduct a computational study of a **solid-state quantum emitter** of your choice from the list below. You will use ASE (and a DFT calculator if available to you) to characterise the host material and defect structure, and present your findings in a well-documented Jupyter Notebook.

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

1. Build the primitive unit cell of your chosen host material using ASE. State the crystal structure, space group, and lattice parameters.
2. Create a supercell appropriate for a defect calculation. Justify your choice of supercell size by estimating the minimum image distance between periodic defect copies.
3. Write the structure to both CIF and POSCAR formats. Include both files in your submission.
4. **(If DFT access is available)** Compute the equation of state and extract the equilibrium lattice constant and bulk modulus. Compare to experimental or literature values.
5. Plot the high-symmetry Brillouin zone path for your host material and identify the location of the valence band maximum (VBM) and conduction band minimum (CBM). State whether the bandgap is direct or indirect and explain what this means for optical emission.

### Part 2: Defect Structure (30 marks)

1. Introduce the defect into your supercell (substitution, vacancy creation, or both). Document each step with code and prose.
2. State the point symmetry of the defect complex and identify the symmetry operations.
3. **(If DFT access is available)** Relax the defect supercell geometry and report: (a) the maximum residual force before and after relaxation, (b) the displacement of the nearest-neighbour atoms around the defect.
4. Sketch (or generate computationally) the defect electronic level diagram, showing the host valence band, conduction band, and in-gap defect states. Label the charge state and spin state.

### Part 3: Optical Properties — Analysis and Discussion (40 marks)

1. Draw the configuration coordinate diagram for your chosen emitter. Label: ZPL energy, Stokes shift, absorption energy, emission energy, and reorganisation energy. Use literature values where computation is not available.
2. Explain the physical meaning of the Huang-Rhys factor $S$ for your system. Find a published value and comment on whether the ZPL fraction ($\approx e^{-S}$) is favourable for quantum optics applications.
3. Discuss **two** key challenges for using this system in a real quantum optics device (e.g. collection efficiency, spectral diffusion, dephasing, charge instability). For each challenge, describe one approach — experimental or computational — that is being pursued to address it.
4. Identify **one recent paper** (published 2020–present) that uses computational methods to study this quantum emitter. Summarise the key computational method and result in your own words (200–300 words).

---

## Submission Requirements

- A single Jupyter Notebook (`.ipynb`) with all code, figures, and discussion
- All code cells must be executable (test with "Restart and Run All" before submitting)
- Any external data files (CIF, POSCAR) included alongside the notebook
- References formatted consistently (e.g. APA or Vancouver)

## Assessment Criteria

| Criterion | Marks |
|-----------|-------|
| Correct use of ASE to build and manipulate structures | 25 |
| Quality and clarity of figures | 20 |
| Physical understanding demonstrated in discussion | 30 |
| Engagement with primary literature | 15 |
| Code clarity, comments, and reproducibility | 10 |

---

## Hints and Resources

- The [ASE documentation](https://wiki.fysik.dtu.dk/ase/) is your primary reference
- The [Materials Project](https://materialsproject.org) provides starting structures and reference DFT data
- The [Defects in Semiconductors](https://www.sciencedirect.com/book/9780080519425/defects-in-semiconductors) textbook is useful background reading
- For quantum optics context: Aharonovich et al., *Nature Photonics* 10, 631 (2016) is an excellent review
- The [SHAKENBREAK](https://shakenbreak.readthedocs.io/) code is useful for exploring defect geometries beyond standard relaxation
- Post questions to the course discussion forum — do not share code solutions

---

*Good luck! Computational materials science is a powerful lens for understanding quantum systems, and the skills you develop here are directly transferable to research in quantum technologies.*
