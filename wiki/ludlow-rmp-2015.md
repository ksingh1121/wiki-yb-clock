# Ludlow et al. RMP 2015

**Summary**: Comprehensive review of optical atomic clocks covering operating principles, systematic effects, stability, and state-of-the-art performance for both single-ion and optical lattice clock platforms as of 2015.

**Sources**: A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Reference

A. D. Ludlow, M. M. Boyd, J. Ye, E. Peik, and P. O. Schmidt, "Optical atomic clocks," *Rev. Mod. Phys.* **87**, 637 (2015).

## Scope and Organization

This 65-page review article is the standard reference for the optical atomic clock field. It covers:

1. **Fundamentals**: atomic physics of clock transitions, trapping, cooling, interrogation
2. **Clock laser technology**: ultrastable cavities, thermal noise limits, PDH locking
3. **Ion clock systems**: Al⁺, Yb⁺, Sr⁺, Ba⁺, Hg⁺, including systematic evaluations
4. **Neutral atom lattice clocks**: Sr, Yb, Hg, Mg, Ca — principles, magic wavelengths, systematic budgets
5. **Clock comparisons and applications**: frequency ratios, geodesy, fundamental physics, timescales

## Key Concepts Covered

### Stability
The review gives the quantum-projection-noise limited Allan deviation:
$$\sigma_y(\tau) \approx \frac{1}{2\pi\nu_0} \sqrt{\frac{T_c}{N \cdot T_\text{int} \cdot \tau}}$$
and discusses the Dick effect as the practical limiting factor. The derivation of the Dick effect from pulsed interrogation and the aliasing of laser phase noise is presented in detail. (source: A Ludlow et al. RMP 2015.pdf)

### Systematic Effects
The review provides a unified treatment of all systematic effects common to optical clocks:
- AC Stark shifts (lattice, probe, stray fields)
- BBR shift (formula, temperature sensitivity, dynamic correction)
- Zeeman shifts (first-order, second-order, vector light shift)
- Density and cold-collision shifts
- Servo offset errors
- Background gas collisions
- Gravitational redshift and relativistic effects

### Magic Wavelength Framework
The concept of the magic wavelength is derived from the AC polarizability formalism. The review explains why E1 magic wavelengths exist and introduces the corrections from higher multipoles (M1, E2) and hyperpolarizability as the framework for understanding the full lattice light shift hierarchy. This framework is implemented in the subsequent Brown 2017 and Bothwell 2025 papers.

### Performance Survey (as of 2015)

| Clock | Lab | Systematic uncertainty (2015) |
|-------|-----|-------------------------------|
| Al⁺/Be⁺ | NIST | $8.6\times10^{-18}$ |
| ⁸⁷Sr | JILA | $6.4\times10^{-18}$ |
| ¹⁷¹Yb | NIST | $1.6\times10^{-18}$ (projected) |
| Yb⁺ (E3) | PTB | $7.1\times10^{-18}$ |

The review reflects the state as of ~2014–2015 and does not include the Brown 2017 or Beloy 2014 results (which post-date its preparation).

## Yb-Specific Content

The review covers Yb lattice clocks specifically, including:
- The 1S₀→3P₀ transition physics (hyperfine-induced linewidth, 44 mHz natural width)
- Magic wavelength at 759 nm and the role of nearby two-photon resonances in the hyperpolarizability
- Comparison of ¹⁷¹Yb vs. ¹⁷³Yb vs. ¹⁷⁴Yb+MIS
- The NIST Yb clock design and systematic evaluation methodology

## Broader Context

The review situates optical clocks within the broader context of:
- **Realization of the SI second**: how optical clocks are compared to Cs fountain primary standards via frequency combs
- **Frequency ratios**: how ratios between different clock species can be measured to test constancy of fundamental constants
- **Chronometric geodesy**: using redshift differences to measure gravitational potential differences
- **Timescale generation**: how optical clock data feeds into international atomic time (TAI)

## Limitations as a Reference

This review covers the field as of ~2015. Key developments not covered:
- Brown 2017 operational magic wavelength
- Beloy 2014 BBR shield (published Dec 2014; likely cited in the review)
- Bothwell 2025 dual-ensemble evaluation
- Sub-$10^{-18}$ total systematic evaluations in Yb or Sr

For developments after 2015, the individual papers should be consulted.

## Related pages

- [[optical-lattice-clock]]
- [[clock-stability]]
- [[systematic-uncertainty-budget]]
- [[blackbody-radiation-shift]]
- [[lattice-light-shift]]
- [[magic-wavelength]]
