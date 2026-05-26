# Quantum RNE Empirical Scaling Experiments

This repository contains numerical experiments for **"Optimal Quantum Speedups for Repeatedly Nested Expectation Estimation"**.

The main notebook, `scaling_experiments.ipynb`, provides two empirical checks:

- **QAMC building block:** compares classical Monte Carlo scaling against Quantum Amplitude Estimation using Qiskit's Iterative Amplitude Estimation.
- **Per-level variance decay:** verifies the approximate `2^-n` variance decay of MLMC telescoping differences in a concrete nested expectation setting.

## Repository Contents

- `scaling_experiments.ipynb` - Jupyter notebook containing the experiments, plots, and discussion.
- `requirements.txt` - pinned Python dependencies used for the notebook.

## Setup

The notebook was prepared with Python 3.12.7.

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
pip install notebook ipykernel
```

Register the Jupyter kernel:

```bash
python -m ipykernel install --user --name quantum-rne --display-name "Quantum RNE"
```

Start Jupyter:

```bash
jupyter notebook
```

Then open `scaling_experiments.ipynb` and select the `Quantum RNE` kernel.

## Notes

The notebook includes saved outputs so the plots are visible when browsing the repository on GitHub. To regenerate the results, rerun the notebook from top to bottom in the environment above.

