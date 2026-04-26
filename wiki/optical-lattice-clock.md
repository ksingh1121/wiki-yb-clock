# Optical Lattice Clock

**Summary**: An atomic frequency standard in which an ensemble of neutral atoms is trapped in a magic-wavelength optical standing wave and interrogated on an ultranarrow optical transition.

**Sources**: Takamoto et al. nature 2005.pdf, A Ludlow et al. RMP 2015.pdf, N D Lemke et al. PRL 2009.pdf

**Last updated**: 2026-04-26

---

## Operating Principle

An optical lattice clock (OLC) combines the signal-averaging advantage of neutral-atom ensembles with the motional control of trapped-ion systems. The key steps are:

1. **Cool and trap** ~10⁴–10⁵ neutral atoms (¹⁷¹Yb, ⁸⁷Sr, ...) in a magneto-optical trap.
2. **Load** into an optical standing wave at the [[magic-wavelength]], confining atoms in the Lamb-Dicke regime.
3. **Interrogate** with an ultranarrow clock laser on the 1S₀→3P₀ transition.
4. **Detect** the excitation fraction via electron shelving fluorescence.
5. **Lock** the clock laser to the atomic resonance via a servo loop.

The optical lattice potential is formed by a retroreflected focused laser beam, creating a series of pancake-shaped trapping sites with spacing λ_L/2 ~380 nm. Typically 10³–10⁴ lattice sites are occupied, each containing one to a few atoms.

## Stability

The quantum-projection-noise (QPN) limited Allan deviation is:
$$\sigma_y(\tau) \approx \frac{1}{2\pi\nu_0} \sqrt{\frac{T_c}{N \cdot T_\text{int} \cdot \tau}}$$

where N is the atom number, $T_c$ is the cycle time, $T_\text{int}$ the interrogation time, and $\tau$ the averaging time. For $N=10^4$, $T_c=1$ s, $T_\text{int}=0.5$ s: $\sigma_y \sim 3\times10^{-17}/\sqrt{\tau}$. In practice, Dick effect noise from the pulsed interrogation limits short-term stability; see [[clock-stability]]. (source: Takamoto et al. nature 2005.pdf, A Ludlow et al. RMP 2015.pdf)

## Lamb-Dicke Regime

Atoms are in the Lamb-Dicke regime when their motional amplitude $\Delta x \ll \lambda_\text{clock}/(2\pi)$, i.e., $\eta = k_\text{clock}\Delta x \ll 1$ (Lamb-Dicke parameter). In this regime, the first-order Doppler effect and photon recoil are suppressed. Typical lattice depths of 50–500 $E_r$ ($E_r = h^2/(2m\lambda^2)$) give vibrational frequencies $\omega_z \sim 2\pi\times 50$–150 kHz along the lattice axis, confining atoms well within the Lamb-Dicke limit.

## Electron Shelving Detection

Excitation fraction is measured via the 399 nm cycling transition. Atoms in 1S₀ fluoresce; atoms shelved in 3P₀ are dark. The normalized excitation fraction is computed from three 399 nm pulses:
1. Detect ground-state atoms → heat them away.
2. Detect background (from thermal beam).
3. Pump atoms back 3P₀→3D₁→1S₀ (via 1388 nm repump), detect excited-state atoms.

Normalization suppresses shot-to-shot atom number fluctuations. The NIST NIST-Yb clock achieves signal-to-noise approaching quantum projection noise limit with >100 atoms/site. (source: N D Lemke et al. PRL 2009.pdf)

## Comparison with Single-Ion Clocks

| Feature | Optical Lattice Clock | Single-Ion Clock |
|---------|----------------------|-----------------|
| Number | 10³–10⁵ atoms | 1 ion |
| Short-term stability | Excellent (∝1/√N) | Limited |
| Systematic uncertainty | Excellent (<10⁻¹⁸) | Excellent (<10⁻¹⁸) |
| Collisional shifts | Need care (density) | Absent |
| Trap perturbation | Managed via magic λ | Near zero (Paul trap) |
| Species | Neutral (Yb, Sr, Hg, ...) | Ions (Al⁺, Yb⁺, Sr⁺, ...) |

The optical lattice clock was proposed and demonstrated as a way to get the best of both: motional control from tight confinement, and signal averaging from many atoms.

## Yb vs Sr

Both Yb and Sr are leading candidates. Key differences:
- **Magic wavelength**: Sr ~813 nm (near 1P₁ resonance); Yb ~759 nm. Yb's magic wavelength is closer to two-photon resonances (759.7 nm, 754.23 nm), leading to larger [[hyperpolarizability]] shifts at the same trap depth.
- **BBR shift**: Yb's differential static polarizability Δα(0) = 145.726(3) a.u. is larger than Sr's, giving a larger [[blackbody-radiation-shift]] that is nonetheless well-characterised.
- **Isotope**: ¹⁷¹Yb (I=1/2) is simpler than ⁸⁷Sr (I=9/2) for polarization control and state preparation.
- **Cooling**: Yb has a convenient two-stage cooling scheme (399 nm + 556 nm). Sr uses 461 nm + 689 nm.

## Performance Milestones (Yb)

| Year | Lab | Systematic uncertainty | Reference |
|------|-----|----------------------|-----------|
| 2009 | NIST | 3.4×10⁻¹⁶ | Lemke 2009 |
| 2018 | ECNU | 1.7×10⁻¹⁶ | Gao 2018 |
| 2017 | NIST | 1.2×10⁻¹⁸ (lattice light shift) | Brown 2017 |

## Related pages

- [[clock-transition-yb]]
- [[magic-wavelength]]
- [[lattice-light-shift]]
- [[clock-stability]]
- [[systematic-uncertainty-budget]]
- [[blackbody-radiation-shift]]
- [[density-shift]]
- [[yb-atomic-structure]]
