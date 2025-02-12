# Metastable-dynamics

## What it is?

This is the Mathematica code to trace the evolution of metastable species - charged pions, muons, and kaons - injected by decays of hypothetical Long-Lived Particles (LLPs) in the MeV primordial plasma of the Early Universe. The code incorporates various processes with metastable particles: decays, annihilations, and interactions with nucleons, and solves the system of integrated Boltzmann equations on their number densities. The output may be used for various solvers of neutrino Boltzmann equations.

The underlying physics is described in the associated preprints [2411.00931](https://arxiv.org/abs/2411.00931) and [2411.00892](https://arxiv.org/abs/2411.00892). 

## Structure of the code

The code consists of a few main notebooks:

* <dt><code>main.nb</code></dt>
* <dt><code>plot-numbers.nb</code></dt>
* <dt><code>plot-distributions.nb</code></dt>

as well a secondary notebooks defining details of the metastable particles dynamics and various routines. 

The first notebook defines all the machinery needed to calculate the dynamics of the metastable particles in the form of the probabilities to decay, annihilate, and scatter off nucleons. It also exports the data in the format suitable for the unintegrated neutrino Boltzmann equation solver described in the same papers. The pre-defined models are given in chapter "LLP input", with the section "Description of all the required input" summarizing the input required from the user to implement new models. Additional details are provided in the Appendix of [2411.00931](https://arxiv.org/abs/2411.00931). 

The second notebook uses the generated data, as well as the output of the unintegrated Boltzmann code (the associated data will be available via a dedicated Zenodo repository), to make various plots such as N_eff, energy injected into the neutrino sector as the function of the LLP mass and lifetime, and others.

The third notebook utilizes the output of the unintegrated Boltzmann code for the tabulated neutrino distributions (similarly, it will be available via a dedicated Zenodo repository). 

## How to launch

Just launch the initialization cells in the main notebook <code>main.nb</code>.

For the given implemented model, after launching the initialization cells, launch manually the content of the chapter "Launching for mass and lifetime grids". 

If you want to visualize the dynamics of the LLP for the given mass and lifetime, launch the content of the chapter "Illustrating the dynamics".

The code also has corresponding [Zenodo repository](https://doi.org/10.5281/zenodo.14020343).


## Requirements

The code requires [FeynCalc](https://feyncalc.github.io/) package that may be easily installed inside Mathematica.