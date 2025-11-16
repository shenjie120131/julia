# AQFED.jl

**AQFED.jl** is a collection of algorithms for advanced financial engineering.  It contains tools for Monte‑Carlo simulations, spline approximations, root finding and optimization used in derivative pricing and risk analysis.

## Key Features

- Implements a broad set of numerical methods for pricing exotic derivatives.
- Integrates interpolation (via PPInterpolation), characteristic function pricing (via CharFuncPricing) and root‑finding (via Roots).
- Includes optimization models using JuMP/COSMO and convex solvers.

## Dependencies

The package has a large dependency graph: `AbstractAlgebra`, `BSplines`, `COSMO`, `CharFuncPricing`, `Colors`, `Convex`, `DSP`, `DataFrames`, `DelimitedFiles`, `Dierckx`, `Distributions`, `DoubleExponentialFormulas`, `FFTW`, `FastGaussQuadrature`, `FiniteDifferences`, `ForwardDiff`, `HypergeometricFunctions`, `Images`, `LeastSquaresOptim`, `LinearAlgebra`, `LsqFit`, `Measures`, `NLsolve`, `OffsetArrays`, `Optim`, `PPInterpolation`, `Polynomials`, `PolynomialRoots`, `QuadGK`, `Random`, `RandomNumbers`, `Revise`, `Roots`, `Sobol`, `SparseArrays`, `SpecialFunctions`, `Statistics`, `StatsBase`, `TaylorSeries`, `Test` and more【3862225395296†screenshot】.

## Notes for C++ Port

Porting AQFED requires porting its dependent modules first (PPInterpolation, CharFuncPricing, Roots) and then rewriting its composite algorithms using C++ numerical libraries.  See the porting guide in `docs/Julia_to_C++_porting.md`.
