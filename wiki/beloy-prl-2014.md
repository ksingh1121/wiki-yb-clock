# Beloy et al. PRL 2014

**Summary**: Demonstration of a room-temperature in-vacuum copper BBR shield that reduces the blackbody radiation shift uncertainty of the ¹⁷¹Yb lattice clock to 10⁻¹⁸, combined with ab initio calculation of the dynamic correction coefficients η₁ and η₂.

**Sources**: K Beloy et al. PRL 2014.pdf

**Last updated**: 2026-04-26

---

## Reference

K. Beloy, N. Hinkley, N. B. Phillips, J. A. Sherman, M. Schioppo, J. Lehman, A. Feldman, L. M. Hanssen, C. W. Oates, and A. D. Ludlow, "Atomic Clock with 1×10⁻¹⁸ Room-Temperature Blackbody Stark Uncertainty," *Phys. Rev. Lett.* **113**, 260801 (2014).

## Context

After Sherman 2012 measured $\Delta\alpha(0)$ to ppm precision, the remaining BBR uncertainty was set by temperature measurement of the apparatus environment. At 300 K, $\partial(\sigma_\text{BBR})/\partial T \approx 3.3\times10^{-18}$/K, meaning $\pm 0.3$ K gives $10^{-18}$ uncertainty. Standard room-temperature environments are inhomogeneous at the 1–10 K level, preventing this goal without a special enclosure.

## The BBR Shield

### Design

An in-vacuum **copper enclosure** surrounds the atom trapping region. Copper was chosen for its high thermal conductivity (~400 W/(m·K)), which minimizes temperature gradients across the shield to $<10$ mK under room-temperature operation.

Key features:
- **Inner surface**: Coated with **carbon nanotube (CNT) paint** for high emissivity ($\epsilon > 0.99$), ensuring the atom sees a near-ideal blackbody at the shield temperature rather than reflections from external sources
- **Temperature sensors**: Calibrated platinum resistance thermometers (PRTs, type Pt-100) mounted directly on the shield walls, read out continuously during clock operation
- **Apertures**: Small holes for the lattice beam, clock laser, MOT beams, and fluorescence collection; sized to minimize external BBR entering the enclosure

### Thermal Characterization

The shield temperature homogeneity was confirmed by comparing multiple RTD readings. The maximum gradient across the shield interior was $\Delta T < 10$ mK. Temporal stability was better than 10 mK over the clock evaluation period.

## Dynamic Correction

Beyond the static polarizability, the BBR spectrum extends to finite frequencies where the polarizability differs from $\Delta\alpha(0)$. The fractional dynamic correction is:

$$\eta_\text{dyn}(T) = \eta_1 \left(\frac{T}{300\text{ K}}\right)^2 + \eta_2 \left(\frac{T}{300\text{ K}}\right)^4$$

Beloy 2014 calculated these coefficients ab initio for ¹⁷¹Yb using relativistic many-body perturbation theory:

| Parameter | Value | Uncertainty |
|-----------|-------|-------------|
| $\eta_1$ | 0.01745 | 0.00038 |
| $\eta_2$ | 0.000593 | 0.000016 |

The dominant contribution to $\eta_1$ comes from the electric-dipole transitions from 1S₀ and 3P₀ to intermediate states. The uncertainty in $\eta_1$ contributes $\sim 10^{-19}$ to the BBR fractional uncertainty at 300 K.

## Achieved BBR Uncertainty

With the copper shield and RTD characterization:

$$\sigma_\text{BBR} = 1\times10^{-18}$$

Breakdown:
- Temperature measurement uncertainty ($\Delta T < 10$ mK): $< 10^{-19}$ contribution
- Dynamic correction theory uncertainty ($\delta\eta_1 = 0.00038$): $\sim 3\times10^{-19}$
- Aperture/reflection corrections: $< 10^{-19}$
- **Total**: $1\times10^{-18}$

## Significance

This paper removed BBR from the list of leading systematic uncertainties in the Yb lattice clock, enabling the total systematic budget to approach $10^{-18}$. The copper-shield approach has been adopted by other groups and is now a standard technique for room-temperature lattice clocks targeting $10^{-18}$ accuracy.

The combination of Sherman 2012 (precise $\Delta\alpha(0)$) and Beloy 2014 (precise thermal environment) reduced the BBR uncertainty by a total factor of $\sim 1000$ from the Lemke 2009 value.

## Related pages

- [[blackbody-radiation-shift]]
- [[bbr-shield]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
- [[sherman-prl-2012]]
