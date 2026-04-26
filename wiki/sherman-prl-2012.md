# Sherman et al. PRL 2012

**Summary**: Precision measurement of the ¹⁷¹Yb differential static polarizability Δα(0) = 36.2612(7) kHz(kV/cm)⁻² using a calibrated DC electric field, reducing the BBR fractional uncertainty from 10⁻¹⁵ to 3×10⁻¹⁷.

**Sources**: J A Sherman et al. PRL 2012.pdf

**Last updated**: 2026-04-26

---

## Reference

J. A. Sherman, N. D. Lemke, N. Hinkley, M. Pizzocaro, R. W. Fox, A. D. Ludlow, and C. W. Oates, "High-Accuracy Measurement of Atomic Polarizability in an Optical Lattice Clock," *Phys. Rev. Lett.* **108**, 153002 (2012).

## Context

After the Lemke 2009 Yb clock evaluation, the dominant systematic uncertainty was the [[blackbody-radiation-shift]], which scaled with the differential static polarizability $\Delta\alpha(0)$. The prior theoretical value had ~10% uncertainty, contributing a $9.7\times10^{-16}$ fractional frequency uncertainty. This paper eliminated this bottleneck by measuring $\Delta\alpha(0)$ directly at the ppm level.

## Key Results

### Measured Polarizability
$$\Delta\alpha(0) = 36.2612(7) \text{ kHz(kV/cm)}^{-2} = 145.726(3) \text{ a.u.}$$

(The conversion is $1 \text{ kHz(kV/cm)}^{-2} = 4.0189 \text{ a.u.}$ via appropriate unit conversion involving the Bohr radius and atomic energy units.)

Fractional uncertainty: **20 ppm** (3 ppm on the value in a.u., ~7×10⁻⁴ relative uncertainty in kHz(kV/cm)⁻² units — actually 7/36261 ≈ 19 ppm).

### BBR Shift at 300 K (from this measurement)
$$\delta\nu_\text{BBR}(300\text{ K}) = -1.273(17) \text{ Hz}$$
$$\frac{\delta\nu_\text{BBR}}{\nu_\text{clock}} = -2.454(33)\times10^{-16}$$

The 17 mHz absolute uncertainty corresponds to a $3\times10^{-17}$ fractional uncertainty — a 30× improvement over the pre-measurement situation.

## Experimental Method

### DC Stark Shift Measurement

An electric field is applied to the atoms via biased parallel electrodes mounted inside the vacuum chamber. The clock frequency shift as a function of applied voltage $V$ is:

$$\delta\nu = -\frac{\Delta\alpha(0)}{2h} E^2$$

where $E$ is the electric field at the atomic position. The relationship $E = \kappa V$ depends on the electrode geometry through a calibration factor $\kappa$.

### Electrode Calibration

The electrodes (separated by ~5 mm) were designed for a near-uniform field region. The calibration factor $\kappa$ (V/m per applied volt) was computed by finite-element electrostatic simulation and verified by measuring the field distribution with an independent probe. The dominant systematic uncertainty in $\kappa$ was:
1. **Uncertainty in the inter-electrode spacing** (physical measurement)
2. **Higher-order field corrections** (departure from ideal uniform field at the atom cloud position)

### Signal Extraction

The clock frequency was measured vs. applied voltage at several values of $V$. The quadratic dependence $\delta\nu \propto V^2$ gave $\Delta\alpha(0)$ directly. By operating at multiple voltage values, the quadratic coefficient was extracted with a statistical uncertainty of ~6 ppm.

## Significance

This measurement transformed the BBR shift from the dominant systematic ($\sim 10^{-15}$) to a manageable contribution ($3\times10^{-17}$ for $\pm1$ K temperature uncertainty). After this paper, the lattice light shift became the next dominant systematic, motivating the Brown 2017 hyperpolarizability work.

The same technique (DC Stark shift measurement in a lattice clock) has since been applied to Sr and other species.

## Related pages

- [[blackbody-radiation-shift]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
- [[bbr-shield]]
