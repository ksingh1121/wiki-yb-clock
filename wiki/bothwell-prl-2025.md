# Bothwell et al. PRL 2025

**Summary**: The most advanced ¹⁷¹Yb lattice clock evaluation to date, using a dual-ensemble apparatus and running-wave technique to separate E1 and M1E2 contributions, achieving <10⁻¹⁸ uncertainty for all lattice light shift contributions and resolving the long-standing M1E2 theory-experiment discrepancy via the diamagnetic correction.

**Sources**: T Bothwell et al. PRL 2025.pdf

**Last updated**: 2026-04-26

---

## Reference

T. Bothwell, C. J. Kennedy, A. Aeppli, D. Kedar, J. M. Robinson, E. Oelker, A. Staron, and J. Ye, *Phys. Rev. Lett.* (2025). [Title and exact journal reference not fully extracted from source.]

*Note: This may be a JILA (Boulder) group paper, not NIST. Verify affiliation from source PDF.*

## Context

As of 2017 (Brown et al.), the NIST Yb lattice light shift uncertainty stood at $1.2\times10^{-18}$. Two remaining challenges were:
1. Separating the E1 magic frequency $\nu_{E1}$ from the M1E2 contribution with low correlation
2. Resolving the theory-experiment discrepancy in $\tilde{\alpha}_{M1E2}$ (previous experiments and theory disagreed by ~2σ in both Yb and Sr)

Bothwell 2025 addressed both issues simultaneously with a new dual-ensemble running-wave technique.

## Key Results

### Magic Frequency and Light Shift Coefficients

| Quantity | Value | Notes |
|----------|-------|-------|
| $\nu_{E1}$ (E1 magic frequency) | $394,798,266.9(2.6)$ MHz | Pure E1 zero, $T=0$ limit |
| $\partial\tilde{\alpha}_{E1}/\partial\nu$ | $4.2(1)\times10^{-20}$ /MHz | Intrinsic (T=0) slope |
| $\tilde{\alpha}_{M1E2}$ (measured) | $-1.41(9)\times10^{-18}$ | — |
| $\tilde{\alpha}_{M1E2}$ (theory, with diamagnetic) | $-1.9(5)\times10^{-18}$ | 1.1σ agreement |
| $\tilde{\beta}$ (hyperpolarizability) | $-1.7(4)\times10^{-21}$ | Harmonic-state basis |
| Total lattice light shift uncertainty | $<10^{-18}$ | All contributions |

### Convention Notes vs. Brown 2017

| Quantity | Brown 2017 definition | Bothwell 2025 definition |
|----------|----------------------|--------------------------|
| Magic frequency zero | $\nu_\text{zero}$ (zero of $\alpha^*$ at finite $T$) | $\nu_{E1}$ (zero of $\tilde{\alpha}_{E1}$ at $T=0$) |
| Value | $394,798,267(3)$ MHz | $394,798,266.9(2.6)$ MHz |
| Difference | $\approx 0.1$ MHz (within error) | — |
| Linear slope | $\partial\alpha^*/\partial\nu = 2.46(10)\times10^{-20}$ /MHz | $\partial\tilde{\alpha}_{E1}/\partial\nu = 4.2(1)\times10^{-20}$ /MHz |
| Slope ratio | — | $\approx 2\times$ larger (as expected: $\alpha^* \approx \frac{1}{2}\tilde{\alpha}$ at thermal equilibrium) |
| Hyperpolarizability | $\beta^* = -5.5(2)\times10^{-22}$ (finite-$T$) | $\tilde{\beta} = -1.7(4)\times10^{-21}$ (harmonic) |

The factor ~2 difference in slopes is expected: Brown 2017's $\alpha^*$ averages over thermally excited motional states, which occupy sites of lower average intensity, giving $\partial\alpha^*/\partial\nu \approx \frac{1}{2}\partial\tilde{\alpha}_{E1}/\partial\nu$.

## Dual-Ensemble Running-Wave Technique

### The Problem

$\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$ cannot be separated from standing-wave measurements alone because the standing-wave magic frequency $\nu^0_\text{sw}$ depends on a particular combination of both:

$$\nu^0_\text{sw} = \nu_{E1} + \frac{\tilde{\alpha}_{M1E2}}{\partial\tilde{\alpha}_{E1}/\partial\nu}$$

### The Running-Wave Solution

An auxiliary running-wave field applied to one ensemble changes the effective magic condition because the running wave has different spatial profile (traveling vs. standing). The running-wave magic frequency $\nu^0_r(u_0)$ depends on trap depth $u_0$ and involves a **different** linear combination of $\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$:

$$\nu^0_r(u_0) = \nu_{E1} - \frac{\tilde{\alpha}_{M1E2}}{\partial\tilde{\alpha}_{E1}/\partial\nu} + f(u_0)$$

By measuring both $\nu^0_\text{sw}$ and $\nu^0_r(u_0)$ at multiple $u_0$ values, the two unknowns $\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$ are determined with minimal correlation. This is the key experimental innovation of Bothwell 2025.

### Dual Ensemble

Two atomic clouds are prepared in the same vacuum chamber and interrogated simultaneously by the same clock laser. One ensemble receives the running wave; the other does not. The differential frequency measurement between the two ensembles is Dick-effect-free and allows precise determination of the running-wave-induced shift.

## Resolution of the M1E2 Discrepancy

Prior to Bothwell 2025, measured $\tilde{\alpha}_{M1E2}$ in both Yb and Sr differed from theoretical predictions at the ~2σ level. The root cause was a **diamagnetic contribution** to the M1 polarizability from negative-energy (positronic) states in the relativistic treatment — a ~2% correction that had been omitted from earlier theoretical calculations.

Including the diamagnetic correction in theory shifts the predicted $\tilde{\alpha}_{M1E2}$ closer to the experimental value, giving 1.1σ agreement. This resolved the discrepancy in both Yb (this paper) and Sr (where the same correction was applied).

## Lattice Light Shift Uncertainty <10⁻¹⁸

The total lattice light shift uncertainty achieved:
- E1 contribution: $<10^{-18}$ (controlled by precision measurement of $\nu_{E1}$)
- M1E2 contribution: $<10^{-18}$ (measured with running-wave technique)
- Hyperpolarizability: $<10^{-18}$ (measured from $U^2$ scaling at operational magic wavelength)

This represents the first time all three contributions to the lattice light shift have been simultaneously controlled below $10^{-18}$ in a single evaluation.

## Related pages

- [[lattice-light-shift]]
- [[hyperpolarizability]]
- [[multipolarizability]]
- [[magic-wavelength]]
- [[systematic-uncertainty-budget]]
- [[brown-prl-2017]]
- [[clock-stability]]
