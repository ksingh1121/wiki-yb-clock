# Lemke et al. PRL 2009

**Summary**: First ¹⁷¹Yb optical lattice clock evaluation at NIST, achieving systematic uncertainty of 3.4×10⁻¹⁶ and measuring the absolute clock frequency to 0.7 Hz — the most precise Yb frequency measurement at the time.

**Sources**: N D Lemke et al. PRL 2009.pdf

**Last updated**: 2026-04-26

---

## Reference

N. D. Lemke, A. D. Ludlow, Z. W. Barber, T. M. Fortier, S. A. Diddams, Y. Jiang, S. R. Jefferts, T. P. Heavner, T. E. Parker, and C. W. Oates, "Spin-1/2 Optical Lattice Clock," *Phys. Rev. Lett.* **103**, 063001 (2009).

## Context

This paper is the first systematic evaluation of an optical lattice clock using ¹⁷¹Yb (the fermionic I=1/2 isotope that became the preferred Yb clock species). Prior Yb lattice clock work used ¹⁷⁴Yb with MIS (Barber 2006, 2008). The shift to ¹⁷¹Yb simplified the systematics (no MIS-related quadratic Zeeman, simpler F=1/2 structure) and enabled the use of spin-polarized Fermi statistics to suppress s-wave density shifts.

## Key Results

### Absolute Frequency
$$\nu_{^{171}\text{Yb}} = 518,295,836,590,865.2(0.7) \text{ Hz}$$

This 0.7 Hz uncertainty (fractional $1.3\times10^{-15}$) was measured by referencing to NIST's primary Cs fountain standard (NIST-F1) via an optical frequency comb. It remained the most precise Yb absolute frequency measurement for several years.

**Isotope shift** (from combining with Poli 2008 measurement of ¹⁷⁴Yb):
$$\nu(^{171}\text{Yb}) - \nu(^{174}\text{Yb}) = 1,811,281,647.4(1.1) \text{ Hz}$$

### Magic Frequency
$$\nu_\text{magic}(^{171}\text{Yb}) = 394,798,329(10) \text{ MHz}$$

(~1146 MHz below the ¹⁷⁴Yb magic frequency of Barber 2008, consistent with the isotope shift in polarizability from hyperfine effects.)

### Systematic Uncertainty Budget

| Effect | Fractional uncertainty |
|--------|------------------------|
| BBR shift | $9.7\times10^{-16}$ |
| Lattice first-order light shift | $2.0\times10^{-16}$ |
| Lattice nonlinear (hyperpolarizability) | $0.7\times10^{-16}$ |
| Density/collision shift | $1.0\times10^{-16}$ |
| Second-order Zeeman | $<10^{-17}$ |
| Vector light shift | $3.4\times10^{-17}$ |
| **Total (quadrature)** | **$3.4\times10^{-16}$** |

BBR dominated, with the theoretical uncertainty in $\Delta\alpha(0)$ at ~10% being the largest contributor.

## Experimental Setup

- **Cooling**: 399 nm Zeeman slower → 399 nm MOT (first stage) → 556 nm green MOT (second stage, 6–40 µK)
- **Lattice**: Retroreflected ~759 nm beam, linearly polarized along the quantization axis
- **Clock laser**: Dye laser at 578 nm, narrowed by locking to a ULE Fabry-Pérot cavity (finesse >150,000); sub-Hz linewidth
- **Detection**: Three-pulse electron shelving (399 nm): ground-state, background, excited-state
- **Quantization axis**: Bias B-field ~1 G along the lattice propagation direction
- **Interrogation**: 160 ms Rabi π-pulse, achieving 5.5 Hz FWHM ($Q = 10^{14}$)

## Density Shift Measurement

The collision shift was measured by varying the atom number per lattice site. A slope of approximately $-0.85$ Hz per unit peak 1D density was observed, consistent with p-wave cold collisions in spin-polarized ¹⁷¹Yb. The uncertainty contribution of $1.0\times10^{-16}$ required careful control of loading conditions.

## Vector Light Shift

For ¹⁷¹Yb (J=0), the vector light shift from the lattice is suppressed by:
1. Linear polarization: $A \approx 0$
2. Lattice propagation along the quantization axis
3. Averaging over $m_F = \pm1/2$ transitions

The residual vector light shift uncertainty was $3.4\times10^{-17}$.

## Significance

This paper established ¹⁷¹Yb as the preferred Yb isotope for lattice clocks, demonstrated the full systematic evaluation methodology, and provided an absolute frequency reference that enabled future inter-laboratory comparisons. It also set the stage for the Sherman 2012 measurement that dramatically reduced the BBR uncertainty.

## Related pages

- [[clock-transition-yb]]
- [[magic-wavelength]]
- [[systematic-uncertainty-budget]]
- [[blackbody-radiation-shift]]
- [[density-shift]]
- [[optical-lattice-clock]]
- [[zeeman-shift]]
