# Changelog

All notable changes to this package. Versions follow semver, independent of the Nabi toolchain.

## 0.1.1 (2026-11-22)

- The crate docs now carry the fitting and optimization tutorial (roots,
  minimization, bounds, curve fitting, linear programming), moved from
  the Nabi docs site; its examples run as doc tests.

## 0.1.0 (2026-11-22)

First release.

- Scalar roots (`brentq`, `toms748`, `newton`, `halley`, and more) and
  scalar minima (`golden`, `brent`, `minimize_scalar`).
- Unconstrained minimization: Nelder-Mead, Powell, CG, BFGS, L-BFGS,
  Newton-CG, trust regions (`minimize`).
- Bounds and constraints: `lbfgsb`, `projected_gradient`, `Constraint`,
  `auglag`.
- Linear and quadratic programs: `Lp`, `Qp`, `linprog` (simplex, interior
  point), `quadprog`.
- Least squares and curve fitting: `least_squares` (`Lm`, `Trf`),
  `curve_fit`, robust `Loss`es.
- Systems of equations (`root`, `hybr`, `broyden`) and global search
  (`differential_evolution`, `basin_hopping`, `simulated_annealing`).
- Objectives over `f64`, `Dual`, `Var` or `Complex<f64>`, or an `Objective`
  with known derivatives; finite-difference and complex-step helpers.
- The `ops` feature (default): `ε`, `⩽`, `⩾`, `≐`, `∇`, `∂`. f64, pure
  Nabi, every target including wasm. Needs Nabi 0.1 or later; depends on
  `linalg` and `autodiff`.
