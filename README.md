# Applied Statistics — Take-Home Exam (2020)

Solutions to the take-home exam of **Applied Statistics: From Data to Results**,
a course by professor Troels C. Petersen from the MSc in Bio- and Medical Physics at the **Niels Bohr Institute,
University of Copenhagen**. The exam covers core statistical-analysis topics through
five themed sections, worked out in Python.

> Reworked as a self-study exercise to sharpen data-analysis and scientific-computing
> skills.

## Contents

The notebook is organised by exam section:

| Section | Topic | Problems |
|--------|-------|----------|
| I   | Distributions & probabilities | 1.1 Binomial (even score), 1.2 Geometric / "at least one hit" |
| II  | Error propagation             | 2.1 Weighted average (Hubble tension), 2.2 Coulomb-law uncertainty & optimal distance, 2.3 Neanderthal-DNA distribution fit |
| III | Monte Carlo                   | 3.1 Accept/reject sampling, Pearson correlation, binned χ² fit, required statistics |
| IV  | Statistical tests             | 4.1 Type I/II errors, separation power & ROC/AUC, Fisher linear discriminant |
| V   | Fitting data                  | 5.1 Kepler's third law & solar-mass estimate, 5.2 LHC β-calibration |

## Methods used

- **Probability distributions**: binomial, geometric, Gaussian
- **Error propagation** and inverse-variance weighted averages
- **χ² goodness-of-fit** tests and p-values
- **Monte Carlo** generation (accept/reject method)
- **Hypothesis testing**: type I/II errors, separation power, symmetry tests
- **Classification**: ROC curves, AUC, Fisher linear discriminant
- **Curve fitting** (`scipy.optimize.curve_fit`), parameter covariance & correlation
- **Multivariate calibration** via least squares

## Tech notes

- **Python** with `numpy`, `scipy`, and `matplotlib`.
- Developed with **`numpy < 2.0`** — uses `np.trapz` (renamed `np.trapezoid` in newer versions).
- Plots are rendered inline; nothing is written to disk.

## Data

Problems 2.3, 4.1 and 5.2 read text files expected in a local `data/` folder
next to the notebook:

```
data/
├── data_DNAfraction.txt      # 2.3  Neanderthal DNA fractions (2318 students)
├── data_Cells.txt            # 4.1  cell length & transparency (4690 cells)
└── data_BetaCalibration.txt  # 5.2  β, θ, E, T  (4000 control-sample particles)
```

Original data files were distributed via the course web page.


## Acknowledgements

The exam problems and accompanying datasets were created by **Prof. Troels C. Petersen**
and the teaching team of the *Applied Statistics: From Data to Results* course at the
Niels Bohr Institute, University of Copenhagen. All credit for the problem design and
data belongs to them. The solutions and code in this repository are my own work,
shared for educational and portfolio purposes only.

Course material: <https://www.nbi.dk/~petersen/Teaching/AppliedStatistics2019.html>

---
