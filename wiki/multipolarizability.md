# Multipolarizability (M1E2)

**Summary**: The differential light shift on the clock transition from magnetic-dipole (M1) and electric-quadrupole (E2) interactions with the lattice field, scaling as U^{1/2} and resolved by Bothwell 2025 through the diamagnetic correction.

**Sources**: R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf

**Last updated**: 2026-04-26

---

## Physical Origin

Beyond the dominant electric-dipole (E1) polarizability, higher-order multipole interactions with the lattice field produce additional shifts. The magnetic-dipole (M1) and electric-quadrupole (E2) interactions give a combined differential contribution called the **multipolarizability shift**. Physically, the lattice field drives both electric-quadrupole and magnetic-dipole transitions, and the AC Stark shift from these channels contributes at a level below the E1 shift.

The fractional frequency shift scales as:

$$\frac{\delta\nu_{M1E2}}{\nu_\text{clock}} = -\tilde{\alpha}_{M1E2} \cdot U^{1/2}$$

The $U^{1/2}$ scaling (rather than $U^1$) arises because the lattice field amplitude (not intensity) enters the relevant matrix elements. More precisely, it scales as the local field gradient, which is proportional to $U^{1/2}$ for a standing-wave lattice. (source: T Bothwell et al. PRL 2025.pdf)

## Measured and Theoretical Values

| Quantity | Value | Source |
|----------|-------|--------|
| $\tilde{\alpha}_{M1E2}$ (measured) | $-1.41(9)\times10^{-18}$ | Bothwell 2025 |
| $\tilde{\alpha}_{M1E2}$ (theory, with diamagnetic correction) | $-1.9(5)\times10^{-18}$ | Bothwell 2025 |

Agreement is at the 1.1σ level, which is satisfactory given the 26% theoretical uncertainty. (source: T Bothwell et al. PRL 2025.pdf)

## The Diamagnetic Correction

Prior to Bothwell 2025, there was a longstanding discrepancy between theory and experiment for $\tilde{\alpha}_{M1E2}$ in both Yb and Sr. The root cause was an overlooked contribution: the **diamagnetic term** in the M1 polarizability.

In relativistic quantum mechanics, the M1 polarizability receives a contribution from **negative-energy (positronic) states** — the diamagnetic correction. This was neglected in earlier theoretical treatments. Including it provides a ~2% correction to the total M1E2 coefficient and shifts the theoretical value closer to the experimental measurement. The Bothwell 2025 theory-experiment comparison at the 1.1σ level represents the first satisfactory reconciliation of this long-standing discrepancy, in both Yb and Sr. (source: T Bothwell et al. PRL 2025.pdf)

## Effect on the Apparent Magic Frequency

The M1E2 shift adds a $U^{1/2}$ contribution on top of the linear (E1) shift. When fitting clock frequency data as a linear function of $U$ to extract the "magic frequency," the M1E2 term causes the extrapolated zero to be shifted from $\nu_{E1}$ by:

$$\nu_\text{zero} = \nu_{E1} - \frac{\tilde{\alpha}_{M1E2}}{\partial\tilde{\alpha}_{E1}/\partial\nu}$$

Since $\tilde{\alpha}_{M1E2} < 0$ and $\partial\tilde{\alpha}_{E1}/\partial\nu > 0$, the observed zero $\nu_\text{zero}$ lies **below** $\nu_{E1}$:

$$\nu_\text{zero} \approx \nu_{E1} - 400 \text{ kHz}$$

(source: R C Brown et al. PRL 2017.pdf)

This is why $\nu_\text{zero}$ (as defined by Brown 2017) and $\nu_{E1}$ (as defined by Bothwell 2025) differ by ~400 kHz — they are measuring slightly different quantities. See [[magic-wavelength]] for the full convention comparison.

## Measurement Technique (Bothwell 2025)

Bothwell 2025 used a **running-wave technique** to isolate $\tilde{\alpha}_{M1E2}$. An auxiliary running-wave laser field is applied to one ensemble (dual-ensemble apparatus). The running-wave magic frequency $\nu^0_r(u_0)$ depends on trap depth in a way that involves a different combination of $\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$ than the standing-wave magic frequency. By measuring both the standing-wave and running-wave zeros as a function of trap depth, the two unknowns $\nu_{E1}$ and $\tilde{\alpha}_{M1E2}$ can be separated with minimal correlation. (source: T Bothwell et al. PRL 2025.pdf)

## Related pages

- [[lattice-light-shift]]
- [[hyperpolarizability]]
- [[magic-wavelength]]
- [[optical-lattice-clock]]
- [[systematic-uncertainty-budget]]
