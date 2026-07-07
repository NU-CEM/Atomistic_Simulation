# Atomistic Simulation for Quantum and Molecular Photonics

Welcome to *Atomistic Simulation for Quantum and Molecular Photonics*, a practical undergraduate course in atomistic simulation methods applied to materials for quantum and molecular photonics.

## Course Description

This course introduces the computational tools and concepts needed to model the structural, electronic, and defect properties of materials. We use [ASE (Atomic Simulation Environment)](https://wiki.fysik.dtu.dk/ase/) as our primary software framework, which provides a clean Python interface to a range of pre-processing tools, electronic structure codes and analysis tools.

The course has a dual focus:
- **Core simulation skills** that are transferable across all areas of materials research
- **Application examples** drawn from quantum and molecular optics: single-photon emitters, optically active defects, photonic semiconductors, and 2D materials.

## Who is this course for?

This course is aimed at undergraduate students in physics, chemistry, or materials science who have:
- Basic familiarity with Python (variables, lists, loops, functions)
- Some background in solid-state physics or physical chemistry
- An interest in computational approaches to materials

No prior experience with atomistic simulation is required.

## How to use this resource

Each lecture is a self-contained Jupyter Notebook. You can:
- **Read** the rendered version on this website
- **Run interactively** via Google Colab using the rocket 🚀 button at the top of each page
- **Download** the notebooks and run them locally

## Course Structure

| Lab | Topics | Skills | Exercise |
|---------|--------|--------|----------|
| 1. Introduction | Motivation and scope; brief history of atomistic simulation; expectations and assessment | Setting up a Python environment; navigating Jupyter notebooks | Scientific programming warm-up |
| 2. Atomistic Simulation Basics | Composition-structure-property relationships; overview of simulation methods; where DFT, MLIPs, and MD fit in | Using the Materials Project database; interpreting crystal structure data | Exploring the Materials Project |
| 3. Working with Atoms | The ASE Atoms class; accessing and modifying structural data; reading and writing structure files; visualising structures | ASE Atoms object; CIF/XYZ file I/O; structure visualisation with nglview | Lattice parameter of gold |
| 4. Manipulating Atoms | Building molecules and bulk crystals; creating supercells; introducing point defects | ASE build module; supercell construction; vacancy and substitution creation | Building a defect supercell |
| 5. Potential Energy and Equilibrium Structure | Effective Medium Theory; computing potential energy surfaces; fitting equations of state; finding equilibrium structures | EMT calculator; equation of state fitting with ASE | Equation of state for a metal |
| 6. Local Optimisation | Introduction to DFT; optimising atomic positions; optimising the unit cell | GPAW setup and convergence; geometry relaxation | Relaxing a crystal structure with DFT |
| 7. Electronic Structure | Electronic bandstructure; density of states; k-point convergence | GPAW bandstructure and DOS calculations; k-point convergence tests | Bandstructure of silicon |
| 8. Machine-Learnt Interatomic Potentials | What are MLIPs and when should I use them?; using MACE for geometry optimisation; screening studies | MACE calculator; high-throughput structure relaxation | Screening lattice parameters across a material family |
| 9. Point Defects | Defect supercells; geometry relaxation with MLIPs; electronic structure of defect systems; relevance to quantum emitters | Defect creation in ASE; MACE relaxation; GPAW DOS for defect systems | NV centre in diamond |
| 10. Molecular Dynamics | MD for time evolution; tracking thermodynamic properties; generating and relaxing disordered structures | NVT/NPT MD with ASE; trajectory analysis | Thermal expansion of a crystal |


## Acknowledgements

Much of the core ASE content is adapted from the [Open Science with ASE workshop tutorials](https://ase-workshop-2023.github.io/tutorial/) (CC-BY 4.0) developed by Adam Jackson and Lucy Whalley. 

This course is developed by Lucy Whalley and James Quirk at [Northumbria University](https://www.northumbria.ac.uk/).
