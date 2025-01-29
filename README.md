# Geodesics in Heat Implementation

## Overview

This repository contains an implementation of the "Geodesics in Heat" method for approximating geodesic distances on surface manifolds. The implementation is applied to triangular simplicial meshes.

## Contents

- **Report:** A detailed PDF report explaining the method, implementation, and evaluation results.
- **Python Notebook:** A Jupyter Notebook containing the implementation of the method, including visualization of results.
- **Sample Mesh Data:** Stanford Bunny mesh used for evaluation.

## Methodology

The heat method can be broken down into four main steps:

1. **Discrete Heat Flow:** Solve the heat equation over the mesh to compute heat distribution.
2. **Normalized Vector Field:** Compute the gradient of the heat distribution and normalize it.
3. **Divergence of the Vector Field:** Compute the divergence to prepare for solving the Poisson equation.
4. **Poisson Equation:** Solve for the scalar potential to approximate geodesic distances.

### Libraries Used

- `python==3.9.18`
- `scipy==1.11.4`
- `trimesh==4.0.9`
- `libigl==2.5.1`
- `numpy==1.26.3`
- `matplotlib==3.8.0`

## Installation

To run this implementation, install the required dependencies using:

```sh
pip install scipy trimesh libigl numpy matplotlib
```

## References

- K. Crane, C. Weischedel, and M. Wardetzky, “Geodesics in heat: A new approach to computing distance based on heat flow,” ACM Transactions on Graphics, vol. 32, no. 5, p. 1–11, Sep. 2013. [DOI](http://dx.doi.org/10.1145/2516971.2516977)

