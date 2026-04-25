# Resources

## Software

### Core tools used in this course
- [ASE (Atomic Simulation Environment)](https://wiki.fysik.dtu.dk/ase/) — the framework used throughout
- [GPAW](https://gpaw.readthedocs.io/) — DFT code written in Python, integrates tightly with ASE
- [Quantum ESPRESSO](https://www.quantum-espresso.org/) — widely used plane-wave DFT code
- [nglview](https://nglviewer.org/nglview/latest/) — interactive 3D molecular viewer for Jupyter

### Useful complementary packages
- [pymatgen](https://pymatgen.org/) — materials analysis library; excellent for symmetry analysis
- [spglib](https://spglib.github.io/spglib/) — space group library (used by both ASE and pymatgen)
- [phonopy](https://phonopy.github.io/phonopy/) — phonon calculations
- [SHAKENBREAK](https://shakenbreak.readthedocs.io/) — defect geometry exploration
- [py-sc-fermi](https://py-sc-fermi.readthedocs.io/) — defect concentration and Fermi level calculations

## Databases

- [Materials Project](https://materialsproject.org) — DFT-computed structures and properties
- [Crystallography Open Database (COD)](http://www.crystallography.net/cod/) — experimental crystal structures
- [ICDD / ICSD](https://icsd.products.fiz-karlsruhe.de/) — inorganic crystal structure database (institutional access)
- [AFLOW](http://aflowlib.org/) — high-throughput computational materials database
- [Quantum Defect Database (QD²)](https://qd2.materialsproject.org/) — computed properties of defect qubits

## Key Review Articles

### Quantum emitters and defect physics
- Aharonovich, I., Englund, D. & Toth, M. *Solid-state single-photon emitters.* Nature Photonics **10**, 631–641 (2016).
- Atatüre, M. et al. *Material platforms for spin-based photonic quantum technologies.* Nature Reviews Materials **3**, 38–51 (2018).
- Gottscholl, A. et al. *Initialization and read-out of intrinsic spin defects in a van der Waals crystal at room temperature.* Nature Materials **19**, 540–545 (2020).

### Computational methods for defects
- Freysoldt, C. et al. *First-principles calculations for point defects in solids.* Reviews of Modern Physics **86**, 253 (2014).
- Dreyer, C. E. et al. *First-principles calculations of point defects for quantum technologies.* Annual Review of Materials Research **48**, 1–26 (2018).

## Textbooks

- Sholl, D. S. & Steckel, J. A. *Density Functional Theory: A Practical Introduction.* Wiley (2009). — Excellent starting point for DFT
- Martin, R. M. *Electronic Structure: Basic Theory and Practical Methods.* Cambridge University Press (2020).
- Alkauskas, A., Deák, P., Neugebauer, J., Pasquarello, A. & Van de Walle, C. G. (Eds.) *Advanced Calculations for Defects in Materials.* Wiley-VCH (2011).

## Online Courses and Tutorials

- [ASE Workshop tutorials](https://ase-workshop-2023.github.io/tutorial/) — the source for much of this course's core content (CC-BY 4.0)
- [GPAW tutorials](https://gpaw.readthedocs.io/tutorialsexercises/) — practical DFT calculations
- [The Carpentries — Programming with Python](https://swcarpentry.github.io/python-novice-inflammation/) — Python refresher

## Pseudopotentials and Basis Sets

For file-based DFT calculations you will need pseudopotentials:
- [PseudoDojo](http://www.pseudo-dojo.org/) — high-quality norm-conserving pseudopotentials (QE, GPAW, Abinit)
- [GBRV](https://www.physics.rutgers.edu/gbrv/) — ultrasoft pseudopotentials for QE
- [ONCVPSP](http://www.mat-simresearch.com/) — optimised norm-conserving Vanderbilt pseudopotentials

## Getting Help

- [ASE GitLab Issues](https://gitlab.com/ase/ase/-/issues) — bug reports and feature requests
- [ASE mailing list](https://listserv.fysik.dtu.dk/mailman/listinfo/ase-users)
- [Materials Science Stack Exchange](https://mattermodeling.stackexchange.com/)
- Course discussion forum (see Blackboard/Canvas)
