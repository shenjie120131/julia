# PPInterpolation.jl

This directory contains the Julia package **PPInterpolation.jl**.  The package implements piecewise‑polynomial interpolation routines, including B‑spline and polynomial interpolants, used for constructing smooth functions from tabular data.

## Key Features

- Support for B‑spline interpolation and evaluation.
- Construction of piecewise polynomial interpolants.
- Utilities for evaluating interpolants and computing derivatives.

## Dependencies

The original Julia package lists the following dependencies in its `Project.toml` file: `BSplines`, `BenchmarkTools`, `ForwardDiff`, `LinearAlgebra`, `QuadGK`, `Random`, `SpecialFunctions` and `Test`【252709605493385†screenshot】.

## Notes for C++ Port

The algorithms implemented here will need to be ported to C++ using appropriate numerical libraries (e.g.\ Eigen for linear algebra, custom routines for B‑splines and quadrature).  See `docs/Julia_to_C++_porting.md` for guidance.
