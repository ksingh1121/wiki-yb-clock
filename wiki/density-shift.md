# Density Shift (Collisional Shift)

**Summary**: The frequency shift of the clock transition arising from atom-atom interactions (cold collisions) within the optical lattice, primarily from p-wave collisions in spin-polarized fermionic ¹⁷¹Yb.

**Sources**: N D Lemke et al. PRL 2009.pdf, Q Gao et al. SR 2018.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Physical Mechanism

When multiple atoms occupy the same lattice site, they interact via cold collisions. For **fermionic** atoms in a single spin state (spin-polarized), the Pauli exclusion principle suppresses s-wave (contact) collisions at low temperature (since the wave function must be antisymmetric). However, **p-wave** collisions, which are centrifugally suppressed at zero temperature but can be significant at finite temperature ($T \sim \mu$K), give a density-dependent frequency shift.

For spin-polarized ¹⁷¹Yb atoms in $m_F = +1/2$ (or $-1/2$):

$$\delta\nu_\text{coll} = C_\text{p-wave} \cdot \rho \cdot T_\text{eff}^n$$

where $\rho$ is the atomic density, $T_\text{eff}$ is the effective collision temperature, and $C_\text{p-wave}$ is a p-wave collision coefficient. In practice the shift is characterized empirically as a function of atom number per site.

## Convention: Density or Atom-Number Shift?

Different papers parameterize the density shift differently:

- **Lemke 2009**: Quotes a shift slope as frequency vs. atom density $\rho_0$ (peak 1D linear density): slope $\approx -0.85$ Hz per unit $\rho_0$. Here $\rho_0$ is the peak atom number per unit length along the lattice. The total shift requires knowing the density distribution.
- **Gao 2018**: Quotes the shift as a measured frequency difference between two conditions: $-0.570(25)$ Hz, measured directly by comparing clock frequencies at different atom numbers in a synchronous comparison setup.

Always check the normalization convention when comparing collision shift coefficients across papers. (sources: N D Lemke et al. PRL 2009.pdf, Q Gao et al. SR 2018.pdf)

## Lemke 2009 Measurement

In the NIST 2009 evaluation, the density shift was assessed by varying the atom number loaded into the lattice and extrapolating to zero density. The observed slope of $\sim -0.85$ Hz/$\rho_0$ was used to correct the clock frequency. In the 2009 budget this uncertainty was $1.0\times10^{-16}$ — the second-largest contribution after BBR. (source: N D Lemke et al. PRL 2009.pdf)

## Gao 2018 Measurement

The ECNU group measured the density shift using a **synchronous comparison** method: two Yb ensembles loaded from the same MOT are interrogated simultaneously, with one ensemble at high density and the other at low density. This simultaneous measurement cancels common-mode laser noise (Dick effect noise) and allows precise determination of the density-dependent frequency offset.

Result: density shift of $-0.570(25)$ Hz, contributing an uncertainty of $4.9\times10^{-17}$ in the total budget. This measurement represents a significant advance in the methodology for evaluating density shifts in optical lattice clocks. (source: Q Gao et al. SR 2018.pdf)

## Suppression Strategies

1. **Low filling fraction**: Load fewer than 1 atom per lattice site on average. At $\langle n \rangle = 1$, most sites have 0 or 1 atom (Poissonian distribution), minimizing multi-occupancy.
2. **Spin polarization**: All atoms in a single $m_F$ state to suppress s-wave collisions (fermionic case).
3. **Synchronous comparison**: Measure the density-dependent frequency shift in real time by comparing high- and low-density ensembles.
4. **Extrapolation to zero density**: Vary atom number and extrapolate. Requires the shift to be linear in density.

## Bosonic vs. Fermionic Case

For **bosonic** Yb isotopes (¹⁷⁴Yb), s-wave collisions are not suppressed by the Pauli principle, and the density shift can be larger. This is one reason ¹⁷¹Yb (fermionic) is preferred for precision clocks despite the added complexity of hyperfine structure.

For ¹⁷¹Yb, the p-wave suppression at low temperatures ($T \lesssim$ 1 µK) means the density shift can be very small if the sample is cold enough. At typical lattice temperatures of a few µK after sideband cooling, p-wave contributions become relevant.

## Uncertainty in Evaluated Budgets

| Year | Lab | Density shift uncertainty | Source |
|------|-----|--------------------------|--------|
| 2009 | NIST | $1.0\times10^{-16}$ | Lemke 2009 |
| 2018 | ECNU | $4.9\times10^{-17}$ | Gao 2018 |

(sources: N D Lemke et al. PRL 2009.pdf, Q Gao et al. SR 2018.pdf)

## Related pages

- [[optical-lattice-clock]]
- [[clock-transition-yb]]
- [[systematic-uncertainty-budget]]
- [[yb-atomic-structure]]
