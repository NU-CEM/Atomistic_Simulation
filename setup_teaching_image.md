# KL6003 Materials Simulation — Setup Guidance for teaching image


This describes the software environment required for the KL6003 Materials Simulation module (computer labs led by Lucy Whalley, l.whalley@northumbria.ac.uk).

---

## Prerequisites

### Anaconda or Miniconda

The standard Anaconda or Miniconda installation is sufficient. If conda (or mamba) is already deployed on the teaching image, no additional package manager is needed.

---

## Environment Setup

Run the following commands from the **Anaconda Prompt**. Each step is explained below.

### Step 1: Create and activate the environment

```bat
conda create -n KL6003 python=3.11
conda activate KL6003
```

**Why Python 3.11?** The key dependency PyTorch (required for MACE) currently only ships wheels for Python 3.11 and below on x86_64. Python 3.12+ will cause installation failures.

### Step 2: Install core scientific packages via conda-forge

```bat
conda install -c conda-forge gpaw ase matplotlib numpy jupyter jupyterlab pandas matscipy "numpy<2" pip spglib
```

**Package notes:**
- `gpaw` — DFT code used for electronic structure calculations
- `ase` — Atomic Simulation Environment, the core framework
- `matscipy` — required by MACE at runtime; must be installed via conda-forge to avoid C++ compilation errors on Windows
- `numpy<2` — MACE's PyTorch dependency requires NumPy 1.x; installing via conda-forge ensures consistent versions
- `pip` — needed for packages not available on conda-forge
- `spglib` - handling crystal symmetry

### Step 3: Install MACE via pip

```bat
pip install mace-torch
```

MACE is a machine-learned interatomic potential used for fast geometry relaxation. It is only available via pip. Installing after the conda-forge packages ensures no version conflicts.

### Step 4: Install GPAW PAW datasets and basis sets

GPAW requires PAW (Projector Augmented Wave) datasets and LCAO basis set files. These are separate from the code and must be downloaded and installed.

```bat
gpaw install-data --version=24.11.0 %CONDA_PREFIX%\Lib\site-packages\gpaw_data\setups
gpaw install-data --basis %CONDA_PREFIX%\Lib\site-packages\gpaw_data\setups
```

Then unzip all downloaded files. GPAW ships data files as gzipped archives but reads them uncompressed; this step is essential — without it GPAW will fail with `FileNotFoundError`.

### Step 5: Set the GPAW_SETUP_PATH environment variable

GPAW needs to know where to find its data files at runtime - set this as a system environment variable.

**Option A — via the conda environment activation script:**

```bat
mkdir %CONDA_PREFIX%\etc\conda\activate.d
echo set "GPAW_SETUP_PATH=%CONDA_PREFIX%\Lib\site-packages\gpaw_data\setups" > %CONDA_PREFIX%\etc\conda\activate.d\gpaw_setup.bat
```

**Option B — via Windows System Environment Variables:**

1. Open System Properties → Advanced → Environment Variables
2. Under System Variables, click New
3. Variable name: `GPAW_SETUP_PATH`
4. Variable value: `C:\ProgramData\Miniconda3\envs\KL6003\Lib\site-packages\gpaw_data\setups` (adjust path to match your Miniconda installation location)

Option A is preferred as it does not affect other Python environments on the machine.

---

## Verification

Run the following sanity check from the Anaconda Prompt to confirm the environment is working correctly. This should complete in under 60 seconds.

```bat
conda activate KL6003

python -c "
from gpaw import GPAW
from ase.build import bulk

diamond = bulk('C', 'diamond', a=3.57)
calc = GPAW(mode='lcao', basis='dzp', xc='PBE', kpts=(1,1,1), txt='-')
diamond.calc = calc
diamond.get_potential_energy()
print('PASS: GPAW LCAO working correctly')

from mace.calculators import mace_mp
diamond2 = bulk('C', 'diamond', a=3.57)
calc2 = mace_mp(model='medium', dispersion=False, default_dtype='float64')
diamond2.calc = calc2
energy = diamond2.get_potential_energy()
print(f'PASS: MACE working correctly (energy = {energy:.3f} eV)')

import jupyter, jupyterlab
print('PASS: Jupyter and JupyterLab available')
print()
print('All tests passed. Environment is ready for KL6003.')
"
```

Expected output:
```
PASS: GPAW LCAO working correctly
PASS: MACE working correctly (energy = -X.XXX eV)
PASS: Jupyter and JupyterLab available

All tests passed. Environment is ready for KL6003.
```

---

## MPI Parallelisation (not absolutely critical, but would be beneficial)

GPAW supports MPI parallelisation with no changes to student scripts. On Windows, MPI support depends on whether GPAW was built with MPI — the conda-forge GPAW build includes Microsoft MPI (MS-MPI) support.

Check if MPI is available:

```bat
conda activate KL6003
python -c "from gpaw.mpi import world; print(f'MPI available, size={world.size}')"
```

If MS-MPI is not already installed on the teaching image, install it:
- Download from https://www.microsoft.com/en-us/download/details.aspx?id=105289
- Install `msmpisetup.exe` (runtime) and `msmpisdk.msi` (SDK)

If it is installed correctly then it can be run with:

```bat
mpiexec -n 4 gpaw python script.py
```

---

## Troubleshooting

**`FileNotFoundError: N.dzp.basis`** — The unzip step did not complete, or `GPAW_SETUP_PATH` is not set. Re-run Step 4 and verify Step 5.

**`matscipy` compilation failure** — matscipy was installed via pip instead of conda-forge. Run `pip uninstall matscipy` then `conda install -c conda-forge matscipy`.

**`numpy` version conflicts** — A pip package has upgraded numpy to 2.x. Run `conda install -c conda-forge "numpy<2" --force-reinstall`.

**conda environment solving is very slow** — Install mamba: `conda install -n base -c conda-forge mamba`, then replace `conda` with `mamba` in Steps 1 and 2.

---

