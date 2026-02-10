# QAOA for MaxCut – Research Summary

## What the literature claims
- QAOA can approximate MaxCut with increasing depth p
- For p → ∞, converges to optimal solution
- Small p may already outperform random guessing

## What is realistic today
- Practical implementations limited to p ≤ 2
- Parameter optimization is nontrivial
- Noise significantly affects performance on hardware

## Mapping to Qiskit
- QAOA implemented via `qiskit.algorithms.minimum_eigensolvers.QAOA`
- Uses parameterized circuits + classical optimizer
- Straightforward to simulate

## Initial skepticism
- Brute force is trivial for small graphs
- Classical heuristics already excellent
- No obvious path to scaling on NISQ devices

