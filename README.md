# Metastable-dynamics

## What is it?

This is the Mathematica code to trace the evolution of metastable species - pions, muons, and kaons - injected by decays of hypothetical Long-Lived Particles (LLPs) in the MeV primordial plasma of the Early Universe. The code incorporates various processes with metastable particles: decays, annihilations, and interactions with nucleons, and solves the system of integrated Boltzmann equations on their number densities. The output may be used for various solvers of neutrino Boltzmann equations.

The underlying physics is described in the associated preprints [2411.00931](https://arxiv.org/abs/2411.00931) and [2411.00892](https://arxiv.org/abs/2411.00892). 


## How to launch

Just launch the initialization cells in the main notebook <code>main.nb</code> and follow the Appendix of [2411.00931](https://arxiv.org/abs/2411.00931). 

The corresponding [Zenodo repository](https://doi.org/10.5281/zenodo.14020343) containts precomputed data that may be used to make some plots from the associated preprints.



## Requirements

The code requires [FeynCalc](https://feyncalc.github.io/) package that may be easily installed inside Mathematica.