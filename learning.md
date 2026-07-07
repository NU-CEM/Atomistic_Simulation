# Learning Outcomes

By the end of each session, students should be able to:

## 1. Introduction
- Describe the role of atomistic simulation in modern materials research
- Explain how atomistic simulation has developed historically, from empirical potentials to machine learning
- Set up and navigate a Jupyter notebook environment for computational work

## 2. Atomistic Simulation Basics
- Explain the composition-structure-property paradigm and its relevance to materials design
- Identify appropriate simulation methods (DFT, MLIPs, MD) for a given materials problem
- Use the Materials Project to retrieve and interpret structural and electronic data for a material of interest

## 3. Working with Atoms
- Create and manipulate an ASE Atoms object to represent a molecule or crystal
- Read and write structure files in common formats (CIF, XYZ, POSCAR)
- Visualise atomic structures interactively using nglview

## 4. Manipulating Atoms
- Build molecules and bulk crystal structures programmatically using ASE
- Construct a supercell of appropriate size for a given simulation task
- Introduce point defects (vacancies, substitutions) into a host supercell

## 5. Potential Energy and Equilibrium Structure
- Calculate the potential energy of an atomic system using an EMT calculator
- Fit an equation of state to energy-volume data and extract equilibrium lattice parameters and bulk modulus
- Compare computed structural properties to experimental values

## 6. Local Optimisation
- Explain the basic principles of density functional theory at a conceptual level
- Set up and run a DFT geometry optimisation using GPAW
- Assess convergence of a geometry relaxation and interpret the output

## 7. Electronic Structure
- Compute and plot an electronic bandstructure and density of states using DFT
- Identify the valence band maximum, conduction band minimum, and bandgap
- Test and justify a choice of k-point sampling for a given material

## 8. Machine-Learnt Interatomic Potentials
- Explain the key advantages and limitations of MLIPs relative to DFT
- Use the MACE-MP-0 potential to relax a crystal structure
- Design and run a simple screening study across a set of structures or compositions

## 9. Point Defects
- Construct a defect supercell and assess its suitability for a DFT or MLIP calculation
- Relax a defect geometry using MACE and report key structural changes
- Compute a density of states for a defect system and identify in-gap defect states
- Connect computed defect properties to experimentally observable quantities such as zero-phonon line emission

## 10. Molecular Dynamics
- Set up and run an NVT or NPT molecular dynamics simulation using ASE
- Extract and plot thermodynamic properties (temperature, energy, pressure) from a trajectory
- Generate a disordered structure via high-temperature MD followed by quench relaxation
