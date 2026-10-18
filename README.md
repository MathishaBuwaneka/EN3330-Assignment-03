# EN3330 – Assignment 03

**Introduction to Engineering Optimization | University of Moratuwa**

This repository contains the Python work for Assignment 03. The problems cover Lagrangian duality, saddle-point conditions and weak duality.

## Contents

| File | What it covers |
| --- | --- |
| `notebooks/Q_1_Lagrangian_Duality.ipynb` | Lagrangian curves, the dual function and the primal function |
| `notebooks/Q_2_Saddle_Point.ipynb` | Saddle-point inequalities, complementary slackness and the relaxed constraint |
| `notebooks/Q_3_Weak_Duality.ipynb` | Numerical weak-duality checks and the lower envelope of affine functions |
| `generate_figures.py` | Generates the six figures used in the report |
| `figures/` | PNG versions of the report figures |

## Running the notebooks

The notebooks use Python 3, NumPy and Matplotlib. To install the packages and start Jupyter Notebook:

```bash
python -m pip install -r requirements.txt
jupyter notebook
```

Open a notebook in the `notebooks/` folder and use **Run All**. Each notebook includes the equations, Python code and plots for its question.

To regenerate the six report figures, run:

```bash
python generate_figures.py
```

The script saves the plots in the `figures/` folder.

## Problem considered

The main problem is to minimize $x^2$ subject to $x \geq 1$, with Lagrangian

$$
L(\mu,x)=x^2+\mu(1-x), \qquad \mu \geq 0.
$$

The notebooks check the solutions using mathematical derivations and plotted results.
