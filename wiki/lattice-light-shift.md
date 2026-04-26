# Lattice Light Shift

**Summary**: The AC Stark shift of the clock transition due to the optical lattice field, organized as a hierarchy of terms scaling as different powers of trap depth U.

**Sources**: Z W Barber et al. PRL 2008.pdf, N D Lemke et al. PRL 2009.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## The Shift Hierarchy

The fractional frequency shift of the clock transition due to the optical lattice has a hierarchy of terms that scale with different powers of the trap depth U (in units of recoil energy $E_r$):

$$\frac{\delta\nu_\text{clock}}{\nu_\text{clock}} = -\underbrace{\tilde{\alpha}_{E1} \cdot \delta_L \cdot U^1}_{\text{E1 (linear)}} - \underbrace{\tilde{\alpha}_{M1E2} \cdot U^{1/2}}_{\text{multipolarizability}} - \underbrace{\tilde{\beta} \cdot U^2}_{\text{hyperpolarizability}}$$

where $\delta_L = \nu_L - \nu_{E1}$ is the detuning of the lattice from the E1 magic frequency, and the "tilde" quantities are dimensionless differential coefficients.

More precisely, following Brown 2017 and Bothwell 2025, the shift for an atom in longitudinal band $n_z$ and transverse state $n_\rho$ includes motional-state-dependent corrections. For a thermal sample with temperature proportional to U (which is observed experimentally), the model simplifies to:

$$\frac{\delta\nu_\text{clock}}{\nu_\text{clock}} \approx -\alpha^* U - \beta^* U^2$$

where $\alpha^*$ and $\beta^*$ are **effective** finite-temperature polarizabilities that are approximately independent of U. (source: R C Brown et al. PRL 2017.pdf)

## E1 Differential Polarizability (Linear Term)

The dominant term. Controlled by operating at the [[magic-wavelength]] where $\Delta\alpha_{E1}(\nu_\text{magic}) = 0$. At finite detuning $\delta_L$ from $\nu_{E1}$:

$$\delta\nu_{E1} \approx -\frac{\partial\tilde{\alpha}_{E1}}{\partial\nu} \cdot \delta_L \cdot U \cdot \nu_\text{clock}$$

Measured slope (Bothwell 2025): $\partial\tilde{\alpha}_{E1}/\partial\nu = 4.2(1)\times10^{-20}$ (1/MHz)
Measured slope (Brown 2017): $\partial\alpha^*/\partial\nu = 2.46(10)\times10^{-20}$ (1/MHz) [at finite temperature]

**Convention note**: The "slope" depends on whether one quotes $\partial\tilde{\alpha}_{E1}/\partial\nu$ (intrinsic atomic property, T=0) or $\partial\alpha^*/\partial\nu$ (finite-temperature quantity). At Brown 2017's experimental temperature (T proportional to U), $\partial\alpha^*/\partial\nu \approx (1/2)\partial\tilde{\alpha}_{E1}/\partial\nu$ due to spatial delocalization of thermally excited atoms. (source: R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf)

## Multipolarizability (M1E2, Scales as U^{1/2})

Beyond the electric-dipole (E1) polarizability, magnetic-dipole (M1) and electric-quadrupole (E2) interactions give a differential shift that scales as $U^{1/2}$. The relevant coefficient is $\tilde{\alpha}_{M1E2}$.

**Measured value** (Bothwell 2025): $\tilde{\alpha}_{M1E2} = -1.41(9)\times10^{-18}$
**Theoretical value** (Bothwell 2025): $\tilde{\alpha}_{M1E2} = -1.9(5)\times10^{-18}$

Agreement within 1.1σ, after including the previously neglected **diamagnetic contribution** to the M1 polarizability (a ~2% correction arising from negative-energy states in the relativistic treatment). This resolved a longstanding discrepancy between theory and experiment in both Yb and Sr. (source: T Bothwell et al. PRL 2025.pdf)

The M1E2 term shifts the observed linear-coefficient zero from the E1 magic frequency by:
$$\nu_\text{zero} = \nu_{E1} - \frac{\tilde{\alpha}_{M1E2}}{\partial\tilde{\alpha}_{E1}/\partial\nu} \approx \nu_{E1} - 400 \text{ kHz}$$
(source: R C Brown et al. PRL 2017.pdf)

