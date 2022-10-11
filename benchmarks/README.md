# FEREBUS Benchmarks

This directory contains the training set can configuration file used to run the FEREBUS benchmarks. The training set is taken from the C1 glycine model in the following: [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006). FEREBUS can be compiled for the GPU using either the PGI or nvidia compilers then the CPU and GPU binaries (`ferebus_cpu` and `ferebus_gpu` respectively) can be benchmarked using the following (up to 16 cores):
```bash
#!/bin/bash

nprocs=(1 2 4 8 16)

for nproc in ${nprocs[@]}; do
  export OMP_NUM_THREADS=$nproc
  ./ferebus_cpu > cpu_$nproc.log
  ./ferebus_gpu > gpu_$nproc.log
done
```
