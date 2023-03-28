# hawkes-markov

---


### Introduction

This repository contains the code used for computation and simulation studies of the paper: **Markovian multivariate Hawkes population processes: efficient evaluation of moments**. It covers the class of multivariate Hawkes processes with exponential decay. It further allows for random marks, which in this setting entails that its intensity jumps according to a random jump size $B_{ij}$. Further, we consider the _population process_, which allows for events to depart from the system; in this setting the sojourn time is taken to be Exponentially decaying.

---


### Code

The Initialization Jupyter Notebook contains the relevant packages and introduces the parameters needed to run the code. Each Jupyter Notebook contains functions for a specific method of computing moments. All the specific methods refer to sections of the paper and were used to obtain the results in the numerics section. There are three main ways to obtain transient moments:

1. _Benchmark_ (BM) method: this is an _ODE method_ in the d=3 setting and it is a _block-matrix method_ in the d=2 setting.
2. _Finite Difference_ (FD) of the Joint Transform.
3. _Monte Carlo_ (MC) simulation based on Ogata's thinning algorithm.

We also find a way to compute stationary moments, which are solves using Sylvester equations. It is emphasized that in this code, the random jump sizes $B_{ij}$ are  Exponentially distributed. This is important since (combinations of) the moments of $B_{ij}$ appear in the often convoluted expressions of large matrices and constants.


---

### References

- _Karim, R.S., Laeven, R.J.A. & Mandjes, M. (2023)._ Markovian multivariate Hawkes population processes: efficient evaluation of moments.
- _Ogata, Y. (1981)._ On Lewis' simulation method for point processes. _IEEE Transactions on Information Theory 27, 23-31._
