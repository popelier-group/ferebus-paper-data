# Active Dimensions

This directory contains the training and validation sets generated using the following function:
```
y = -0.1*x1^2 + sin(x2+pi/2)+1
```
where `x1` and `x2` correspond to the features `f1` and `f2` in the training and validation set files and represent the first and second dimension of the input respectively.

The training set inputs (`f1` and `f2`) were generated using a uniform random distribution in the range of [-8.5, 8.5] and validation set inputs were generated using a uniform random distribution in the range of [-15, 15].

The RBF model can be generated using the `rbf.toml` configuration file as follows:
```
./ferebus -c rbf.toml
```

The periodic model can be generated using the `per.toml` configuration file as follows:
```
./ferebus -c per.toml
```

The RBF+periodic model can be generated using the `rbf.toml` configuration file as follows:
```
./ferebus -c rbf+per.toml
```
