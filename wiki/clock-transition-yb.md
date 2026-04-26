# Clock Transition in Yb

**Summary**: The ¹S₀→³P₀ optical clock transition in neutral ytterbium at 578.42 nm (~518 THz), its physical origin, measured frequency, linewidth, and role as the frequency reference.

**Sources**: C W Hoyt et al. PRL 2005.pdf, Z W Barber et al. PRL 2005.pdf, N D Lemke et al. PRL 2009.pdf, T Kohno et al. APE 2009.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## The Transition

The clock transition is the doubly forbidden ¹S₀(6s²) → ³P₀(6s6p) transition at approximately 578.42 nm. It is forbidden because:
1. The spin-selection rule ΔS=0 is violated (singlet→triplet).
2. For J=0→J=0, electric-dipole transitions are strictly forbidden.

In the **odd isotopes** (¹⁷¹Yb, ¹⁷³Yb), hyperfine interaction between the nucleus (I≠0) and the electronic angular momentum mixes a small fraction of the ³P₁ state into ³P₀, relaxing rule (1) and giving a finite (but tiny) E1 transition probability. The resulting natural linewidth is ~44 mHz (¹⁷¹Yb) and the lifetime is ~23–26 s.

In the **even isotopes** (¹⁷⁴Yb, etc.), neither mechanism operates and the transition is strictly forbidden. It can be opened using a static magnetic field; see [[magnetic-field-induced-spectroscopy]].

## Measured Absolute Frequencies

| Isotope | Frequency | Uncertainty | Source |
|---------|-----------|-------------|--------|
| ¹⁷¹Yb (F=1/2→F=1/2) | 518,295,836,591.6(4.4) kHz | 4.4 kHz | Hoyt 2005 (MOT) |
| ¹⁷³Yb (F=5/2→F=5/2) | 518,294,576,847.6(4.4) kHz | 4.4 kHz | Hoyt 2005 (MOT) |
| ¹⁷¹Yb | **518,295,836,590,865.2(0.7) Hz** | 0.7 Hz | Lemke 2009 (lattice) |
| ¹⁷¹Yb | 518,295,836,590,864(28) Hz | 28 Hz | Kohno 2009 (lattice) |

(sources: C W Hoyt et al. PRL 2005.pdf, N D Lemke et al. PRL 2009.pdf, T Kohno et al. APE 2009.pdf)

The NIST Lemke 2009 value (0.7 Hz uncertainty) is the most precise measurement of the absolute frequency. The NMIJ Kohno 2009 value agrees within uncertainties.

**Isotope shift**: ν(¹⁷¹Yb) − ν(¹⁷⁴Yb) = 1,811,281,647.4(1.1) Hz, as determined by combining the Lemke 2009 and Poli 2008 measurements. (source: N D Lemke et al. PRL 2009.pdf)

**Isotope shift**: ν(¹⁷¹Yb) − ν(¹⁷³Yb) = 1,259,744.0 kHz, as measured in a MOT. (source: C W Hoyt et al. PRL 2005.pdf)

## Transition Properties

- **Wavelength**: 578.42 nm (yellow)
- **Frequency**: 518,295,836,590,865.2 Hz ≈ 518.3 THz
- **Natural linewidth (¹⁷¹Yb)**: ~44 mHz
- **Lifetime (³P₀)**: ~23 s (¹⁷¹Yb), ~26 s (¹⁷³Yb)
- **Quality factor Q = ν/Δν**: ~10¹⁶ for 1 Hz spectroscopy, up to ~10¹⁴ demonstrated (Lemke 2009 achieves 5.5 Hz FWHM, Q=10¹⁴ at 160 ms interrogation)

## Spectroscopy Methods

**In a MOT (free atoms)**: First observations (Hoyt 2005, Barber 2005). Clock transition driven on cold (~50–80 µK) atoms in a green MOT. Line shapes are Doppler broadened; widths of hundreds of kHz for 50–80 µK samples. Major systematic: Doppler shift from cloud drift velocity (~4 kHz uncertainty). Not Lamb-Dicke confined.

**In an optical lattice (confined atoms)**: Lattice at [[magic-wavelength]] ~759 nm confines atoms in the Lamb-Dicke regime. Doppler and recoil shifts suppressed. Fourier-limited linewidths achievable: Barber 2006 observed 20 Hz FWHM (64 ms pulse); Lemke 2009 observed 5.5 Hz FWHM (160 ms pulse) with Q=10¹⁴.

## Laser Source at 578 nm

578 nm is not readily available from standard diode or solid-state lasers. Two main approaches:
1. **Dye laser**: Used by NIST group (Barber, Lemke). Narrow linewidth <1 Hz, but requires dye circulation.
2. **Sum-frequency generation (SFG)**: Used by NMIJ (Kohno 2009) and ECNU (Gao 2018). 1030-nm Yb:YAG + 1319-nm Nd:YAG → 578 nm via PPLN waveguide. All-solid-state.

Both approaches achieve sub-Hz linewidth by locking to an ultra-low-expansion (ULE) Fabry-Pérot reference cavity with finesse >10⁵.

## Detection: Electron Shelving

Excitation to the long-lived ³P₀ state is detected via the electron shelving technique: atoms remaining in ¹S₀ after the clock pulse are detected by blue (399 nm) fluorescence, while atoms shelved in ³P₀ are dark. To measure excited state population, atoms are pumped back to ¹S₀ via the 3P₀→3D₁ transition at 1388 nm and then detected. A three-pulse detection sequence (ground state, background, excited state) provides a normalized excitation fraction. (source: N D Lemke et al. PRL 2009.pdf)

## Related pages

- [[yb-atomic-structure]]
- [[optical-lattice-clock]]
- [[magic-wavelength]]
- [[magnetic-field-induced-spectroscopy]]
- [[clock-stability]]
- [[systematic-uncertainty-budget]]
- [[zeeman-shift]]
