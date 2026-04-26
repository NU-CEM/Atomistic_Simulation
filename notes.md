- could time as function of number of electrons
- vary between bulk and monolayer in hBN
- could also think about varying chemistry (carbon monolayers)
- need to show eos for layered material

I want to make an example notebook for another question, to show the depth of thinking that is required for top marks.

Group assignment: For that size I'd probably go with a short Google Form asking:

Python confidence (1-5 scale)
Any scheduling constraints (days and times in the week)
Optionally, a system preference (1st and 2nd choice)
Is there anything we should be aware of when forming pairs? You don't need to give details — a brief note is fine. 

If you have any concerns please reach out to the course instructor via email.

Then assign groups yourself using that info to balance confidence levels, and try to honour at least one system preference per group. 

source /Users/mynf8/miniforge3/bin/activate KL6003


#### Tutorial one: Introduction

1. Motivation and scope
   ---> What is atomistic simulation, and how does it relate to physics? the big ideas. sschematic showing how it relates to the physics degree programme.
   ---> Why is atomistic simulation important? applications: semiconductors, energy, quantum computing (this course)
2. A brief history of atomistic simulation (including shift to machine learning) and the future: inverse design and integration with experiment.
3. outline of this course
4. Expectations and assessments
5. Setup

Exercise: Scientific programming exercise, including verification of setup steps (everything installed correct)

#### Tutorial two: Atomistic Simulation Basics

1. Composition-Structure-Property relationships
2. Which methods do we commonly use to simulate materials?
3. Introduction to DFT, Machine-learnt interatomic potentials

Exercise: The Materials Project exercise: website and API. But what?

#### Tutorial three: Working with atoms

1. How can I describe a molecule or a crystal using the Atoms class?
2. How can I access and adjust Atoms information?
3. How do I read/write structure(s) from/to a file?
4. How do I visualise structures? (in notebook and in vesta)

Exercise: Reading in a cif file from the materials project: website and API. But what?

#### Tutorial four: Manipulating atoms

1. How can I build molecules?
2. How can I build and bulk structures?
3. How can I create supercells?
4. How can I create point defects?
5. How can I build layered materials?
6. How can I access structural properties of my material?

Exercise: Creating a defect complex. Creating a layered material and (extension) heterostructure.
Creating the structure for your coursework.

#### Tutorial five: Potential energy and equilibrium structure

1. ASE calculators
2. What is Effective Medium Theory (EMT)?
2. How can I use EMT to calculate the potential energy of metal alloy systems?
3. How can I fit simple EOS models to my data to find equilibrium structure?
4. Limitations of this approach (local minima, when many degrees of freedom)

Exercise: The lattice parameter of gold.
Exercise: Finding the equilibrium structure for your coursework.

#### Tutorial six: Local optimisation

1. Density Functional Theory (DFT) basics
    - kpoints, XC's, PBC, basis functions etc etc
2. How can I use DFT to optimise atom positions?
3. How can I use DFT to optimise other degrees of freedom?
4. Limitations: hitting on the computer expense (HPC and friends)

Exercise: Compare to the EOS approach

#### Tutorial seven: Electronic structure 
  
2. How can I use DFT to produce an electronic bandstructure?
3. How can I use DFT to produce an electronic (projected) density of states?
4. How can I test for k-point convergence?

Exercise: Convergence testing

#### Tutorial eight: Machine-Learnt Interatomic Potentials 

1. What are Machine-Learnt Interatomic Potentials (MLIPs)?
    3. Advantages and limitations of MLIPs. Foundational models. Training.
2. How can I use MLIPs to identify equilibrium positions?
3. How can I use MLIPs to relax a defect? (breaking symmetry)

Exercise: ???

#### Tutorial nine: Molecular Dynamics

1. How can I use Molecular Dynamics (MD) to evolve a system over time?
2. How can I track system properties over time?
3. How can I generate disordered structures?
4. How can I relax disordered structures?

Exercise: ???

#### Tutorial ten: Point Defects

1. Intro to point defects: why important (optoelectronic killers and SPEs)
2. Types of point defect
3. Modelling point defects: introducing charge.

