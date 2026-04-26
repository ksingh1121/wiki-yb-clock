# Hoyt et al. PRL 2005

**Summary**: First spectroscopy of the ¹⁷¹Yb and ¹⁷³Yb 1S₀→3P₀ clock transitions in a laser-cooled MOT sample, establishing the absolute frequencies and demonstrating that odd-isotope Yb is viable for a lattice clock.

**Sources**: C W Hoyt et al. PRL 2005.pdf

**Last updated**: 2026-04-26

---

## Reference

C. W. Hoyt, Z. W. Barber, C. W. Oates, T. M. Fortier, S. A. Diddams, and L. Hollberg, "Observation and absolute frequency measurements of the ¹S₀–³P₀ optical clock transition in neutral ytterbium," *Phys. Rev. Lett.* **95**, 083003 (2005).

## Context

This paper predates the first Yb optical lattice clock by several years. Its goal was to confirm that the 1S₀→3P₀ clock transition in ¹⁷¹Yb and ¹⁷³Yb could be driven and detected in cold atoms, and to measure its absolute frequency. The atoms were in a MOT (not a lattice), so the spectroscopy was not Lamb-Dicke confined and systematic uncertainties were large (kHz level), but the absolute frequency was anchored to an optical frequency comb referenced to H-maser + GPS.

## Key Results

| Isotope | Measured frequency | Uncertainty |
|---------|-------------------|-------------|
| ¹⁷¹Yb (F=1/2→F=1/2) | 518,295,836,591.6 kHz | 4.4 kHz |
| ¹⁷³Yb (F=5/2→F=5/2) | 518,294,576,847.6 kHz | 4.4 kHz |

**Isotope shift**: $\nu(^{171}\text{Yb}) - \nu(^{173}\text{Yb}) = 1,259,744.0$ kHz (from the above values).

The 4.4 kHz uncertainty was dominated by the Doppler shift from the MOT cloud's bulk motion and the uncertainty in the optical frequency comb calibration.

## Experimental Method

1. ¹⁷¹Yb and ¹⁷³Yb atoms cooled in a 556 nm green MOT to ~40 µK
2. Clock laser at 578 nm drives the transition with $\sim$100 ms pulses
3. Detection via electron shelving: excited atoms detected by absence of 399 nm fluorescence
4. Absolute frequency measured by optical frequency comb (Er:fiber-based, referenced to H-maser)
5. Measured frequency vs. cooling intensity, cloud displacement, etc. to extrapolate to zero systematic

## Dominant Systematic: Doppler Shift

In a free-atom MOT sample (not Lamb-Dicke), the Doppler shift from bulk cloud velocity dominates. The NIST group found the cloud drifts at up to ~4 mm/s under gravity and push-beam imbalance, contributing a ~4 kHz frequency uncertainty. In a lattice, this effect is suppressed by the Lamb-Dicke confinement.

## Significance for Lattice Clocks

This paper confirmed the basic physical picture: ¹⁷¹Yb has a clock transition accessible with a tunable dye laser at 578 nm, with a natural linewidth of ~44 mHz (lifetime ~23 s), and the hyperfine coupling (I=1/2) provides the state mixing that opens the otherwise forbidden transition. It established the starting absolute frequency for all subsequent more precise lattice measurements.

## Related pages

- [[clock-transition-yb]]
- [[yb-atomic-structure]]
- [[optical-lattice-clock]]
