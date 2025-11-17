# CharFuncPricing.jl

**CharFuncPricing.jl** provides pricing routines for financial derivatives using characteristic functions.  It implements Fourier and FFT‑based pricing methods and integrates special functions and root‑finding algorithms.

## Key Features

- Pricing options and derivatives via characteristic functions of stochastic processes.
- Support for FFT and double‑exponential integration techniques.
- Uses automatic differentiation for gradient computations.

## Dependencies

According to the package’s `Project.toml`, it depends on `AbstractFFTs`, `BenchmarkTools`, `DoubleExponentialFormulas`, `FastGaussQuadrature`, `ForwardDiff`, `LinearAlgebra`, `MFFT`, `Nemo`, `Optim`, `Revise`, `Roots`, `SpecialFunctions`, `StatsBase`, and `TestEnv`【851296527575676†screenshot】.

## Notes for C++ Port

FFT‑based pricing routines should be implemented using FFTW or Eigen’s FFT capabilities.  Root‑finding and optimization can be replaced with Boost’s root‑finding tools and NLopt/Ceres.  Refer to `docs/Julia_to_C++_porting.md` for details.
