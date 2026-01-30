# Spin Dynamics Workshop (Python)

This repository contains the material for a hands-on workshop where students build an atomistic spin-dynamics code from scratch in Python. The focus is didactic: we implement each routine step-by-step and immediately test/visualize the result inside a Jupyter Notebook.

## What you will learn
- Represent spins as normalized 3D vectors
- Build lattices and periodic boundary conditions (PBC)
- Define interactions: exchange J_ij, DMI D_ij with D_ji = -D_ij, and an external Zeeman field
- Compute effective fields H_eff
- Integrate the Landau–Lifshitz–Gilbert (LLG) equation with a stable predictor–corrector scheme
- Visualize magnetic configurations interactively (ipympl) and via top-view plots

## Notebook content
The main notebook is routine-by-routine and includes three examples:
- Example 01: Nanochain (baseline workflow)
- Example 02: Square lattice (20×20, PBC) with skyrmion initialization and Zeeman field
- Example 03: Kagomé lattice example (non-collinear order)

## Requirements
- Python 3.10+ recommended
- Packages: numpy, pandas, matplotlib, tqdm, ipympl

Install with:
    pip install numpy pandas matplotlib tqdm ipympl

If you use classic Jupyter Notebook, you may need (one-time):
    jupyter nbextension enable --py --sys-prefix ipympl

## How to run
From the repository root:
    jupyter notebook

Open the notebook and run cells from top to bottom.

## Notes
Some sections generate simple input files (e.g. lattice_*.in, jij_*.in, dij_*.in) to demonstrate I/O. These can be deleted safely after running.

## Suggested repository structure (optional)
- notebooks/ : workshop notebooks
- src/       : reusable functions if you later refactor code out of the notebook
- data/      : example inputs
- outputs/   : results generated during runs

## Contact
Created by Ramon Cardias and Flaviano José dos Santos
