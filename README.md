# Grand Proof I — Publication Package (Grand Proof Series I)

> **Türkçe:** [README_TR.md](./README_TR.md)

**Grand Proof I: Dark-Matter-Free Galactic Dynamics, the Meral Cosmic Acceleration Scale, SPARC Rotation Curves, and EHT Black-Hole Ring Evidence**

Author: Fahri Meral · Date: October 19, 2026 · Version: v1 (Grand Proof I)

> **Status:** Unpublished preprint (v1). Not peer-reviewed.

## Contents

| File | Description |
|---|---|
| `paper/grand_proof_I_galaktik_dinamik.tex` | Main paper, Turkish (Tables 1–3, Figure 1 2×2) |
| `paper/grand_proof_I_galactic_dynamics_EN.tex` | English version |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.pdf` | Tests T29–T31 figure (TR, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.png` | Tests T29–T31 figure preview (TR) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.pdf` | Tests T29–T31 figure (EN, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.png` | Tests T29–T31 figure preview (EN) |
| `CITATION.cff` | Citation record |
| `LICENSE` | CC BY 4.0 |

## Results (zero free parameters)

- Meral scale `a_Meral = 1.146589e-10 m/s²` vs SPARC `a_0 = 1.20e-10` (4.45%, 0.22σ_sys).
- BTFR slope exactly 4.000000000000000 (R² = 1.0); 5 SPARC archetypes mean 4.54%
  (UGC 2885 is an openly reported 12.9% outlier).
- EHT rings: Sgr A* 50.31 μas (0.65σ), M87* 38.31 μas (1.23σ).

## Numerical reproduction

Tests T29–T31 are produced with the solver in the **Paper V repository**
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py   # T1–T31 (31/31 PASS)
python duran_sicimler_sim/mini_check_gp1.py  # independent cross-check (15/15 PASS)
```

The independent cross-check never imports the solver.
Figure 1 is produced by the `fig13` function in `generate_figures.py`.
