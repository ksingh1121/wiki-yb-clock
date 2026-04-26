# Wiki Log

Append-only record of all wiki operations.

---

## 2026-04-26 — Initial Build: All 14 Sources

**Session**: Initial wiki construction from 14 readable source PDFs (one source, A D Ludlow et al. PRA 2011, was unreadable due to image-only PDF format).

### Sources Ingested

1. Takamoto et al. Nature 2005 — First Sr optical lattice clock
2. C W Hoyt et al. PRL 2005 — First Yb MOT clock transition spectroscopy
3. Z W Barber et al. PRL 2006 (file: PRL 2005) — First ¹⁷⁴Yb lattice clock with MIS
4. Z W Barber et al. PRL 2008 — Lattice light shifts and hyperpolarizability in Yb
5. N D Lemke et al. PRL 2009 — First ¹⁷¹Yb lattice clock evaluation
6. T Kohno et al. APE 2009 — NMIJ ¹⁷¹Yb clock, independent frequency measurement
7. J A Sherman et al. PRL 2012 — DC Stark measurement of Δα(0)
8. K Beloy et al. PRL 2014 — In-vacuum BBR shield achieving 10⁻¹⁸ BBR uncertainty
9. R C Brown et al. PRL 2017 — Hyperpolarizability and operational magic wavelength
10. Q Gao et al. Scientific Reports 2018 — ECNU synchronous comparison, density shift
11. M S Safronova et al. PRL 2018 — Dual clock transition proposal (3P₀→J=2 at 1695 nm)
12. V Dzuba et al. PRA 2018 — CIPT calculations for Yb clock transition candidates
13. A Ludlow et al. RMP 2015 — Comprehensive optical clocks review
14. T Bothwell et al. PRL 2025 — Dual-ensemble evaluation, all lattice shifts <10⁻¹⁸

**Unreadable**: A D Ludlow et al. PRA 2011 (image-only PDF, no text layer — flagged for user to re-acquire)

### Pages Created

**Concept pages (11)**:
- `yb-atomic-structure.md` — Yb energy levels, isotopes, transitions
- `clock-transition-yb.md` — 1S₀→3P₀ frequency, linewidth, spectroscopy
- `magic-wavelength.md` — Measured values, convention warnings
- `optical-lattice-clock.md` — Operating principle, stability, Yb vs. Sr
- `lattice-light-shift.md` — Full shift hierarchy, evaluated uncertainties
- `hyperpolarizability.md` — β̃ vs. β* conventions, two-photon resonances
- `multipolarizability.md` — α̃_M1E2, diamagnetic correction
- `blackbody-radiation-shift.md` — BBR formula, Δα(0), dynamic correction
- `magnetic-field-induced-spectroscopy.md` — MIS for ¹⁷⁴Yb
- `zeeman-shift.md` — First-order, quadratic Zeeman, vector light shift
- `density-shift.md` — p-wave collisions, synchronous comparison method
- `clock-stability.md` — Allan deviation, Dick effect, synchronous comparison
- `systematic-uncertainty-budget.md` — Budget comparison 2009–2025
- `bbr-shield.md` — Copper shield design, CNT coating, RTD thermometry
- `fundamental-constants-variation.md` — α-variation, K_α coefficients
- `dual-clock-transitions-yb.md` — 3P₀→J=2 dual clock proposal

**Paper summary pages (14)**:
- `takamoto-nature-2005.md`
- `hoyt-prl-2005.md`
- `barber-prl-2006.md`
- `barber-prl-2008.md`
- `lemke-prl-2009.md`
- `kohno-ape-2009.md`
- `sherman-prl-2012.md`
- `beloy-prl-2014.md`
- `brown-prl-2017.md`
- `gao-sr-2018.md`
- `safronova-prl-2018.md`
- `dzuba-pra-2018.md`
- `ludlow-rmp-2015.md`
- `bothwell-prl-2025.md`

**Infrastructure**:
- `index.md` — Full table of contents with key numbers at a glance
- `log.md` — This file

**Total pages created**: 32 (16 concept + 14 paper summaries + index + log)

### Key Decisions and Notes

- File `Z W Barber et al. PRL 2005.pdf` is actually PRL 96 (2006); wiki page named `barber-prl-2006.md` to match publication date
- Convention differences between Brown 2017 (β*, ν_zero, α*) and Bothwell 2025 (β̃, ν_E1, α̃) are explicitly documented in `magic-wavelength.md`, `hyperpolarizability.md`, and `lattice-light-shift.md`
- The factor ~2 between ∂α*/∂ν (Brown 2017) and ∂α̃_E1/∂ν (Bothwell 2025) is explained by thermal averaging in the lattice
- The M1E2 diamagnetic correction (~2% from negative-energy states) that resolved the theory-experiment discrepancy is documented in `multipolarizability.md`
- Page `systematic-uncertainty-budget.md` tracks the evolution of the BBR and lattice light shift uncertainties from 10⁻¹⁵ to 10⁻¹⁸ level across 2009–2025
