[![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)
[![deploy-book](https://github.com/NU-CEM/Atomistic_Simulation/actions/workflows/deploy.yml/badge.svg)](https://github.com/NU-CEM/Atomistic_Simulation/actions/workflows/deploy.yml)
[![CC-BY license](https://img.shields.io/badge/License-CC--BY-blue.svg)](https://creativecommons.org/licenses/by/4.0)

# Atomistic Simulation for Quantum and Molecular Optics

Online resource for a practical undergraduate course in atomistic simulation, with applications to materials for quantum and molecular optics.

## Course Website

View the book at: **https://nu-cem.github.io/Atomistic_Simulation**

## Course Description

*Atomistic Simulation* provides a practical introduction to atomistic simulation using the [Atomic Simulation Environment (ASE)](https://wiki.fysik.dtu.dk/ase/). It is aimed at undergraduate students in physics, chemistry, or materials science.

The course develops core simulation skills — building structures, running calculators, computing electronic structure, performing MD and geometry optimisation — and applies them to materials of current interest in quantum and molecular optics: single-photon emitters, wide-bandgap semiconductors, and 2D materials.

## Contents

| Lecture | Title | Topics | Exercise |
|---------|-------|-----------|---------|
| 1 | Introduction | Motivation and scope, A brief history of atomistic simulation, Expectations and assessments | Software setup |
| 2 | Atomistic Simulation Basics | Composition-Structure-Property relationships, Atomistic simulation methods overview | Finding first-principles data |
| 3 | Reading and Writing Atoms |  `Atoms` class, I/O formats, Visualising atomic structures | Exploring crystal symmetry |
| 4 | Manipulating Atoms | Supercells, Point defects, Interfaces| Creating complex materials |
| 5 | Potential Energy and Equations of State | ASE calculators, Effective Medium Theory, Equations of State | The lattice parameter of gold I |
| 6 | Local Optimisiation | Density Functional Theory, Convergence, Geometry relaxation | The lattice parameter of gold II |
| 7 | Electronic Structure | Bandstructures, density of states | Convergence testing |
| 8 | Point Defects | Defect types, NV centre | Identifying deep defects |
| 9 | Machine Learning Interatomic Potentials | MACE, Foundational models | Relaxing point defects |


## Building the Book Locally

Install Jupyter Book:

```bash
pip install jupyter-book
```

Clone this repository and build:

```bash
git clone https://github.com/NU-CEM/Atomistic_Simulation
cd Atomistic_Simulation
jupyter-book build .
```

Open `_build/html/index.html` in your browser.

## Running Notebooks

Each notebook can be run:
- **On Google Colab**: click the 🚀 button at the top of any page on the website
- **Locally**: install requirements with `pip install -r requirements.txt`, then `jupyter notebook`. Need Python 3.11 for MACE/pytorch.
- **On Binder**: click the Binder button at the top of any page

## Acknowledgements

Core ASE content is adapted from the [Open Science with ASE workshop tutorials](https://ase-workshop-2023.github.io/tutorial/) (Adam Jackson and Lucy Whalley). 

## Licence

[Creative Commons Attribution 4.0 International (CC-BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

You are free to share and adapt this material, provided you give appropriate credit.
