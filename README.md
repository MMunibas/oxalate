<p align="center">
Hydrogenoxalate Potential Energy Surfaces<br>
Meuwly Group, University of Basel
</p>

# General

The present repository provides access to the raw data and potential energy surfaces
for hydrogenoxalate, which are described in detail
in Reference [1]. The PESs are obtained following a rational procedure based on transfer
learning to reach CCSD(T) quality for large molecules and are based on PhysNet [2].
This repository contains instructions for the installation and dependencies, a 
description of the different PESs and corresponding raw data. This is followed by examples 
on using the neural network-based PESs. The ab initio raw data is available in *data/MP2* and *data/CCSD(T)*.

# Installations & Dependencies

The following installation steps were tested on a Ubuntu 20.04 workstation and using
Conda 23.7.2 (see https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).
The installation of the dependencies (excluding the installation of Miniconda) takes
less than 5 min. 

a) If not installed already, install Miniconda on your machine (see https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

b) Create an environment named (e.g.) physnet_env, install Python 3.6:

    conda create --name physnet_env python=3.6

   Activate it:

    conda activate physnet_env

    (deactivating it by typing: conda deactivate)


c) With activated environment, all dependencies can be installed.

    pip install ase==3.19.1
    pip install tensorflow==1.12
    pip install tensorflow_estimator


# Potential Energy Surfaces


# Examples


### Evaluations in Python/ASE
Most Python scripts that are used to evaluate the PhysNet PESs make use of the atomic simulation environment (ASE) [3] 
and are written in Python. It is important to get used to ASE, which has very good tutorials 
online (https://wiki.fysik.dtu.dk/ase/tutorials/tutorials.html#ase). 
Scripts on how to use the PESs that have been used throughout the evalulation of Reference [1] are given in the *evaluation* folder. These can for example be used to 

-

-

-


# How to cite 
When using the PhysNet or the Hydrogenoxalate PESs, please cite the following papers:

#### For PhysNet:
Oliver T. Unke and Markus Meuwly "PhysNet: A Neural Network for Predicting Energies,
Forces, Dipole Moments, and Partial Charges", J. Chem. Theory Comput., 2019,
15, 6, 3678–3693

#### For the Hydrogenoxalate PESs:




# References
[1] 

[2] Oliver T. Unke, and Markus Meuwly "PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments, and Partial Charges" J. Chem. Theory Comput. 2019, 15, 6, 3678–3693

[3] Ask Hjorth Larsen et al, "The atomic simulation environment—a Python library for working with atoms", 2017, J. Phys.: Condens. Matter, 29, 273002,  DOI 10.1088/1361-648X/aa680e



# Contact

If you have any questions about the codes free to contact Prof. Markus Meuwly (m.meuwly@unibas.ch)
