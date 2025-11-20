# Machine Learning Potential for tobermorite and C-S-H Systems

# Introduction
This work develops a Neuroevolution Potential (NEP) suitable for tobermorite and C-S-H systems. The versatility of the NEP is demonstrated by predicting the structural and mechanical properties of tobermorite, and it is applied for the first time to MD simulations of amorphous configurations. This repository provides the dataset, training scripts, and MD examples for the NEP model.

# Usage
1.NEP Training and Testing.
Run the following command:

cd 01-NEP-tob-C-S-H ln -s train-440.xyz train.xyz 

../../ GPUMD-master/src/nep &

2.MD simulation.
This example runs with GPUMD. For the GPUMD source code and compilation instructions, please refer to the official installation guide: https://gpumd.org/installation.html. This NEP potential can also be used in LAMMPS. To use it within LAMMPS, simply compile the code with NEP-related packages enabled.

cd 02-Examples-MD/Tobermorite-NPT

ln -s model-9A.xyz model.xyz

../../ GPUMD-master/src/gpumd>nep.log &

# Literature link
https://doi.org/10.1016/j.cemconres.2025.108091
