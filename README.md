# Stationary Strings XII — Publication Package

> **Türkçe:** [README_TR.md](./README_TR.md)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)

**Stationary Strings XII: Dark-Matter-Free Galactic Dynamics, the Meral Cosmic Acceleration Scale, SPARC Rotation Curves, and EHT Black-Hole Ring Evidence**

Author: Fahri Meral · Date: October 19, 2026 · Version: v1 (Stationary Strings XII)

> **Status:** Unpublished preprint (v1). Not peer-reviewed. *[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23517474-blue.svg)](https://doi.org/10.5281/zenodo.23517474)*

## Contents

| File | Description |
|---|---|
| `paper/stationary_strings_XII_galaktik_dinamik.tex` | Main paper, Turkish (Tables 1–3, Figure 1 2×2) |
| `paper/stationary_strings_XII_galactic_dynamics_EN.tex` | English version |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.pdf` | Tests T29–T31 figure (TR, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.png` | Tests T29–T31 figure preview (TR) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.pdf` | Tests T29–T31 figure (EN, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.png` | Tests T29–T31 figure preview (EN) |
| `CITATION.cff` | Citation record |
| `LICENSE` | CC BY 4.0 |

## Key findings

- **T29 (Theorem XII.1):** zero-parameter Meral cosmic acceleration scale
  `a_Meral = µ_s^Meral (1-η_T0) c H_0 = 1.1465889797e-10 m/s²`
  (Planck 2018 `H_0 = 67.4`), i.e. the model predicts the **dimensionless ratio**
  `κ_Meral = a_0/(cH_0) = 0.175097`. The comparison to the SPARC
  `a_0 = (1.20 ± 0.02 ± 0.24)e-10` is 4.45 % (0.22 σ_sys) with Planck and
  0.06 % with the local `H_0 = 70.5` — the test therefore carries the adopted
  `H_0` and shows *consistency*, not an `H_0`-independent absolute scale.
- **T29/T30 (Theorem XII.2):** string-loop radial acceleration relation
  `g_obs = g_bar[1+(x+x²)^(-1/2)]`, `x = g_bar/a_Meral`, gives the outer-halo
  law `v_flat⁴ = G M_b a_Meral` with log-log slope **4.000000000000000**
  (`R² = 1.0`) and a 4.54 % mean deviation over five SPARC archetypes
  (four below 4.1 %; the giant spiral UGC 2885 is an openly reported 12.9 %
  outlier).
- **T31 (Theorem XII.3):** EHT ring saturation
  `d_ring = 6 θ_g C_univ √(1+µ_s/4) = 10.002404 θ_g`, predicting
  50.31 μas for Sgr A* (0.65 σ) and 38.31 μas for M87* (1.23 σ) against the
  51.8 ± 2.3 μas and 42.0 ± 3.0 μas measurements.

## Numerical reproduction

Tests T29–T31 are produced with the solver in the **Paper V repository**
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py     # T1–T31 (31/31 PASS)
python duran_sicimler_sim/mini_check_gp1.py    # independent cross-check (15/15 PASS)
```

The independent cross-check never imports the solver. Figure 1 is produced by
the `fig13` function in `duran_sicimler_sim/generate_figures.py`.

## Citation

```bibtex
@misc{meral2026grandproofi,
  author = {Fahri Meral},
  title  = {Stationary Strings XII: Dark-Matter-Free Galactic Dynamics, the Meral Cosmic Acceleration Scale, SPARC Rotation Curves, and EHT Black-Hole Ring Evidence},
  year   = {2026},
  url    = {https://github.com/fahrim/stationary-strings-xii}
  doi    = {10.5281/zenodo.23517474},
}
```

See also `CITATION.cff`.

## Related work

- `stationary-strings-i` … `stationary-strings-x` — Theorems I–X (the parent series).
- `stationary-strings-xiii` — Yang–Mills mass gap, glueball spectrum, quark confinement.
- `stationary-strings-xiv` — Benchtop vortex PIV, Vela glitches, Na-22 positronium.

## License

CC BY 4.0 — see `LICENSE`. Content is not peer-reviewed.
