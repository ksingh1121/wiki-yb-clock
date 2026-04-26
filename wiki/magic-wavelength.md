# Magic Wavelength

**Summary**: The lattice laser wavelength at which the differential AC Stark shift on the clock transition vanishes, enabling trap-independent spectroscopy at the sub-Hz level.

**Sources**: Takamoto et al. nature 2005.pdf, Z W Barber et al. PRL 2005.pdf, Z W Barber et al. PRL 2008.pdf, N D Lemke et al. PRL 2009.pdf, T Kohno et al. APE 2009.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf

**Last updated**: 2026-04-26

---

## Concept

An atom trapped in an optical lattice experiences an AC Stark shift of its internal energy levels due to the lattice light. The differential shift of the clock transition is:

$$\delta\nu = -\frac{1}{2\epsilon_0 c h} \Delta\alpha(\nu_L) I + O(I^2)$$

where $\Delta\alpha(\nu_L) = \alpha_e(\nu_L) - \alpha_g(\nu_L)$ is the difference in AC polarizability between excited (3P₀) and ground (1S₀) clock states at the lattice laser frequency $\nu_L$, and $I$ is the lattice intensity.

The **magic frequency** $\nu_\text{magic}$ is defined by $\Delta\alpha(\nu_\text{magic}) = 0$: both clock states experience identical AC Stark shifts, leaving the transition frequency unperturbed to first order in lattice intensity. (source: Takamoto et al. nature 2005.pdf)

This concept was first proposed for Sr by Katori (2002) and extended to Yb by Porsev, Derevianko, and Fortson (2004). The theoretical estimate for Yb was ~752 nm initially. (source: C W Hoyt et al. PRL 2005.pdf)

## Measured Magic Frequencies in Yb

| Isotope | Magic frequency (MHz) | Magic wavelength | Source |
|---------|----------------------|------------------|--------|
| ¹⁷⁴Yb | 394,799,475(35) | ~759.3537 nm | Barber 2008 |
| ¹⁷¹Yb | 394,798,329(10) | ~759.354 nm | Lemke 2009 |
| ¹⁷¹Yb | 394,798,267(3) | ~759.354 nm | Brown 2017 (ν_zero) |
| ¹⁷¹Yb | 394,798,266.9(26) | ~759.354 nm | Bothwell 2025 (ν_E1) |
| ¹⁷⁴Yb (rough) | ~759.35(0.02) nm | — | Barber 2006 |
| ¹⁷¹Yb | ~759.353(3) nm | — | Kohno 2009 |

(sources: Z W Barber et al. PRL 2008.pdf, N D Lemke et al. PRL 2009.pdf, R C Brown et al. PRL 2017.pdf, T Bothwell et al. PRL 2025.pdf)

**Convention warning**: The "magic frequency" reported by different groups is not always the same quantity:
- Barber 2008 and Lemke 2009 report the frequency where the **first-order (E1) differential polarizability** $\Delta\alpha_{E1}$ vanishes; this is denoted $\nu_\text{magic}$ or $\nu_{E1}$.
- Brown 2017 defines $\nu_\text{zero}$ as the frequency where the **effective linear coefficient** $\alpha^*$ (which includes both E1 and M1E2 contributions at finite temperature) vanishes. $\nu_\text{zero} \approx \nu_{E1} - \nu_{M1E2}$, shifted by ~400 kHz.
- Bothwell 2025 uses $\nu_{E1}$ explicitly for the E1 zero, and $\nu^0_r(0) = \nu_{E1} - \alpha_{M1E2}/(\partial\alpha_{E1}/\partial\nu)$ for the running-wave magic frequency.

**Isotope dependence**: The ¹⁷¹Yb magic frequency differs from ¹⁷⁴Yb by 1146(36) MHz (Lemke 2009 value). This isotope shift arises from the different hyperfine-induced polarizability contributions. (source: N D Lemke et al. PRL 2009.pdf)

## Measuring the Magic Wavelength

### Slope method (standard)
Measure the clock frequency shift vs. lattice intensity at several lattice wavelengths. The slope $d(\delta\nu)/dI$ is proportional to $\Delta\alpha(\nu_L)$. Plot slope vs. frequency and find the zero crossing. Used by Barber 2008 and Lemke 2009.

### Line broadening and asymmetry
Operating off-magic wavelength causes inhomogeneous broadening (atoms in different lattice sites experience different intensities). Monitoring linewidth and asymmetry provides a coarse indication of the magic wavelength. Used for initial location in Barber 2006.

### Running wave technique (Bothwell 2025)
An auxiliary running wave field is applied to one of two dual ensembles. The running wave magic frequency $\nu^0_r(u_0)$ depends on trap depth and contains both $\nu_{E1}$ and $\alpha_{M1E2}$, allowing them to be disentangled. This is a new technique that separates E1 and M1E2 contributions with minimal correlation. (source: T Bothwell et al. PRL 2025.pdf)

## First-Order Light Shift Uncertainty

Given the measured magic frequency and its uncertainty $\delta\nu_\text{magic}$, the residual first-order light shift for a trap depth $U$ is:

$$\delta\nu_\text{shift} = \frac{\partial\Delta\alpha}{\partial\nu}\bigg|_{\nu=\nu_\text{magic}} \cdot \delta\nu_\text{magic} \cdot U$$

From Brown 2017: $\partial\alpha^*/\partial\nu = 2.46(10)\times10^{-20}$ (1/MHz). For $\delta\nu_\text{magic} = 1$ MHz, $U = 50 E_r$: residual fractional shift $\sim 1\times10^{-18}$.

From Barber 2008: With 35 MHz uncertainty in $\nu_\text{magic}$ and 500 $E_r$ depth: uncertainty in first-order shift is 0.38 Hz (fractional $7\times10^{-16}$). Further refinement to 100 kHz uncertainty possible. (source: Z W Barber et al. PRL 2008.pdf)

## Sr Magic Wavelength (for comparison)

For ⁸⁷Sr, the magic wavelength is ~813.4 nm (Takamoto 2005 measured 813.420(7) nm). This was the first experimental demonstration of a magic wavelength optical lattice clock. (source: Takamoto et al. nature 2005.pdf)

## Related pages

- [[lattice-light-shift]]
- [[hyperpolarizability]]
- [[multipolarizability]]
- [[optical-lattice-clock]]
- [[clock-transition-yb]]
- [[yb-atomic-structure]]
