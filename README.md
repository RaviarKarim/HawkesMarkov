# hawkes-markov

---


### Introduction

This repository contains the code used for computation and simulation studies of the paper: **Markovian multivariate Hawkes population processes: efficient evaluation of moments**. It covers the class of multivariate Hawkes processes with exponential decay. It further allows for random marks, which in this setting entails that its intensity jumps according to a random jump size $B_{ij}$. Further, we consider the _population process_, which allows for events to depart from the system; in this setting the sojourn time is taken to be Exponentially decaying.

---


### Code

The Initialization Jupyter Notebook contains the relevant packages and introduces the parameters needed to run the code. Each Jupyter Notebook contains functions for a specific method of computing moments. All the specific methods refer to sections of the paper and were used to obtain the results in the numerics section. It is emphasized that in this code, the random jump sizes $B_{ij}$ are Exponentially distributed. This is important since the moments of $B_{ij}$ appear in the often convoluted expressions of large matrices and constants.



---

### References

- R.S. Karim, R.J.A. Laeven & M. Mandjes (2023). _Markovian multivariate Hawkes population processes: efficient evaluation of moments_.
- Ogata thinning algorithm paper
