# Stationary Strings XII — Yayın Paketi

> **English:** [README.md](./README.md)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)

**Stationary Strings XII: Karanlık-Maddesiz Galaktik Dinamik, Meral Kozmik İvme Ölçeği, SPARC Dönüş Eğrileri ve EHT Karadelik Halka Kanıtı**

Yazar: Fahri Meral · Tarih: 19 Ekim 2026 · Sürüm: v1 (Stationary Strings XII)

> **Durum:** Yayımlanmamış ön-baskı (v1). Hakem denetiminden geçmemiştir. *Zenodo DOI'si yüklemeyi bekliyor.*

## İçerik

| Dosya | Açıklama |
|---|---|
| `paper/stationary_strings_XII_galaktik_dinamik.tex` | Ana makale, Türkçe (Tablo 1–3, Şekil 1 2×2) |
| `paper/stationary_strings_XII_galactic_dynamics_EN.tex` | İngilizce sürüm |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.pdf` | T29–T31 şekli (TR, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.png` | T29–T31 şekil önizlemesi (TR) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.pdf` | T29–T31 şekli (EN, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.png` | T29–T31 şekil önizlemesi (EN) |
| `CITATION.cff` | Atıf kaydı |
| `LICENSE` | CC BY 4.0 |

## Ana bulgular

- **T29 (Teorem XII.1):** sıfır-parametreli Meral kozmik ivme ölçeği
  `a_Meral = µ_s^Meral (1-η_T0) c H_0 = 1,1465889797e-10 m/s²`
  (Planck 2018 `H_0 = 67,4`), yani model **boyutsuz oran**
  `κ_Meral = a_0/(cH_0) = 0,175097` öngörür. SPARC `a_0 =
  (1,20 ± 0,02 ± 0,24)e-10` ile karşılaştırma Planck'ta %4,45
  (0,22σ_sys), yerel `H_0 = 70,5`'te %0,06'dır — test benimsenen `H_0`'ı
  taşır ve **mutlak, `H_0`'dan bağımsız bir ölçek doğrulaması değil,
  tutarlılık** gösterir.
- **T29/T30 (Teorem XII.2):** sicim-çember RAR'ı
  `g_obs = g_bar[1+(x+x²)^(-1/2)]`, `x = g_bar/a_Meral`, dış-halo yasası
  `v_flat⁴ = G M_b a_Meral` ve log-log eğimi **4,000000000000000**
  (`R² = 1,0`); beş SPARC arketipinde ortalama %4,54 sapma (dördü %4,1'in
  altında; dev sarmal UGC 2885 açıkça raporlanan %12,9 dış-değerdir).
- **T31 (Teorem XII.3):** EHT halka doyumu
  `d_ring = 6 θ_g C_univ √(1+µ_s/4) = 10,002404 θ_g`; Sgr A* için
  50,31 μas (0,65σ), M87* için 38,31 μas (1,23σ) — ölçümler sırasıyla
  51,8 ± 2,3 ve 42,0 ± 3,0 μas.

## Sayısal yeniden-üretim

T29–T31 testleri **Makale V deposundaki** çözücüyle üretilir
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py     # T1–T31 (31/31 PASS)
python duran_sicimler_sim/mini_check_gp1.py    # bağımsız çapraz kontrol (15/15 PASS)
```

Bağımsız çapraz kontrol çözücüyü import etmez. Şekil 1,
`duran_sicimler_sim/generate_figures.py` içindeki `fig13` işleviyle üretilir.

## Atıf

```bibtex
@misc{meral2026grandproofi,
  author = {Fahri Meral},
  title  = {Stationary Strings XII: Karanlık-Maddesiz Galaktik Dinamik, Meral Kozmik İvme Ölçeği, SPARC Dönüş Eğrileri ve EHT Karadelik Halka Kanıtı},
  year   = {2026},
  url    = {https://github.com/fahrim/stationary-strings-xii}
}
```

Ayrıca bkz. `CITATION.cff`.

## İlgili çalışmalar

- `stationary-strings-i` … `stationary-strings-x` — Teoremler I–X (ana seri).
- `stationary-strings-xiii` — Yang–Mills kütle aralığı, glueball spektrumu, kuark kuşatması.
- `stationary-strings-xiv` — Masaüstü girdap PIV, Vela glitch, Na-22 pozitronyum.

## Lisans

CC BY 4.0 — bkz. `LICENSE`. İçerik hakem denetiminden geçmemiştir.
