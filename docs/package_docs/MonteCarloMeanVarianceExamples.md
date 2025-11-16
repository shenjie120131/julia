# MonteCarloMeanVarianceExamples.jl

This directory collects example scripts demonstrating Monte‑Carlo estimation of mean and variance for various probability distributions.  It serves as a pedagogical resource rather than a reusable library.

## Key Features

- Illustrates Monte‑Carlo simulation techniques.
- Uses random sampling and statistical summaries.

## Dependencies

The examples rely on Julia’s `Distributions`, `Random`, `Statistics`, `Plots` and `StatsBase` packages.  These dependencies will need C++ equivalents such as `<random>`, Boost.Random, and `matplotlib` for plotting (if visualizations are desired).

## Notes for C++ Port

Porting these examples entails implementing random sampling from various distributions (e.g.\ normal, uniform) using C++’s random facilities and computing sample statistics.  Plots can be produced via Python’s matplotlib when called from the Python wrapper.
