# Julia Repository Setup and Cloning Instructions

This repository contains high-level documentation and porting instructions for several Julia packages originally authored by **Jherek Healy**. To work with the actual code, you need to clone each of the original repositories.

## Clone the required repositories

Open a terminal in the folder where you want to keep the code and run:

```bash
git clone https://github.com/shenjie120131/PPInterpolation.jl.git
git clone https://github.com/shenjie120131/CharFuncPricing.jl.git
git clone https://github.com/shenjie120131/AQFED.jl.git
git clone https://github.com/shenjie120131/LaverySpline.jl.git
git clone https://github.com/shenjie120131/MonteCarloMeanVarianceExamples.jl.git
git clone https://github.com/shenjie120131/Roots.jl.git
```

These commands will create a local copy of each Julia package.

## Next steps

1. **Read the READMEs** in each repository to understand their purpose and dependencies.
2. **Review the document** `docs/Julia_to_C++_porting.md` in this repository for a structured migration plan from Julia to C++ and instructions for creating Python bindings.
3. **Use the provided guide** to port the numerical algorithms to C++ (using Eigen, Boost, FFTW, NLopt, etc.) and test them via Python.

If you have already cloned the repositories, you can skip the `git clone` commands and proceed directly to the porting guide.
