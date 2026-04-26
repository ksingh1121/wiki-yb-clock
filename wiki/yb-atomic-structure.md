# Yb Atomic Structure

**Summary**: Energy level structure of ytterbium relevant to optical lattice clocks, covering the clock states, cooling transitions, isotopes, and nearby metastable states.

**Sources**: C W Hoyt et al. PRL 2005.pdf, Z W Barber et al. PRL 2005.pdf, T Kohno et al. APE 2009.pdf, M S Safronova et al. PRL 2018.pdf, V Dzuba et al. PRA 2018.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Ground State and Valence Configuration

Ytterbium (Z=70) is an alkaline-earth-like element with ground state [Xe] 4f¹⁴6s² ¹S₀. The filled 4f shell means the ground state is a true J=0 singlet, closely analogous to the alkaline earths (Ca, Sr) but heavier and with richer level structure due to the nearby 4f-hole configurations.

The two valence electrons give rise to singlet (¹S, ¹P, ¹D, ...) and triplet (³P, ³D, ...) manifolds. Intercombination transitions between singlet and triplet states are weakly allowed and form the basis of the clock and narrow cooling transitions.

## Key Energy Levels and Transitions

| State         | Config    | Energy (cm⁻¹) | Lifetime               |
| ------------- | --------- | ------------- | ---------------------- |
| 1S₀           | 4f¹⁴6s²   | 0             | ∞                      |
| 3P₀           | 4f¹⁴6s6p  | 17288         | 23–26 s (odd isotopes) |
| 3P₁           | 4f¹⁴6s6p  | 17992         | 500 ns                 |
| 3P₂           | 4f¹⁴6s6p  | 19710         | ~15 s (even isotopes)  |
| 1P₁           | 4f¹⁴6s6p  | 25068         | 5 ns                   |
| 4f¹³5d6s² J=2 | 4f¹³5d6s² | 23188         | ~200 s                 |

(source: V Dzuba et al. PRA 2018.pdf, M S Safronova et al. PRL 2018.pdf)

## Transitions Used in Lattice Clock Experiments

**First-stage cooling (strong transition)**: 6s² ¹S₀ → 6s6p ¹P₁ at **399 nm**, natural linewidth Γ/2π = 28 MHz. Used for Zeeman slowing, first-stage MOT, and ground-state detection (electron shelving). (source: C W Hoyt et al. PRL 2005.pdf)

**Second-stage cooling (intercombination line)**: ¹S₀ → 3P₁ at **556 nm**, natural linewidth Γ/2π = 182 kHz. Provides sub-Doppler cooling to ~6–40 µK, loading into the optical lattice. (source: T Kohno et al. APE 2009.pdf)

**Clock transition**: ¹S₀ → 3P₀ at **578.42 nm** (~518 THz), natural linewidth ~44 mHz (¹⁷¹Yb and ¹⁷³Yb due to hyperfine mixing; strictly forbidden in even isotopes). (source: T Kohno et al. APE 2009.pdf)

**3P₀ repump**: 3P₀ → 3D₁ at **1388 nm**, used to pump atoms from 3P₀ back to 1S₀ for detection in the excited-state fraction measurement. (source: N D Lemke et al. PRL 2009.pdf)

## Stable Isotopes

Yb has seven stable isotopes:

| Isotope | Abundance | Nuclear spin | Fermion/Boson |
|---------|-----------|-------------|---------------|
| ¹⁶⁸Yb | 0.13% | 0 | Boson |
| ¹⁷⁰Yb | 3.04% | 0 | Boson |
| ¹⁷¹Yb | 14.28% | **1/2** | **Fermion** |
| ¹⁷²Yb | 21.83% | 0 | Boson |
| ¹⁷³Yb | 16.13% | **5/2** | **Fermion** |
| ¹⁷⁴Yb | 31.83% | 0 | **Boson (most abundant)** |
| ¹⁷⁶Yb | 12.76% | 0 | Boson |

(source: C W Hoyt et al. PRL 2005.pdf)

The odd isotopes ¹⁷¹Yb (I=1/2) and ¹⁷³Yb (I=5/2) have hyperfine structure that weakly allows the 1S₀→3P₀ transition through state mixing. ¹⁷⁴Yb is the most abundant but its clock transition requires external magnetic field (MIS). ¹⁷¹Yb is favoured for lattice clocks due to its simple I=1/2 spin structure.

## The 3P₀ Clock State

The 3P₀ state is metastable. In the odd isotopes, hyperfine interaction mixes a small fraction of the nearby 3P₁ state into 3P₀, giving a finite dipole matrix element for the 1S₀→3P₀ transition. The induced linewidth is:
- ¹⁷¹Yb: natural linewidth ~44 mHz (lifetime 23 s) (source: T Kohno et al. APE 2009.pdf)
- ¹⁷³Yb: lifetime ~26 s (source: V Dzuba et al. PRA 2018.pdf)

In even isotopes (J=0→J=0 is strictly forbidden), the transition can be opened by a static magnetic field that mixes ³P₁ (m_J=0) into ³P₀; this is [[magnetic-field-induced-spectroscopy]].

## Hyperfine Structure of ¹⁷¹Yb

For I=1/2, the 1S₀ ground state has F=1/2 only (no splitting). The 3P₀ state also has F=1/2. The clock transition is ¹S₀(F=1/2) → ³P₀(F=1/2), with two π-transitions (m_F = ±1/2 → m_F = ±1/2) split by the first-order Zeeman effect (210 Hz/G separation). The simplicity of I=1/2 is a major advantage over ⁸⁷Sr (I=9/2). (source: N D Lemke et al. PRL 2009.pdf)

## Additional Metastable States and Proposed Clock Transitions

Beyond the 1S₀→3P₀ transition, Yb has two additional metastable states accessible from the ground state or from 3P₀:

**3P₂ transition (1S₀→3P₂ at 507 nm / 431 nm)**: An M2 (magnetic quadrupole) transition between ground state and 3P₂. Lifetime ~15 cs for even isotopes. This has been proposed as a second clock transition alongside 1S₀→3P₀. (source: V Dzuba et al. PRA 2018.pdf)

**4f¹³5d6s² J=2 transition (3P₀→J=2 at ~1695 nm)**: This is the proposed [[dual-clock-transitions-yb]] transition. The J=2 state has an open 4f shell (configuration 4f¹³), giving it exceptional sensitivity to variation of the fine-structure constant (K=−15). (source: M S Safronova et al. PRL 2018.pdf)

## Related pages

- [[clock-transition-yb]]
- [[magic-wavelength]]
- [[magnetic-field-induced-spectroscopy]]
- [[dual-clock-transitions-yb]]
- [[zeeman-shift]]
- [[fundamental-constants-variation]]
