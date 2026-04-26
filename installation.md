# Installation Guide

This page explains how to run the course materials. There are two options: running in the cloud (no installation required) or running locally on your own computer.

---

## Option 1: Run in the Cloud (Recommended for Beginners)

No installation is needed. Every notebook has a **launch button** (🚀) at the top of the page. Click it and choose **Google Colab** to open and run the notebook directly in your browser.

You will need a Google account. Your work is saved to your Google Drive automatically.

> **Note:** A small number of exercises require GPAW, which is not available on Colab. These are clearly marked in the notebooks. For those exercises, you will need to run locally (see Option 2) or use the university computing cluster.

---

## Option 2: Run Locally

Running locally gives you the best performance and full access to all software, including GPAW.

### Step 1: Install Miniforge

Miniforge is a lightweight way to install Python and manage software environments. It is free and works on Windows, macOS, and Linux.

1. Go to [https://github.com/conda-forge/miniforge](https://github.com/conda-forge/miniforge#install) and download the installer for your operating system.
2. Run the installer and follow the instructions. Accept the default settings unless you have a reason to change them.
3. Open a new terminal (on Windows, open **Miniforge Prompt** from the Start menu; on macOS/Linux, open **Terminal**).

You can check the installation worked by typing:
```bash
conda --version
```
You should see a version number printed.

### Step 2: Create the Course Environment

A software environment keeps the packages for this course separate from anything else on your computer. To create it, copy and paste the following into your terminal:

```bash
conda create -n KL6003 python=3.11 ase gpaw mace-torch spglib matplotlib numpy jupyterlab nglview ipywidgets -c conda-forge
```

This may take a few minutes. When it finishes, activate the environment:

```bash
conda activate KL6003
```

You will need to run `conda activate KL6003` each time you open a new terminal before working on this course.

### Step 3: Install GPAW Datasets

GPAW requires a set of atomic data files. With the environment active, run:

```bash
gpaw install-data
```

Follow the prompts and accept the default installation location.

### Step 4: Download the Course Notebooks

If you have Git installed:
```bash
git clone https://github.com/NU-CEM/Atomistic_Simulation.git
cd Atomistic_Simulation
git checkout 2026
```

Or download a ZIP file from the [repository page](https://github.com/NU-CEM/Atomistic_Simulation) by clicking **Code → Download ZIP**, then unzip it.

### Step 5: Launch Jupyter

With the environment active and inside the course folder, run:

```bash
jupyter lab
```

Your browser will open automatically. Navigate to the `notebooks/` folder to find the course materials.

---

## Checking Your Installation

Open the first notebook (`introduction.ipynb`) and run all cells. If no errors appear, your installation is working correctly.

If you run into problems, please post a message on the course discussion forum (Blackboard) or [raise an issue](https://github.com/NU-CEM/Atomistic_Simulation/issues) on GitHub.
