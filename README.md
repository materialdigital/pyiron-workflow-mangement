# pyiron-workflow-mangement

pyiron workflows consist of jupyter notebook or more jupyter notebooks plus the conda `environment.yml` file defining the strict dependencies.
In addition they can contain further files like python classes or parameter files. 
They are published in Github repositories as tagged releases and it is recommended to use Github actions to continously test the workflows.
Finally with an mybinder link the repository can be tested directly. 

## Current pyiron workflows 

| Name | Repository | Description | Version |
|------|------------|-------------|---------|
| pyiron-workflow-thermalexpansion | https://github.com/materialdigital/pyiron-workflow-thermalexpansion | Calculate the thermal expansion for different interatomic potentials using LAMMPS | 0.0.2 |
| pyiron-workflow-damask | https://github.com/materialdigital/pyiron-workflow-damask | Calculate temperature dependent elastic constants using LAMMPS and then use those elastic constants in DAMASK to calculate the stress-strain curve of a polycrystal | 0.0.1 |
| pyiron-workflow-phasediagram | https://github.com/materialdigital/pyiron-workflow-phasediagram | Calculate the temperature and concentration dependent free energy with the quasiharmonic approximation using the sqsgenerator, LAMMPS and Phonopy. | 0.0.1 |
| pyiron-workflow-TEMImageSegmentation | https://github.com/materialdigital/pyiron-workflow-TEMImageSegmentation | Analyzes a TEM image and perform a segmentation on it | 0.0.1 |

## Resolving the dependencies 
Example notebook how to resolve the dependencies for different pyiron workflows

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/materialdigital/pyiron-workflow-mangement/HEAD?filepath=compare.ipynb)

## Updates 
The https://dependabot.com app is used to trigger automated updates whenever a new version of a dependency is released. Still dependabot currently only supports `pip` based requirements, updating the conda dependencies still requires manual steps. 
