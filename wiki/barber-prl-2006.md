# Barber et al. PRL 2006

**Summary**: First optical lattice clock using ¹⁷⁴Yb (bosonic isotope) with magnetic-field-induced spectroscopy (MIS), providing the first measurement of the Yb magic wavelength at 759.35(0.02) nm and demonstrating that MIS enables precision clock operation with even isotopes.

**Sources**: Z W Barber et al. PRL 2005.pdf

**Last updated**: 2026-04-26

---

## Reference

Z. W. Barber, C. W. Hoyt, C. W. Oates, L. Hollberg, A. V. Taichenachev, and V. I. Yudin, "Direct Excitation of the Forbidden Clock Transition in Neutral ¹⁷⁴Yb Atoms Confined to an Optical Lattice," *Phys. Rev. Lett.* **96**, 083002 (2006).

**Note on filename**: The file is named "Z W Barber et al. PRL 2005.pdf" but the paper was published in March 2006 (received November 2005).

## Context

Following the Takamoto 2005 Sr demonstration and the Hoyt 2005 Yb MOT spectroscopy, this paper made the first observation of the Yb 1S₀→3P₀ transition in a Lamb-Dicke confined optical lattice. Because ¹⁷⁴Yb (the most abundant isotope, 31.8%) is bosonic with I=0, its clock transition is strictly forbidden without an external perturbation. The authors used a static magnetic field to mix 3P₁ character into 3P₀ (MIS technique), analogous to what had been proposed by Taichenachev et al.

## Key Results

- **Species**: ¹⁷⁴Yb with magnetic-field-induced spectroscopy
- **Magic wavelength**: 759.35(0.02) nm — first experimental determination for Yb
- **Applied B-field**: ~0.1 mT (1 G) along the quantization axis
- **Clock transition linewidth**: Fourier-limited lines demonstrated (tens of Hz with ms interrogation)
- **Quadratic Zeeman coefficient**: $\beta_\text{QZ} = 6.6(0.4)$ MHz/T² — measured by varying B and extrapolating

## Magic Wavelength Measurement

The magic wavelength was located by the **line broadening and asymmetry method**: off-magic wavelengths cause atoms in different sites to experience different intensities and thus different light shifts, leading to inhomogeneously broadened, asymmetric clock lines. The magic wavelength is where the line is narrowest and most symmetric.

This gave a rough first value of 759.35(0.02) nm (~20 MHz uncertainty in frequency). More precise measurements followed in Barber 2008 and Lemke 2009.

## MIS Technique

A magnetic field $B \parallel \hat{z}$ (quantization axis = lattice propagation axis) mixes:

$$|3P_0^*\rangle \approx |3P_0\rangle + \varepsilon |3P_1, m_J=0\rangle$$

The mixing coefficient $\varepsilon \propto B$, so the induced transition rate scales as $\Gamma_\text{induced} \propto B^2$. At $B = 0.1$ mT, the induced linewidth is ~1 mHz, enabling spectroscopy with reasonable Rabi times while maintaining a narrow linewidth.

## Quadratic Zeeman Systematics

The applied field introduces a quadratic Zeeman shift $\delta\nu = -\beta_\text{QZ} B^2$. The measured coefficient $\beta_\text{QZ} = 6.6(0.4)$ MHz/T² means at $B=1$ G ($10^{-4}$ T), the shift is $\delta\nu = -66$ nHz, negligible at the $10^{-16}$ level of precision at that time but requiring extrapolation to $B \to 0$ for higher precision.

## Significance

This paper proved the Yb lattice clock concept with a practical (most-abundant) isotope. However, subsequent work shifted to ¹⁷¹Yb (I=1/2) which does not require MIS and benefits from simpler hyperfine structure and Pauli suppression of s-wave density shifts.

## Related pages

- [[magnetic-field-induced-spectroscopy]]
- [[magic-wavelength]]
- [[optical-lattice-clock]]
- [[yb-atomic-structure]]
- [[zeeman-shift]]
