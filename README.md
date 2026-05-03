# Cosmology: Recombination Models Notebook

This repository contains a teaching notebook on cosmological recombination.

The main file is:

- `recombination.ipynb`

The notebook develops a sequence of increasingly realistic models:

1. Hydrogen recombination in Saha equilibrium
2. Hydrogen + helium recombination in Saha equilibrium
3. The Peebles (1968) non-equilibrium recombination equation
4. Coupled evolution of the free-electron fraction `x_e` and baryon temperature `T_b`
5. A simple reionization model and the Thomson optical depth `tau`
6. An optional toy energy-injection extension

## Intended Use

This notebook is written to be:

- readable by senior undergraduate students
- suitable for lecture demonstrations or guided assignments
- compact enough to inspect equation-by-equation

It is primarily an educational notebook rather than a precision cosmology pipeline.

## Repository Contents

- `recombination.ipynb`: the main teaching notebook
- `requirements.txt`: minimal Python dependencies
- `.gitignore`: standard Python and Jupyter ignores

## Getting Started

Create or activate a Python environment, then install the dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook recombination.ipynb
```

The notebook is committed without stored cell outputs so the repository stays lightweight. Run the cells to regenerate all figures.

## Notebook Structure

The notebook is organized as follows:

- `Cosmology and constants`: background cosmology and physical constants
- `Background helper functions`: conversions between `z`, `a`, and `x = ln(a)`
- `Hydrogen recombination in Saha equilibrium`
- `Equilibrium Saha model with hydrogen and helium`
- `The Peebles (1968) non-equilibrium hydrogen recombination model`
- `Coupled evolution of x_e and the baryon temperature T_b`
- `A phenomenological reionization model and the optical depth tau`
- `Optional extension: a toy energy-injection model`

## Physics Scope

This repository intentionally balances clarity and physical realism.

- The hydrogen Saha and Peebles treatments are the core models.
- The hydrogen + helium Saha section is included to illustrate how helium modifies the early-time ionization history.
- The reionization and energy-injection sections are phenomenological extensions intended for teaching.
- This notebook is not a replacement for dedicated recombination codes such as RECFAST, HyRec, or CosmoRec.

## Suggested Classroom Uses

- Compare equilibrium and non-equilibrium recombination histories
- Explore the effect of helium on `x_e(z)`
- Study the decoupling of `T_b` from `T_gamma`
- Relate reionization histories to the optical depth
- Build short student exercises by modifying `Y_p`, the reionization parameters, or the energy-injection model

## Notes

- The current notebook replaces an older version of the repository with a cleaner, better documented teaching version.
- A local backup of the original notebook was kept during development, but it is not included in this GitHub upload package.
