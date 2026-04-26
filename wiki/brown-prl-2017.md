# Brown et al. PRL 2017

**Summary**: Systematic evaluation of the nonlinear lattice light shift in ¹⁷¹Yb using the operational magic wavelength concept, achieving 1.2×10⁻¹⁸ lattice light shift uncertainty and measuring the finite-temperature hyperpolarizability β* = −5.5(2)×10⁻²².

**Sources**: R C Brown et al. PRL 2017.pdf

**Last updated**: 2026-04-26

---

## Reference

R. C. Brown, N. B. Phillips, K. Beloy, W. F. McGrew, M. Schioppo, R. J. Fasano, G. Milani, X. Zhang, N. Hinkley, H. Leopardi, T. H. Yoon, D. Nicolodi, T. M. Fortier, and A. D. Ludlow, "Hyperpolarizability and Operational Magic Wavelength in an Optical Lattice Clock," *Phys. Rev. Lett.* **119**, 023201 (2017).

## Context

After Beloy 2014 reduced the BBR uncertainty to $10^{-18}$, the lattice light shift became the dominant systematic. The linear (E1) term could be controlled by operating near the magic wavelength, but the nonlinear terms — particularly the hyperpolarizability ($\propto U^2$) and multipolarizability ($\propto U^{1/2}$) — remained at the $1–5 \times10^{-18}$ level. This paper introduced the **operational magic wavelength** as a practical method to suppress the nonlinear shift.

## Key Physics: Operational Magic Wavelength

The total fractional frequency shift due to the lattice can be written (for a thermal sample with $T \propto U$):

$$\frac{\delta\nu}{\nu} \approx -\alpha^*(U) \cdot U - \beta^* U^2$$

where $\alpha^*(U) = \alpha^*_0 + \frac{\partial\alpha^*}{\partial\nu} \cdot \delta_L$ depends on the detuning $\delta_L = \nu_L - \nu_\text{zero}$.

The total shift has zero derivative with respect to $U$ when:

$$\frac{\partial}{\partial U}\left[\frac{\delta\nu}{\nu}\right] = 0 \implies \delta_L = \frac{-2\beta^* U}{\partial\alpha^*/\partial\nu}$$

This defines the **operational magic wavelength** as a function of trap depth $U$:

$$\nu_\text{op.magic}(U) = \nu_\text{zero} + \frac{-2\beta^* U}{\partial\alpha^*/\partial\nu}$$

At this frequency, first-order sensitivity to trap depth fluctuations vanishes — a 10% change in $U$ changes the fractional shift by only $\sim 10^{-19}$.

## Key Results

| Quantity | Value | Units |
|----------|-------|-------|
| $\nu_\text{zero}$ (zero of $\alpha^*(U)$) | 394,798,267(3) | MHz |
| $\partial\alpha^*/\partial\nu$ | $2.46(10)\times10^{-20}$ | /MHz |
| $\beta^*$ (finite-temperature hyperpolarizability) | $-5.5(2)\times10^{-22}$ | — |
| Operational magic wavelength offset at $50 E_r$ | $+2.2(1)$ MHz above $\nu_\text{zero}$ | — |
| Lattice light shift uncertainty | $1.2\times10^{-18}$ | fractional |

## $\nu_\text{zero}$ vs $\nu_{E1}$

Brown 2017 defines $\nu_\text{zero}$ as the frequency where the effective linear coefficient $\alpha^*(U)$ vanishes. Because $\alpha^*$ includes both E1 and M1E2 contributions at finite temperature, $\nu_\text{zero}$ is shifted from the pure E1 zero ($\nu_{E1}$) by:

$$\nu_\text{zero} = \nu_{E1} - \frac{\tilde{\alpha}_{M1E2}}{\partial\tilde{\alpha}_{E1}/\partial\nu} \approx \nu_{E1} - 400 \text{ kHz}$$

This convention difference explains why the Bothwell 2025 $\nu_{E1} = 394,798,266.9(2.6)$ MHz and Brown 2017's $\nu_\text{zero} = 394,798,267(3)$ MHz are nearly equal: the 400 kHz difference is within the uncertainty. See [[magic-wavelength]] for the full convention comparison.

## Convention: $\beta^*$ vs $\tilde{\beta}$

Brown 2017 measures $\beta^* = -5.5(2)\times10^{-22}$, the **effective finite-temperature** hyperpolarizability. This differs from the intrinsic harmonic-state quantity $\tilde{\beta} = -1.7(4)\times10^{-21}$ (Bothwell 2025) by a factor $|\beta^*/\tilde{\beta}| \approx 0.32$, due to spatial delocalization of thermally excited atoms in the lattice potential.

Always check which convention is used when comparing hyperpolarizability values. See [[hyperpolarizability]].

## Temperature Model

A key simplification in this paper: the sample temperature is observed to scale proportionally with trap depth ($T \propto U$, with the same proportionality constant throughout the lattice loading and cooling sequence). Under this condition, the motional-state-dependent corrections collapse into effective coefficients $\alpha^*$ and $\beta^*$ that are approximately independent of $U$, greatly simplifying the analysis.

## Significance

This paper defined the operational framework for controlling the nonlinear lattice light shift at $10^{-18}$ that has been used by all subsequent NIST Yb evaluations (including Bothwell 2025). The concept of operating at the operational magic wavelength rather than the E1 magic wavelength is now standard practice.

## Related pages

- [[lattice-light-shift]]
- [[hyperpolarizability]]
- [[multipolarizability]]
- [[magic-wavelength]]
- [[systematic-uncertainty-budget]]
- [[bothwell-prl-2025]]
