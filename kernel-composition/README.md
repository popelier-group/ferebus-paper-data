# Kernel Composition

This directory contains the training and validation sets generated using the following function:
```
y = 10sin(3x) + 1.2x + e
```
where `e` is a normally distributed random perturbation with a mean of 0 and a variance of 1.

The training set inputs (`x`) were generated using a uniform random distribution in the range [0, 10] and the validation set using a uniform random distribution in the range [-5, 15].

The periodic model can be generated using the `per.toml` configuration file as follows:
```
./ferebus -c per.toml
```

And the periodic+linear model can be generated using the `per+lin.toml` configuration file as follows:
```
./ferebus -c per+lin.toml
```
