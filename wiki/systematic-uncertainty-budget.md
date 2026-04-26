# Systematic Uncertainty Budget

**Summary**: A comparison of the systematic uncertainty budgets for ¹⁷¹Yb optical lattice clocks across major evaluations from 2009 to 2025, tracking the reduction of each shift category.

**Sources**: N D Lemke et al. PRL 2009.pdf, J A Sherman et al. PRL 2012.pdf, K Beloy et al. PRL 2014.pdf, R C Brown et al. PRL 2017.pdf, Q Gao et al. SR 2018.pdf, T Bothwell et al. PRL 2025.pdf

**Last updated**: 2026-04-26

---

## Overview

A systematic uncertainty budget enumerates every known physical effect that shifts or broadens the clock frequency, along with the uncertainty in each correction. The **total systematic uncertainty** is the quadrature sum of all individual contributions.

For an optical lattice clock, the dominant systematic categories are:

1. [[blackbody-radiation-shift]] — largest in early clocks
2. [[lattice-light-shift]] — dominant nonlinear term at mid-era
3. [[zeeman-shift]] — well-controlled by $m_F$ averaging
4. [[density-shift]] — requires careful atom-number control
5. AC Stark from probe laser — small for short Rabi pulses
6. Servo offset and line pulling — apparatus-dependent

## Lemke 2009 Budget (NIST, First ¹⁷¹Yb Lattice Clock)

Total systematic uncertainty: **$3.4\times10^{-16}$**

| Effect | Uncertainty |
|--------|-------------|
| BBR shift | $9.7\times10^{-16}$ (fractional) |
| Lattice light shift (first-order) | $2.0\times10^{-16}$ |
| Lattice light shift (nonlinear) | $0.7\times10^{-16}$ |
| Density/collisional shift | $1.0\times10^{-16}$ |
| Second-order Zeeman | $<10^{-17}$ |
| DC Stark (stray fields) | — |
| Probe AC Stark | — |
| **Total (quadrature)** | **$3.4\times10^{-16}$** |

BBR dominated the budget because the differential static polarizability $\Delta\alpha(0)$ was poorly known (10% theoretical uncertainty). (source: N D Lemke et al. PRL 2009.pdf)

## Sherman 2012 Impact

Sherman 2012 measured $\Delta\alpha(0) = 36.2612(7)$ kHz(kV/cm)⁻² with ppm precision. This reduced the BBR fractional uncertainty from $9.7\times10^{-16}$ to $3\times10^{-17}$ — a 30× improvement — without changing the apparatus. After this, lattice light shifts became the dominant uncertainty source. (source: J A Sherman et al. PRL 2012.pdf)

## Beloy 2014 Budget (NIST, With BBR Shield)

The in-vacuum copper thermal shield (see [[bbr-shield]]) reduced the BBR uncertainty to $1\times10^{-18}$ by:
1. Operating the atoms in a colder, more uniform thermal environment inside the shield
2. Precisely characterizing the shield temperature with resistance thermometers
3. Computing the dynamic correction with ab initio theory ($\eta_1$, $\eta_2$ from Beloy 2014)

After Beloy 2014, the lattice light shift became the leading systematic. (source: K Beloy et al. PRL 2014.pdf)

## Brown 2017 Budget (NIST, Lattice Light Shift Evaluation)

Total lattice light shift uncertainty: **$1.2\times10^{-18}$**

Brown 2017 focused on the nonlinear lattice light shift. Using the operational magic wavelength at $U=50 E_r$ reduced the hyperpolarizability uncertainty to $1.2\times10^{-18}$. The E1 linear term was controlled by precision measurement of $\nu_\text{zero}$ and $\partial\alpha^*/\partial\nu$. At this level, the lattice light shift was the only remaining contribution above $10^{-18}$. (source: R C Brown et al. PRL 2017.pdf)

## Gao 2018 Budget (ECNU)

Total systematic uncertainty: **$1.7\times10^{-16}**

| Effect | Uncertainty |
|--------|-------------|
| BBR shift | — |
| Lattice light shift | — |
| Density/collision shift | $4.9\times10^{-17}$ |
| Zeeman shift | — |
| **Total** | **$1.7\times10^{-16}$** |

ECNU achieved $1.7\times10^{-16}$ total uncertainty with the synchronous comparison method, enabling a precise density shift measurement of $-0.570(25)$ Hz. (source: Q Gao et al. SR 2018.pdf)

## Bothwell 2025 Budget (NIST, Dual-Ensemble)

Total systematic uncertainty: **$<10^{-18}$** for lattice light shift contributions

| Effect | Uncertainty |
|--------|-------------|
| E1 lattice shift | $<10^{-18}$ |
| M1E2 multipolarizability | $<10^{-18}$ |
| Hyperpolarizability $\tilde{\beta}$ | $<10^{-18}$ |
| BBR shift | Controlled by existing shield |
| **Total lattice light shift** | **$<10^{-18}$** |

Bothwell 2025 used the dual-ensemble apparatus with running-wave probing to separate $\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$ with minimal correlation. The diamagnetic correction to the M1 polarizability resolved the theory-experiment discrepancy. (source: T Bothwell et al. PRL 2025.pdf)

## Progress Summary

| Year | Lab | Total uncertainty | Limiting effect |
|------|-----|------------------|----------------|
| 2009 | NIST | $3.4\times10^{-16}$ | BBR |
| 2012 | NIST | $\sim3\times10^{-17}$ | Lattice light shift |
| 2014 | NIST | $\sim10^{-18}$ | Lattice light shift |
| 2017 | NIST | $1.2\times10^{-18}$ | Lattice light shift (nonlinear) |
| 2018 | ECNU | $1.7\times10^{-16}$ | BBR + density |
| 2025 | NIST | $<10^{-18}$ | All contributions below $10^{-18}$ |

## Related pages

- [[blackbody-radiation-shift]]
- [[lattice-light-shift]]
- [[zeeman-shift]]
- [[density-shift]]
- [[bbr-shield]]
- [[optical-lattice-clock]]
- [[hyperpolarizability]]
- [[multipolarizability]]
