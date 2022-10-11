# Likelihood Functions

This directory contains the data used to compare likelihood (concentrated vs marginal) functions. The following system/atoms were used:
| System     | Atom | Source                                                                 |
| ---------- | ---- | ---------------------------------------------------------------------- |
| Water      | O1   | [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006) |
| Ammonia    | N1   | [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006) |
| Methanol   | C1   | [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006) |
| NMA        | C1   | [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006) |
| Glycine    | C1   | [https://doi.org/10.1002/jcc.27006](https://doi.org/10.1002/jcc.27006) |
| Ibuporofen | C1   | Under Review                                                           |

All data sets were generated using the same active learning method from an AIMD simulation using CP2K with the exception of ibuprofen which was generated using a 500 K AMBER simualtion and a variance based sampling method.

Each directory contains the training and validation sets alongside a `marginal` and `concentrated` directory containing the configuration file and FEREBUS results. To run FEREBUS, a symmlink can be created in the directory and ran with the following:
```
./ferebus > ferebus.log
```
- 
