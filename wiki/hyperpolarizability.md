# Hyperpolarizability

**Summary**: The fourth-order (two-photon) AC Stark shift of the clock transition due to the optical lattice field, scaling as U², arising from nearby two-photon resonances from the 3P₀ clock state.

**Sources**: Z W Barber et al. PRL 2008.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf

**Last updated**: 2026-04-26

---

## Physical Origin

The hyperpolarizability arises from the fourth-order interaction of the lattice electric field with the atom. In perturbation theory, this is a two-photon process: the lattice field simultaneously drives two electric-dipole transitions. For the clock transition, what matters is the **differential** hyperpolarizability between 3P₀ and 1S₀.

For a 1D standing-wave lattice at depth $U$ (in units of recoil energy $E_r$), the fractional frequency shift is:

$$\frac{\delta\nu_\text{HP}}{\nu_\text{clock}} = -\tilde{\beta} U^2$$

Because the lattice intensity $I \propto U$, this is indeed a fourth-order field effect (or second-order in intensity).

## Two-Photon Resonances in Yb

The hyperpolarizability is dominated by nearby two-photon resonances from the 3P₀ clock state. For ¹⁷¹Yb at the ~759 nm magic wavelength:

| Resonance | Wavelength | Detuning from magic λ | Source |
|-----------|-----------|----------------------|--------|
| 3P₀ → 6s8p³P₀ | 759.7082 nm | ~184 GHz (closest) | Barber 2008 |
| 3P₀ → 6s8p³P₂ | 754.23 nm | — | Barber 2008 |
| 3P₀ → 6s5f³F₂ | 764.95 nm | — | Barber 2008 |

The 3P₀→6s8p³P₀ resonance at 759.7082 nm is the dominant contributor because it lies only ~184 GHz from the magic wavelength, making the two-photon detuning only ~184 GHz / (2 × ~518 THz) — a small fraction of the clock frequency. (source: Z W Barber et al. PRL 2008.pdf)

This proximity of the magic wavelength to a two-photon resonance is a key disadvantage of Yb compared to Sr, where the analogous resonances are farther away and the hyperpolarizability is smaller.

## Polarization Dependence

For **circular polarization**, the two-photon path 3P₀(J=0) → 3P₀(J=0) is absent by electric-dipole selection rules (ΔJ = 0 forbidden for two identical circular photons when J=0). This significantly reduces $\tilde{\beta}$ for circular polarization compared to linear. The concept of **magic ellipticity** — an elliptical polarization at which $\tilde{\beta} = 0$ — has been proposed as a way to operate at zero hyperpolarizability shift. (source: Z W Barber et al. PRL 2008.pdf)

## Measured and Notation-Dependent Values

The hyperpolarizability is quoted in several different ways across papers, and the values are **not** directly interchangeable:

| Quantity | Symbol | Value | Conditions | Source |
|----------|--------|-------|------------|--------|
| Absolute shift | — | 170(33) mHz | At 500 $E_r$, linear polarization | Barber 2008 |
| Finite-temperature effective | $\beta^*$ | $-5.5(2)\times10^{-22}$ | Thermal sample (T∝U), ¹⁷¹Yb | Brown 2017 |
| Harmonic (T=0, intrinsic) | $\tilde{\beta}$ | $-1.7(4)\times10^{-21}$ | Harmonic trap eigenstate basis | Bothwell 2025 |

(sources: Z W Barber et al. PRL 2008.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf)

### Convention warning: $\beta^*$ vs $\tilde{\beta}$

These two quantities measure the same physical effect but under different assumptions about the atomic motional state:

- **$\tilde{\beta}$** is the intrinsic two-photon differential polarizability, calculated for atoms in a single harmonic trap eigenstate (typically the ground state $n_z=0$). It represents a T=0, single-atom quantity.
- **$\beta^*$** is an effective coefficient measured in a thermal ensemble where the trap depth $T \propto U$. Thermally excited atoms are spatially delocalized and experience lower average lattice intensity (they spend time near the nodes of the standing wave). The result is $|\beta^*| < |\tilde{\beta}|$.

Brown 2017 finds $\beta^* \approx -5.5\times10^{-22}$, while Bothwell 2025 finds $\tilde{\beta} \approx -1.7\times10^{-21}$. The ratio $|\beta^*/\tilde{\beta}| \approx 0.32$, reflecting the significant motional averaging at finite temperature. Always check which quantity is being quoted before comparing numbers.

## Interaction with E1 Term: Operational Magic Wavelength

Because $\tilde{\beta} < 0$ (shift is positive, since $-\tilde{\beta}U^2 > 0$) while the E1 polarizability slope allows negative corrections at frequencies above $\nu_\text{zero}$, one can choose a lattice frequency slightly above $\nu_\text{zero}$ such that the two shifts partially cancel. This is the **operational magic wavelength** concept:

$$\nu_\text{op.magic}(U) = \nu_\text{zero} + \frac{-2\beta^* U}{\partial\alpha^*/\partial\nu}$$

At this frequency the derivative of the total shift with respect to U vanishes, giving first-order insensitivity to trap depth fluctuations. For Brown 2017's parameters at $U = 50 E_r$, the operational magic wavelength is 2.2(1) MHz above $\nu_\text{zero}$. (source: R C Brown et al. PRL 2017.pdf)

## Uncertainty Contribution

| Year | Lab | Hyperpolarizability uncertainty (fractional) | Source |
|------|-----|----------------------------------------------|--------|
| 2008 | NIST | ~3×10⁻¹⁶ (at 500 $E_r$) | Barber 2008 |
| 2017 | NIST | 1.2×10⁻¹⁸ (at 50 $E_r$, operational magic λ) | Brown 2017 |
| 2025 | NIST | <10⁻¹⁸ | Bothwell 2025 |

The evolution from 10⁻¹⁶ to 10⁻¹⁸ required lower trap depths and the operational magic wavelength technique. (sources: Z W Barber et al. PRL 2008.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf)

## Related pages

- [[lattice-light-shift]]
- [[multipolarizability]]
- [[magic-wavelength]]
- [[optical-lattice-clock]]
- [[systematic-uncertainty-budget]]
