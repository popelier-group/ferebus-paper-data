# Swarm Updater

This directory contains the training set and validation set along with the configuration files used to test the effect of the FEREBUS PSO swarm updater. The training and validation sets for the C1 atom of glycine was taken from the following: [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006). Each subdirectory contains the configuration file for the respective swarm updater and can be ran by making a symlink to the training set then run FEREBUS using:
```
./ferebus > ${PWD##*/}.log
```
