# LaverySpline.jl

**LaverySpline.jl** provides implementations of Lavery’s rational cubic splines.  These splines are used to fit smooth curves subject to shape constraints.

## Key Features

- Rational cubic spline interpolation.
- Support for fitting splines with shape constraints via optimization.
- Depends on PPInterpolation for underlying polynomial interpolation.

## Dependencies

From its `Project.toml`, the package depends on `Cbc` (branch‑and‑cut solver), `JuMP` (for modelling optimization problems), `LinearAlgebra` and `PPInterpolation`【689619311621031†screenshot】.

## Notes for C++ Port

Rational spline algorithms must be ported to C++ (custom implementation may be required).  Optimization problems formulated in JuMP should be expressed using a C++ optimization library such as Cbc or NLopt.
