# Magnetic-Field-Induced Spectroscopy (MIS)

**Summary**: A technique that uses a static magnetic field to open the strictly forbidden 1S₀→3P₀ clock transition in bosonic (even) Yb isotopes by mixing the 3P₁ state into 3P₀, enabling lattice clock operation with ¹⁷⁴Yb.

**Sources**: Z W Barber et al. PRL 2005.pdf (actually PRL 2006), A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Motivation

In even isotopes of Yb (¹⁷⁴Yb, ¹⁷²Yb, etc.), the 1S₀→3P₀ transition is **strictly forbidden**: the electric-dipole selection rules ΔJ=0 (J=0→J=0 forbidden) and ΔS=0 both apply rigorously because there is no nuclear spin (I=0) to mix states. The transition rate is identically zero under any realistic perturbation-free conditions.

A static magnetic field $B$ along the quantization axis mixes the $3P_1(m_J=0)$ state (which has a finite E1 matrix element to 1S₀) into the 3P₀ state via the Zeeman interaction. This induces a small admixture of 3P₁ character in 3P₀, giving the previously forbidden transition a finite electric-dipole matrix element.

## Physics of State Mixing

The mixed clock state to first order in $B$ is:

$$|3P_0^*\rangle = |3P_0\rangle + \varepsilon |3P_1, m_J=0\rangle$$

where the mixing coefficient $\varepsilon \propto B \cdot \langle 3P_1, m_J=0 | H_\text{Zeeman} | 3P_0 \rangle / \Delta E(3P_1 - 3P_0)$. The induced linewidth of the clock transition scales as $\Gamma_\text{induced} \propto B^2 \Gamma_{3P_1}$.

For $B \sim 0.1$ mT (1 G), the induced linewidth is of order $\sim 1$ mHz, which is sufficient for spectroscopy with sub-second Rabi pulses while remaining narrow enough to give a high $Q$-factor. (source: Z W Barber et al. PRL 2005.pdf / 2006)

## Barber 2006 Experiment (First Yb Lattice Clock)

The Barber 2006 paper (filename Z W Barber et al. PRL 2005.pdf) reported the first optical lattice clock using ¹⁷⁴Yb with MIS. Key parameters:

- **Applied field**: $B \approx 0.1$ mT along the lattice/quantization axis
- **Magic wavelength**: ~759.35(0.02) nm (first measurement)
- **Clock transition**: ¹⁷⁴Yb 1S₀→3P₀ opened via MIS
- **Linewidth achieved**: sub-Hz Fourier-limited lines with ms interrogation
- **Systematics**: quadratic Zeeman shift, lattice light shift, BBR shift

(source: Z W Barber et al. PRL 2005.pdf)

## Quadratic Zeeman Shift

The applied magnetic field introduces a quadratic Zeeman shift (in addition to the first-order shift that averages to zero for $m_F = 0$ states in bosonic isotopes). For ¹⁷⁴Yb (J=0 clock states), the 3P₀ state acquires a quadratic shift from the mixed 3P₁ character:

$$\delta\nu_\text{QZ} = -\beta_\text{QZ} B^2$$

where $\beta_\text{QZ} = 6.6(0.4) \text{ MHz/T}^2$ for ¹⁷⁴Yb (Barber 2006). To evaluate this shift, $B$ must be accurately known or measured. The shift at $B = 0.1$ mT is:

$$\delta\nu_\text{QZ} = -6.6 \times (10^{-4})^2 \text{ Hz} = -66 \text{ nHz}$$

which is negligible at 10⁻¹⁶ level but must be tracked at higher precision. The field must be extrapolated to $B \to 0$ to remove it. (source: Z W Barber et al. PRL 2005.pdf)

## Advantages and Disadvantages of MIS vs. Odd Isotopes

| Aspect | MIS (¹⁷⁴Yb, bosonic) | Odd isotopes (¹⁷¹Yb, fermionic) |
|--------|----------------------|--------------------------------|
| Clock transition | Induced by $B$ | Hyperfine-induced (natural) |
| Nuclear spin | I = 0 | I = 1/2 |
| Zeeman structure | No first-order Zeeman | Two $m_F=\pm1/2$ lines |
| Density shift | Bosonic (s-wave suppressed) | Fermionic (p-wave) |
| Hyperfine complexity | None | Simple (I=1/2) |
| Systematic: QZ shift | Present (must characterize B) | Present but small |
| State preparation | No optical pumping needed | Requires spin polarization |

The simplicity of no hyperfine structure in ¹⁷⁴Yb is partially offset by the need for an accurate B-field measurement and the $B$-dependent systematic. Most state-of-the-art Yb lattice clocks now use ¹⁷¹Yb for its simpler I=1/2 structure.

## Related pages

- [[clock-transition-yb]]
- [[yb-atomic-structure]]
- [[zeeman-shift]]
- [[optical-lattice-clock]]
- [[systematic-uncertainty-budget]]
- [[barber-prl-2006]]
