# Grand Proof I — Yayın Paketi (Büyük Kanıt Serisi I)

> **English:** [README.md](./README.md)

**Grand Proof I: Karanlık-Maddesiz Galaktik Dinamik, Meral Kozmik İvme Ölçeği, SPARC Dönüş Eğrileri ve EHT Karadelik Halka Kanıtı**

Yazar: Fahri Meral · Tarih: 19 Ekim 2026 · Sürüm: v1 (Grand Proof I)

> **Durum:** Yayımlanmamış ön-baskı (v1). Hakem denetiminden geçmemiştir.

## İçerik

| Dosya | Açıklama |
|---|---|
| `paper/grand_proof_I_galaktik_dinamik.tex` | Ana makale, Türkçe (Tablo 1–3, Şekil 1 2×2) |
| `paper/grand_proof_I_galactic_dynamics_EN.tex` | İngilizce sürüm |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.pdf` | T29–T31 şekli (TR, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring.png` | T29–T31 şekil önizlemesi (TR) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.pdf` | T29–T31 şekli (EN, 2×2) |
| `figs/fig13_dark_matter_free_sparc_btfr_and_eht_ring_en.png` | T29–T31 şekil önizlemesi (EN) |
| `CITATION.cff` | Atıf kaydı |
| `LICENSE` | CC BY 4.0 |

## Sonuçlar (sıfır serbest parametre)

- Meral ölçeği `a_Meral = 1,146589e-10 m/s²`, SPARC `a_0 = 1,20e-10` ile %4,45 fark (0,22σ_sys).
- BTFR eğimi tam 4,000000000000000 (R² = 1,0); 5 SPARC arketipinde ortalama %4,54
  (UGC 2885 açıkça raporlanan %12,9 dış-değerdir).
- EHT halkaları: Sgr A* 50,31 μas (0,65σ), M87* 38,31 μas (1,23σ).

## Sayısal yeniden-üretim

T29–T31 testleri **Makale V deposundaki** çözücüyle üretilir
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py   # T1–T31 (31/31 PASS)
python duran_sicimler_sim/mini_check_gp1.py  # bağımsız çapraz kontrol (15/15 PASS)
```

Bağımsız çapraz kontrol çözücüyü import etmez.
Şekil 1, `generate_figures.py` içindeki `fig13` işleviyle üretilir.
