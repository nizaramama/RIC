# RIC: A Solver-Observable Proxy for Proof-Theoretic SAT Hardness

**Author:** Nizar Amama  
**ORCID:** 0009-0004-6721-1117  
DOI (Zenodo, v2): https://doi.org/10.5281/zenodo.17968982

---

## Overview

This repository contains the paper and supplementary material for:

> **RIC (Resolution Information Complexity): A Solver-Observable Proxy for
> Proof-Theoretic SAT Hardness**

RIC is an **empirical, solver-observable proxy** designed to approximate
proof-theoretic hardness in SAT instances using:
- Compression-based approximations to time-bounded Kolmogorov complexity
- CDCL solver dynamics (conflicts, propagations, decisions)

RIC is **not a formal complexity measure**.  
It is a **foundation contribution** demonstrating that proof-theoretic
information constitutes a dimension *orthogonal* to structural SAT measures
(e.g., treewidth).

---

## Key Findings

- Ultra-low correlation with treewidth: ρ = -0.218 (n = 653)
- Standalone predictive power: R² = 13.90%
- Combined with treewidth: +39.8% improvement in R²
- Demonstrates an empirical orthogonal dimension of SAT hardness

---

## Epistemic Positioning

- **What RIC is:**  
  A solver-observable *proxy* for proof-theoretic hardness.

- **What RIC is not:**  
  A formal complexity measure or a proof-theoretic invariant.

Current experiments focus on **satisfiable (SAT)** instances.
Extension to **UNSAT + DRAT proof analysis** is ongoing future work.

---

## Files

- `RIC_SAT_Paper_v2.pdf` — revised paper (proxy positioning)
- `paper/` — LaTeX sources (if applicable)
- `figures/` — figures used in the paper

---

## Citation

If you use this work, please cite it via the Zenodo DOI.
