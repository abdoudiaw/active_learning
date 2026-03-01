# active_learning

Exploring active-learning methods inspired by:

Lookman et al., "Active learning in materials science with emphasis on adaptive sampling using uncertainties for targeted design" (npj Computational Materials, 2019).

## Notebooks

- `notebooks/active_learning_pure_python.ipynb`
  - Pure Python core loop (no NumPy / scikit-learn required)
  - Toy 1D test function
  - Uncertainty sampling vs targeted sampling vs random baseline
  - Optional plotting if `matplotlib` is available

- `notebooks/lookman_gp_targeted_design.ipynb`
  - GP surrogate with prediction mean and uncertainty bars
  - Uses the polynomial objective shown in the paper figure caption
  - Reproduces the paper-style two-panel flow: initial fit and after iteration 1
  - Prints prediction results (`mu`, `std`) at probe points before/after update
