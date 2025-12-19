# RIC: A Solver-Observable Proxy for Proof-Theoretic SAT Hardness

**Version 2.0 - December 2025**

[![DOI] https://doi.org/10.5281/zenodo.17970752

---

## Overview

This repository contains the paper and experimental code for **RIC (Resolution Information Complexity)**, a solver-observable proxy for proof-theoretic SAT hardness that operates orthogonally to structural measures.

### Key Results

- **Orthogonality**: ρ(RIC, Treewidth) = -0.218 (vs. typical ρ > 0.95)
- **Predictive utility**: +39.8% relative improvement in combined models
- **Sample**: 653 random 3-SAT instances

### Positioning

RIC is explicitly positioned as an **empirical proxy**, not a formal complexity measure. It demonstrates that proof-theoretic information forms a dimension largely orthogonal to structural SAT measures.

---

## Repository Structure

```
RIC-proof-theoretic-sat-hardness/
├── latex/
│   └── main.tex          # Complete paper (v2.0)
├── figures/
│   ├── fig1_models.png
│   ├── fig2_correlation.png
│   ├── fig3_scatter.png
│   └── fig4_distribution.png
├── paper/
│   └── [experiment scripts and data]
├── README.md             # This file
└── LICENSE
```

---

## Quick Start

### Compile the Paper

```bash
cd latex/
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Output: `main.pdf`

### Or Use Overleaf

1. Upload all files from `latex/` and `figures/`
2. Set `main.tex` as main document
3. Compile

---

## What Changed in v2.0

📄 **Paper (PDF):**
https://github.com/nizaramama/RIC-proof-theoretic-sat-hardness/blob/main/paper/RIC_v2.0_final.pdf

### Major Updates

**1. Positioning**
- ✅ Repositioned as "proxy not measure"
- ✅ Added "Scope and Positioning" section
- ✅ Added "Measure vs Proxy" discussion
- ✅ Comprehensive limitations section

**2. Framework**
- ✅ Split Conceptual (ideal) vs Practical (computed)
- ✅ Simplified J_poly (removed φ_phase)
- ✅ Clear uncomputability remarks

**3. Experiments**
- ✅ Strong disclaimer for crafted instances (n=10)
- ✅ Focus on 653 random 3-SAT results
- ✅ No quantitative claims from small samples

**4. Discussion**
- ✅ Epistemic humility throughout
- ✅ SAT-only limitation acknowledged
- ✅ Future work clearly specified

### Title

```
v1.0: "Reflective Information Complexity: A Proof-Theoretic 
       Complement to Structural SAT Hardness Prediction"

v2.0: "RIC: A Solver-Observable Proxy for 
       Proof-Theoretic SAT Hardness"
```

---

## Citation

```bibtex
@misc{amama2024ric,
  title={RIC: A Solver-Observable Proxy for Proof-Theoretic SAT Hardness},
  author={Amama, Nizar},
  year={2024},
  note={Version 2.0},
  doi={10.5281/zenodo.17968982},
  url={https://github.com/nizaramama/RIC}
}
```

---

## Key Features

### What RIC Is

- ✅ Computable proxy for proof-theoretic hardness
- ✅ Validated through correlation and prediction
- ✅ Useful for solver portfolios
- ✅ Orthogonal to structural measures

### What RIC Is Not

- ❌ Formal complexity measure
- ❌ Proof technique for P≠NP
- ❌ Complete without UNSAT extension

---

## Results Summary

| Model | R² | Improvement |
|-------|-----|-------------|
| Treewidth only | 25.29% | — |
| RIC only | 13.90% | — |
| **TW + RIC** | **35.36%** | **+39.8%** |

**Correlation:** ρ = -0.218, p < 10⁻⁴

---

## Figures

All figures are in `figures/` directory:

1. **fig1_models.png** - Model performance comparison
2. **fig2_correlation.png** - RIC-treewidth correlation
3. **fig3_scatter.png** - Scatter plot
4. **fig4_distribution.png** - RIC distribution

---

## Limitations

1. **SAT-only scope** - No UNSAT/DRAT analysis
2. **Compression proxy** - LZMA is crude approximation
3. **Solver dependence** - Depends on CDCL implementation
4. **Benchmark bias** - Random 3-SAT may not generalize
5. **Model simplicity** - Linear models may understate interactions

---

## Future Work

### Short-term (6-12 months)
- Extend to UNSAT with DRAT proofs
- Comprehensive crafted benchmarks (n≥100 per family)
- Solver comparison (CryptoMiniSat, Kissat)

### Medium-term (1-2 years)
- Industrial instance validation
- Hybrid S3R integration
- Theoretical connection to resolution width

### Long-term (3-5 years)
- Formal grounding
- Extensions to SMT/CSP
- Learned compression methods

---

## Dependencies

### For LaTeX
- TeX distribution (TeX Live, MiKTeX, or MacTeX)
- pdflatex
- bibtex

### For Experiments (see paper/ directory)
- Python 3.8+
- Glucose 4.0
- LZMA SDK
- R 4.0+ (for statistical analysis)

---

## Contact

**Author:** Nizar Amama  
**Email:** amamanizar@gmail.com  
**ORCID:** [0009-0004-6721-1117](https://orcid.org/0009-0004-6721-1117)

---

## License

This work is licensed under CC BY 4.0

---

## Acknowledgments

Thanks to the SAT solving and complexity theory communities for foundational work that made this research possible.

---

## Version History

- **v2.0** (December 2024): Complete revision with proxy positioning
- **v1.0** (November 2024): Initial release

---

## Links

- **GitHub:** https://github.com/nizaramama/RIC
- **Zenodo:** https://doi.org/10.5281/zenodo.17970752
- **ORCID:** https://orcid.org/0009-0004-6721-1117

---

**Status:** ✅ Publication-ready
