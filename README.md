# Normalizing Flows Tutorial — ErUM Deep Learning School 2026

This repository contains the lecture and hands-on material on **normalizing flows** prepared for the ErUM Deep Learning School **“Advanced Concepts.”**

The tutorial introduces normalizing flows as tractable generative models for density estimation and sampling. It covers:

- change of variables and exact likelihood evaluation;
- affine coupling transformations and RealNVP-style models;
- masked autoregressive flows (MAF);
- neural spline flows (NSF);
- continuous normalizing flows (CNF);
- conditional density estimation;
- scientific applications to neutron-source modeling.

Most examples use [Zuko](https://zuko.readthedocs.io/), a PyTorch library providing ready-to-use normalizing-flow architectures.

## Main material

- `norm_flow_robledo_erum.pdf` — lecture slides.
- `normalizing_flows_hand-on.ipynb` — participant tutorial with exercises.
- `normalizing_flows_hand-on_solution.ipynb` — completed tutorial and solutions.
- `zuko_tutorial.ipynb` — short introduction to the Zuko interface and its benefits.
- `mcpl_example.ipynb` — scientific example learning the neutron phase-space distribution at surface S003 of the RA-6 reactor from OpenMC/MCPL data.

## Installation

The notebooks primarily require Python, PyTorch, Zuko, NumPy, Matplotlib, Pandas, and Seaborn:

```bash
pip install torch zuko numpy matplotlib pandas seaborn jupyter
```

The neutron-source example additionally requires the MCPL Python package and command-line tools:

```bash
pip install mcpl
```

Start Jupyter from the repository directory and open the participant notebook:

```bash
jupyter lab normalizing_flows_hand-on.ipynb
```

## Learning objective

After completing the tutorial, participants should be able to train and evaluate a normalizing flow, generate samples, inspect the learned latent representation, compare common flow architectures, and construct conditional generative models for scientific data.
