# Reflective Information Complexity (RIC)

**Reflective Information Complexity (RIC)** is an information–proof-theoretic measure
designed to capture SAT instance hardness beyond purely structural metrics
such as treewidth.

RIC combines:
- Time-bounded Kolmogorov complexity (solution compressibility)
- Proof-search dynamics (conflicts, propagations, decisions)
- Phase-aware normalization

## 📄 Paper

- **Title:** Reflective Information Complexity: A Proof-Theoretic Complement to Structural SAT Hardness Prediction
- **Author:** Nizar Amama
- **Preprint (Zenodo DOI):** https://zenodo.org/records/17925892
- **arXiv:** (pending endorsement)

PDF available in `paper/`.

## 📊 Key Findings

- Ultra-low correlation with treewidth (ρ ≈ -0.22)
- Standalone predictive power (R² ≈ 14%)
- Strong complementarity with treewidth (+39.8% improvement)
- Sensitivity to proof-hard instances (PHP, Parity)

## 📁 Repository Structure

- `paper/` — manuscript PDF and LaTeX
- `figures/` — plots used in the paper
- `code/` — RIC computation and analysis scripts
- `data/` — experimental results (CSV)
- `docs/` — methodology notes

## 🧪 Reproducibility

The provided code allows recomputation of:
- RIC values
- Correlation analysis
- Regression models
- Figures reported in the paper
 
## Figures

All figures used in the paper are available in the `figures/` directory:
- Model comparison
- Correlation analysis
- Scatter plots
- Distribution analysis
- Summary table

## 📜 License

MIT License (code)  
Paper © 2025 Nizar Amama

## 📬 Contact

- Email: amamanizar@gmail.com
- ORCID: 0009-0004-6721-1117
