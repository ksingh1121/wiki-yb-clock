# Barber et al. PRL 2008

**Summary**: Precision measurement of lattice light shifts in ¹⁷⁴Yb, refining the magic frequency to 394,799,475(35) MHz and making the first measurement of the hyperpolarizability shift (170±33 mHz at 500 E_r), along with the proposal to use circular polarization to suppress it.

**Sources**: Z W Barber et al. PRL 2008.pdf

**Last updated**: 2026-04-26

---

## Reference

Z. W. Barber, J. E. Stalnaker, N. D. Lemke, N. Poli, C. W. Oates, T. M. Fortier, S. A. Diddams, L. Hollberg, C. W. Hoyt, A. V. Taichenachev, and V. I. Yudin, "Optical Lattice Induced Light Shifts in an Yb Atomic Clock," *Phys. Rev. Lett.* **100**, 103002 (2008).

## Context

This paper systematically characterized the three contributions to the lattice light shift in ¹⁷⁴Yb: (1) the E1 differential polarizability (linear in $U$), (2) the M1E2 multipolarizability (at that time considered but not cleanly separated), and (3) the hyperpolarizability (quadratic in $U$, arising from nearby two-photon resonances). The earlier Barber 2006 paper had only roughly located the magic wavelength; this paper measured it much more precisely.

## Key Results

- **Magic frequency** (¹⁷⁴Yb): 394,799,475(35) MHz — ~35 MHz uncertainty
- **Hyperpolarizability shift**: 170(33) mHz at trap depth $U = 500 E_r$, linear polarization
  - Fractional: $170 \text{ mHz} / (518 \text{ THz}) \approx 3.3\times10^{-16}$
- **Two-photon resonances identified** (from 3P₀):
  - 3P₀ → 6s8p³P₀ at 759.7082 nm (~184 GHz above magic λ)
  - 3P₀ → 6s8p³P₂ at 754.23 nm
  - 3P₀ → 6s5f³F₂ at 764.95 nm
- **Circular polarization suppression**: With circular lattice polarization, the 3P₀→3P₀ two-photon path vanishes by selection rules, substantially reducing $\tilde{\beta}$

## Magic Frequency Measurement

The magic frequency was measured using the **slope method**: the clock frequency shift vs. trap depth was measured at several lattice wavelengths. The slope $d(\delta\nu)/dU$ is proportional to $\Delta\alpha(\nu_L)$. Plotting slope vs. frequency and finding the zero crossing gives $\nu_\text{magic}$.

At 35 MHz uncertainty, the residual fractional first-order light shift uncertainty at $U=500 E_r$ is:

$$\sigma(\delta\nu/\nu) \approx \frac{\partial\tilde{\alpha}_{E1}}{\partial\nu} \cdot 35\text{ MHz} \cdot 500 \approx 7\times10^{-16}$$

Further refinement to 100 kHz precision was projected to give $10^{-18}$ first-order uncertainty.

## Hyperpolarizability Measurement

The quadratic shift $\delta\nu \propto U^2$ was isolated by operating at the (E1) magic frequency and varying $U$. The nonlinear component gave $170(33)$ mHz at $U=500 E_r$.

This is the first experimental measurement of the Yb hyperpolarizability. The identification of the dominant two-photon resonance at 759.7082 nm (only 184 GHz from the magic wavelength) explains the relatively large value.

## Polarization Proposal

For a circularly polarized lattice, the $3P_0 \to 3P_0$ two-photon resonance (which contributes dominantly to $\tilde{\beta}$ for linear polarization) vanishes by selection rules because $\Delta m_J = 0$ is required for $J=0 \to J=0$ via two $\sigma^\pm$ photons but is forbidden. This suggests that circular polarization or "magic ellipticity" could eliminate the hyperpolarizability shift — a concept pursued in later work.

## Isotope Note

Although this paper uses ¹⁷⁴Yb with MIS, the magic wavelength measured here differs from ¹⁷¹Yb by ~1146 MHz (due to isotope shift in polarizability from hyperfine interaction). The qualitative physics and the two-photon resonance identification apply to ¹⁷¹Yb as well.

## Related pages

- [[lattice-light-shift]]
- [[hyperpolarizability]]
- [[magic-wavelength]]
- [[multipolarizability]]
- [[magnetic-field-induced-spectroscopy]]