## Hyperpolarizability (Scales as U^2)

The fourth-order electric-field effect. For a 1D standing wave lattice:

$$\delta\nu_{\text{HP}} = -\tilde{\beta} U^2 \nu_\text{clock}$$

where $\tilde{\beta}$ is the differential hyperpolarizability. For ¹⁷¹Yb:

| Value | Notation | Source |
|-------|----------|--------|
| $-5.5(2)\times10^{-22}$ | $\beta^*$ (finite temperature) | Brown 2017 |
| $-1.7(4)\times10^{-21}$ | $\tilde{\beta}$ (harmonic, Bothwell 2025) | Bothwell 2025 |
| 170(33) mHz at 500$E_r$ | absolute shift | Barber 2008 |

(sources: R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf, Z W Barber et al. PRL 2008.pdf)

**Convention warning**: $\beta^*$ and $\tilde{\beta}$ are NOT the same quantity. $\beta^* < |\tilde{\beta}|$ because thermally excited atoms are spatially delocalized and experience lower average lattice intensity. The relation approximately gives $\beta^* \approx \tilde{\beta}/(2\sqrt{U})^{3/2} \times ...$. Always check whether the quoted hyperpolarizability is the intrinsic atomic property or an effective temperature-dependent quantity. (source: R C Brown et al. PRL 2017.pdf)

The hyperpolarizability arises from nearby two-photon resonances from the 3P₀ clock state to higher 6s8p³P and 6s5f³F states:
- 3P₀ → 6s8p³P₀ at 759.7082 nm (nearest, ~184 GHz from magic λ)
- 3P₀ → 6s8p³P₂ at 754.23 nm
- 3P₀ → 6s5f³F₂ at 764.95 nm
(source: Z W Barber et al. PRL 2008.pdf)

For circularly polarized light, the 3P₀→3P₀ two-photon resonance is absent by selection rules, significantly reducing the hyperpolarizability. This suggests using circular polarization or "magic ellipticity" to cancel $\tilde{\beta}$. (source: Z W Barber et al. PRL 2008.pdf)

## Operational Magic Wavelength

Brown 2017 demonstrated an "operational magic wavelength" where the negative E1 polarizability correction partially cancels the positive hyperpolarizability shift:

$$\nu_\text{op.magic}(U) \equiv \nu_\text{zero} + \frac{-2\beta^* U}{\partial\alpha^*/\partial\nu}$$

At this frequency and trap depth, the clock shift has first-order insensitivity to trap depth fluctuations: a 10% change in U causes only ~10⁻¹⁹ change in fractional frequency. For Brown 2017's parameters at 50 $E_r$: operational magic wavelength is 2.2(1) MHz above $\nu_\text{zero}$. (source: R C Brown et al. PRL 2017.pdf)

## Tensor and Vector Light Shifts

For odd isotopes (¹⁷¹Yb, I=1/2), the tensor light shift is **absent** because the maximum angular momentum of the J=0 clock states is insufficient to produce a tensor component. The vector light shift is present but can be suppressed to below 10⁻¹⁸ by:
1. Linear lattice polarization (A≈0).
2. Geometry (lattice along quantization axis).
3. Averaging over both $m_F = \pm1/2$ transitions.
(source: N D Lemke et al. PRL 2009.pdf)

## Evaluated Uncertainties (¹⁷¹Yb)

| Year | Lab | First-order | Nonlinear | Total lattice |
|------|-----|-------------|-----------|---------------|
| 2009 | NIST | 2.0×10⁻¹⁶ | 0.7×10⁻¹⁶ | ~2.1×10⁻¹⁶ |
| 2017 | NIST | — | 1.2×10⁻¹⁸ | 1.2×10⁻¹⁸ |
| 2025 | NIST | <10⁻¹⁸ | <10⁻¹⁸ | <10⁻¹⁸ |

(sources: N D Lemke et al. PRL 2009.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf)

## Related pages

- [[magic-wavelength]]
- [[hyperpolarizability]]
- [[multipolarizability]]
- [[optical-lattice-clock]]
- [[systematic-uncertainty-budget]]
