# Optimal Radio Antenna Placement — Unconstrained Optimization

This project aims to determine the **optimal position for a radio antenna** within a 2D city-like environment, maximizing signal efficiency while minimizing interference.

### Problem Summary

- **Buildings**: Attract signal — each has a population and position.
- **Anti-buildings**: Repel signal — positioned randomly and penalize signal strength near them.
- **Objective**: Find antenna coordinates \((a, b)\) minimizing a custom cost function that combines:
  - Weighted distances to buildings
  - Penalties from proximity to anti-buildings

### Methodology

- **Optimization algorithms implemented from scratch**:
  - Newton’s Method
  - Davidon-Fletcher-Powell (DFP)
- Both methods are compared in terms of:
  - Convergence speed
  - Robustness to initial guess
  - Computational efficiency

### Results (Example)

| Method | Min Coordinates      | Cost    | Iterations | Time (s) |
|--------|----------------------|---------|------------|----------|
| Newton | (36.06, 31.33)       | ~74.59  | 32         | 0.02     |
| DFP    | (36.07, 31.31)       | ~74.59  | 41         | 0.05     |

### Project Files

- `Seminar_Notebook.ipynb`: Full explanation, code, visualizations, and comparisons.
- `README.md`: Project summary.

### Authors

Melchior Thierry, Victor Pierron, Oscar Pastural, Richard Goudelin

---

📎 *See the notebook for full mathematical formulation, implementation, and visualization.*
