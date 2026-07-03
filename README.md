# Life

**Computational actuarial modelling of longevity risk using Gompertz–Makeham mortality, compound-Poisson FFT aggregation, and structural longevity scenarios.**

## Overview

This repository contains a reproducible actuarial modelling project investigating the distinction between **diversifiable (idiosyncratic)** and **systematic (undiversifiable)** longevity risk in a stylised occupational pension fund.

The project combines classical actuarial mortality modelling with modern open-source scientific computing in Python. Its emphasis is on transparency, reproducibility and computational efficiency rather than methodological novelty.

The accompanying technical note demonstrates how structural longevity scenarios can be analysed using an exact aggregate liability distribution computed by Fast Fourier Transform (FFT) convolution.

---

## Features

- Gompertz–Makeham mortality modelling
- Income-segmented mortality calibration
- Structural longevity scenarios (timing × magnitude)
- Independent Solvency II longevity benchmark
- Compound-Poisson aggregate liability model
- Exact FFT aggregation
- Best Estimate Liability (BEL)
- Value-at-Risk (VaR)
- Tail Value-at-Risk (TVaR)
- Validation against independent Monte Carlo simulation
- Fully reproducible figures and tables

---

## Repository contents

| File | Description |
|------|-------------|
| `PensionFund.ipynb` | Main Jupyter notebook implementing the actuarial model. |
| `pension_paper.docx` | Technical note describing the methodology, assumptions and results. |

---

## Main result

For a large occupational pension fund, the stochastic demographic risk arising from independent deaths is small because it diversifies across members.

The dominant demographic uncertainty comes from **systematic improvements in longevity**, which affect the entire portfolio simultaneously and therefore cannot be diversified away.

The repository provides a reproducible computational framework for quantifying both components and comparing them with the standard Solvency II longevity stress.

---

## Technologies

- Python
- Jupyter Notebook
- NumPy
- Pandas
- SciPy
- Matplotlib
- `aggregate` (Stephen J. Mildenhall)

---

## Purpose

This repository accompanies a technical note on computational actuarial modelling. It is intended as a transparent and reproducible research implementation rather than production software.

Comments, suggestions and constructive criticism are welcome.

---

## Author

**Erik Van Releghem**
