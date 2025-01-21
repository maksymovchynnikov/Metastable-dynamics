# Metastable-dynamics

## What it is?

This is the Mathematica code to trace the evolution of metastable species - charged pions, muons, and kaons - injected by decays of hypothetical Long-Lived Particles (LLPs) in the MeV primordial plasma of the Early Universe. The code incorporates various processes with metastable particles: decays, annihilations, and interactions with nucleons, and solves the system of integrated Boltzmann equations on their number densities. The output may be used for various solvers of neutrino Boltzmann equations.

The underlying physics is described in the associated preprints [2411.00931](https://arxiv.org/abs/2411.00931) and [2411.00892](https://arxiv.org/abs/2411.00892). 

## Structure of the code

The code consists of a few notebooks:

* <dt><code>main.nb</code></dt>
* <dt><code>plot-numbers.nb</code></dt>
* <dt><code>plot-distributions.nb</code></dt>


## How to launch

Just launch the initialization cells in the main notebook <code>main.nb</code>. Additional details are provided in the Appendix of [2411.00931](https://arxiv.org/abs/2411.00931). 

For the given implemented model, after launching the initialization cells, launch manually the content of the chapter "Launching for mass and lifetime grids". 

If you want to visualize the dynamics of the LLP for the given mass and lifetime, launch the content of the chapter "Illustrating the dynamics".

The corresponding [Zenodo repository](https://doi.org/10.5281/zenodo.14020343) containts precomputed data that may be used to make some plots from the associated preprints.


## Requirements

The code requires [FeynCalc](https://feyncalc.github.io/) package that may be easily installed inside Mathematica.