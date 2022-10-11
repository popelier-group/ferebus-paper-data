# Stopping Criteria

This directory contains the files used to analyse the FEREBUS stopping criteria parameters. The `inputs` directory contains the training and validation sets for the C1 atom of glycine taken from the following: [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006). The `outputs` directory contains the configuration files for each stopping criteria parameter combination. To run each test, a symmlink to the training set can be created and FEREBUS can be ran with the following:
```
./ferebus > ferebus.log
```
