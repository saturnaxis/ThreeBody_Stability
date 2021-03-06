# Stability Limit for a Circumstellar Planet within a Binary System
--------
[![Arxiv](https://img.shields.io/badge/arXiv-1912.11019-red.svg?style=flat)](https://arxiv.org/abs/1912.11019)
[![AJ](https://img.shields.io/badge/Version-AJ-brightgreen)](http://dx.doi.org/10.3847/1538-3881/ab64fa)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4026266.svg)](https://doi.org/10.5281/zenodo.4026266)


--------
This is a repository for tools to determine the stability limit, or largest semimajor axis ratio (a_c = a_p/a_bin), of a circumstellar planet. This summarized data in a_crit.txt collates the results of a large number of full N-body simulations using the well-established Mercury6 code (Chambers 1999, Chambers et al. 2002). The simulations evaluated a wide range of initial binary parameters, including the binary mass ratio mu, binary eccentricity e_bin, and varied the mutual inclination relative to the binary orbital plane. The parameter mu is defined as the ratio of the smaller mass star divided by the total mass of the stellar binary (i.e., mu = M_B/(M_A+M_B)). These simulations were performed beginning at binary periastron and should be considered as conservative estimates of stability. Due to symmetry only phases between 0 -- 180 degrees are evaluated, where the negative longitudes (-180 up to 0 deg.) are assumed to be mirror image of the positive ones.

After cloning the repository, the tool for determining a_c for a given set of binary parameters (mu, e_bin) can be determined simply by running **'python get_ac.py mu eb abin ip'**, where mu is replaced with a float [0, 1], eb is replaced with a float [0,0.8], abin is replaced with an arbitrary float, and ip is replaced with an integer [0, 30, 45, 180].

The results from all the simulations are available on Zenodo.org (http://doi.org/10.5281/zenodo.3579202) as a series of compressed tar archives. 

Attribution
--------
A more detailed description of these simulations, the use of an interpolation method, and the context for the future observations with the Transiting Exoplanet Survey Satellite (TESS) are available in the following paper.  Please use the following citation, if you find these tools useful in your research. 

```
@article{Quarles2020,
author = {{Quarles}, B. and {Li}, G. and {Kostov}, V. and {Haghighipour}, N.},
title = "{Orbital Stability of Circumstellar Planets in Binary Systems}",
journal = {\aj},
year = 2020,
month = mar,
volume = {159},
number = {3},
eid = {80},
pages = {80},
doi = {10.3847/1538-3881/ab64fa},
archivePrefix = {arXiv},
eprint = {1912.11019},
primaryClass = {astro-ph.EP},
adsurl = {https://ui.adsabs.harvard.edu/abs/2020AJ....159...80Q},
adsnote = {Provided by the SAO/NASA Astrophysics Data System}
}
```
