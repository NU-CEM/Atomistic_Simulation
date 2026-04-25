[![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![deploy-book](https://github.com/NU-CEM/Materials_Simulation/actions/workflows/deploy.yml/badge.svg)](https://github.com/NU-CEM/Materials_Simulation/actions/workflows/deploy.yml)
[![CC-BY license](https://img.shields.io/badge/License-CC--BY-blue.svg)](https://creativecommons.org/licenses/by/4.0)

# Materials Simulation for Quantum and Molecular Optics

Online resource for a practical undergraduate course in atomistic simulation, with applications to materials for quantum and molecular optics.

## Course Website

View the book at: **https://nu-cem.github.io/Materials_Simulation**

## Course Description

*Materials Simulation* provides a practical introduction to atomistic simulation using the [Atomic Simulation Environment (ASE)](https://wiki.fysik.dtu.dk/ase/). It is aimed at undergraduate students in physics, chemistry, or materials science.

The course develops core simulation skills — building structures, running calculators, computing electronic structure, performing MD and geometry optimisation — and applies them to materials of current interest in quantum and molecular optics: single-photon emitters, wide-bandgap semiconductors, and 2D materials.

## Contents

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
git clone https://github.com/NU-CEM/Materials_Simulation
cd Materials_Simulation
jupyter-book build .
```

Open `_build/html/index.html` in your browser.

## Running Notebooks

Each notebook can be run:
- **On Google Colab**: click the 🚀 button at the top of any page on the website
- **Locally**: install requirements with `pip install -r requirements.txt`, then `jupyter notebook`
- **On Binder**: click the Binder button at the top of any page

## Acknowledgements

Core ASE content is adapted from the [Open Science with ASE workshop tutorials](https://ase-workshop-2023.github.io/tutorial/) (Pietro Delugas, Adam Jackson, Lucy Whalley; CC-BY 4.0). The Jupyter Book infrastructure is inspired by [MLforMaterials](https://github.com/aronwalsh/MLforMaterials) (Aron Walsh; CC0).

## Licence

[Creative Commons Attribution 4.0 International (CC-BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

You are free to share and adapt this material, provided you give appropriate credit.
