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

| Lecture | Title | Topics | Key Skills | Exercise |
|---------|-------|-----------|--------|---------|

| 1 | Introduction | Motivation and scope, A brief history of atomistic simulation, Expectations and assessments | Software setup | Scientific programming |
| 2 | Atomistic Simulation Basics | Composition-Structure-Property relationships, Atomistic simulation methods overview | | The Materials Project |
| 3 | Reading and Writing Structures | I/O formats, trajectories, databases | | |
| 4 | Building and Manipulating Structures | Supercells, point defects, surfaces || |
| 5 | Calculators and Computing Properties | EOS, file-based calculators, k-point convergence || |
| 6 | Electronic Structure | Band structure, DOS, direct/indirect gaps || |
| 7 | Molecular Dynamics | NVE/NVT ensembles, observers, VACF || |
| 8 | Structure Optimisation | BFGS, FIRE, constraints, defect relaxation || |
| 9 | Materials for Quantum and Molecular Optics | NV centre, hBN V_B, QDs, rare-earth ions || |



Tutorial two:
What is atomistic simulation, and how does it relate to physics? (Composition-Structure-Property relationships)
Why is atomistic simulation important?

Where does this course fit in?
Exercise: The Materials Project

Tutorial three: Working with atoms
How can I describe a molecule of crystal using the Atoms class?
How can I access and adjust Atoms information?
How do I read/write structure(s) from/to a file?
How do I visualise structures?
Exercise: The lattice parameter of gold

Tutorial four: Manipulating atoms
How can I build molecules?
How can I build and bulk structures?
How can I create supercells?
How can I create point defects?
Exercise:

Tutorial five: Potential energy and equilibrium structure
What is Effective Medium Theory (EMT)?
How can I use EMT to calculate the potential energy of metal alloy systems?
How can I fit simple models to my data?
How can I identify the equilibrium structure?
Tutorial six: Local optimisation
What is Density Functional Theory (DFT)?
How can I use DFT to optimise atom positions?
How can I use DFT to optimise other degrees of freedom?
Tutorial seven: Electronic structure
How can I use DFT to produce an electronic bandstructure?
How can I use DFT to produce an electronic density of states?
How can I test for k-point convergence?
Tutorial eight: Machine-Learnt Interatomic Potentials
What are Machine-Learnt Interatomic Potentials (MLIPs)?
How can I use MLIPs to identify equilibrium positions?
How can I use MLIPs to perform a screening study?
Tutorial nine: Molecular Dynamics
How can I use Molecular Dynamics (MD) to evolve a system over time?
How can I track system properties over time?
How can I generate disordered structures?
How can I relax disordered structures?
Tutorial ten: Point Defects

| Lecture | Topic | Key skills |
|---------|-------|-----------|

| 1 | Introduction to ASE | Import ASE, EMT calculator, ASE ecosystem |
| 2 | The Atoms Object | Build, visualise, get/set properties |
| 3 | Reading and Writing Structures | I/O formats, trajectories, databases |
| 4 | Building and Manipulating Structures | Supercells, point defects, surfaces |
| 5 | Calculators and Computing Properties | EOS, file-based calculators, k-point convergence |
| 6 | Electronic Structure | Band structure, DOS, direct/indirect gaps |
| 7 | Molecular Dynamics | NVE/NVT ensembles, observers, VACF |
| 8 | Structure Optimisation | BFGS, FIRE, constraints, defect relaxation |
| 9 | Materials for Quantum and Molecular Optics | NV centre, hBN V_B, QDs, rare-earth ions |

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
