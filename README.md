# The horseshoe prior and its limitations

## Introduction
The horseshoe prior is a popular choice for Bayesian variable selection, particularly in high-dimensional settings. It is known for its ability to shrink small coefficients towards zero while allowing larger coefficients to remain relatively unshrunk. It was introduced by Carvalho et al. (2009) and has since gained popularity in various fields, including genomics, finance, and machine learning.

## How to use
This repository contains the code to reproduce the figures contained in our [report](report/report.pdf) on the horseshoe prior. Our report introduces the horseshoe prior and demonstrates its superiority over the LASSO. We also discuss one limitation of the original horseshoe prior, which is the choice of $\tau$. This limitation is adressed in the Finnish horseshoe prior, from which the second part of our report is derived.

## Code
All the code is summarized in the self-contained Jupyter notebook `horseshoe.ipynb`, which reproduces the following figures:
- Figure 1: The priors on $\beta_i$ induced by the different priors on $\lambda_i$.
- Figure 2: The priors on $\kappa_i$ induced by the different priors on $\lambda_i$.
- Figure 3: The posterior mean $\mathbb{E}[\beta_i | y]$ as a function of $y$ using the Horseshoe prior vs. the LASSO.
- Figure 4: The priors on $m_{eff}$ induced by the different priors on $\tau$.

## Report
Our report, alongside the figures, is available in the `report` folder.