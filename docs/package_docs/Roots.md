# Roots.jl

**Roots.jl** offers a variety of numerical root‑finding algorithms for univariate functions, including bracketing and open methods.  It is widely used as a dependency in other Julia packages.

## Key Features

- Implements algorithms such as bisection, secant, Newton, Halley, and Brent’s methods.
- Handles functions with multiple roots and provides convergence diagnostics.
- Serves as a foundation for higher‑level packages such as CharFuncPricing and AQFED.

## Dependencies

Roots.jl primarily depends on Julia’s standard libraries (`LinearAlgebra`, `Statistics`, `Printf`, `Random`) and test utilities.

## Notes for C++ Port

These root‑finding algorithms can be ported using C++ templates.  Boost.Math and the C++ standard library provide some of these methods; others can be implemented directly.  Refer to `docs/Julia_to_C++_porting.md` for guidance.
