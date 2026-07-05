# Longevity Risk Modelling

![Computational framework](figures/figure1_clean.svg)

**Computational actuarial modelling of longevity risk using Gompertz–Makeham mortality, compound-Poisson aggregation, Fast Fourier Transform (FFT), and structural longevity scenarios.**

---

## Overview

This repository contains a reproducible actuarial modelling framework for analysing **idiosyncratic** and **systematic** longevity risk in a stylised occupational pension fund.

The implementation combines classical actuarial modelling with modern scientific computing in Python. A structural longevity transformation allows an entire grid of longevity scenarios to be evaluated by **the same compound-Poisson FFT valuation engine**: only the mortality transformation changes, while survival reconstruction, cash-flow projection and stochastic aggregation remain identical.

The accompanying technical note demonstrates how systematic longevity stresses can be analysed through exact aggregate liability distributions computed by Fast Fourier Transform (FFT) convolution.

---

## Main Results

The notebook illustrates several actuarial observations:

- The random variation arising from independent individual deaths is almost completely diversified in a large pension fund.
- Systematic longevity improvements remain undiversifiable and dominate demographic uncertainty.
- Two structural longevity scenarios exceed the standard Solvency II −20% longevity stress.
- Interest-rate assumptions have a larger financial impact than plausible longevity improvements, while longevity shocks also increase interest-rate sensitivity.
- Exact compound-Poisson FFT aggregation reproduces Monte Carlo results to numerical precision while requiring only a fraction of the computation.

---

## Features

- Gompertz–Makeham mortality model
- Income-segmented mortality calibration
- Structural longevity scenario analysis
- Independent Solvency II benchmark
- Compound-Poisson aggregate liability model
- Exact FFT aggregation
- Best Estimate Liability (BEL)
- Value-at-Risk (VaR)
- Tail Value-at-Risk (TVaR)
- Independent Monte Carlo validation
- Reproducible figures and tables

---

## Repository Contents

| File | Description |
|------|-------------|
| `LongevityRisk.ipynb` | Complete computational implementation |
| `LongevityRisk.pdf` | Technical note describing the methodology, assumptions and results |
| `/figures/` | Figures used in the paper and this repository |
| `/data/Deaths_1x1.txt` | Human Mortality Database (Belgium) deaths |
| `/data/Exposures_1x1.txt` | Human Mortality Database (Belgium) exposures |

---

## Requirements

Python 3.12 or later.

Main packages:

- NumPy
- Pandas
- SciPy
- Matplotlib
- aggregate (Stephen J. Mildenhall)

The Human Mortality Database files `Deaths_1x1.txt` and `Exposures_1x1.txt` should be placed in the repository's `data/` directory.

---

## Purpose

This repository accompanies the technical note and provides a transparent, reproducible research implementation.

It is intended for educational, actuarial and research purposes rather than production software.

Comments, suggestions and constructive criticism are welcome.

---

## Citation

If you use this repository in academic or professional work, please cite the accompanying technical note.

---

## Author

**Erik Van Releghem**
