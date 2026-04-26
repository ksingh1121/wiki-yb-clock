# Clock Stability

**Summary**: The short-term and long-term frequency stability of optical lattice clocks, determined by quantum projection noise, Dick effect aliasing, laser linewidth, and averaging time.

**Sources**: N D Lemke et al. PRL 2009.pdf, Q Gao et al. SR 2018.pdf, T Bothwell et al. PRL 2025.pdf, A Ludlow et al. RMP 2015.pdf, Takamoto et al. nature 2005.pdf

**Last updated**: 2026-04-26

---

## Allan Deviation

Frequency instability is quantified by the overlapping Allan deviation $\sigma_y(\tau)$, where $\tau$ is the averaging time. The quantum-projection-noise (QPN) limited value for a Ramsey/Rabi-interrogated lattice clock is:

$$\sigma_y(\tau) \approx \frac{1}{2\pi\nu_0} \sqrt{\frac{T_c}{N \cdot T_\text{int} \cdot \tau}}$$

where:
- $\nu_0$ is the clock frequency (~518 THz for Yb)
- $N$ is the atom number
- $T_\text{int}$ is the interrogation (Rabi/Ramsey) time
- $T_c$ is the cycle time
- $\tau$ is the total averaging time

For typical parameters $N=10^4$, $T_\text{int}=0.5$ s, $T_c=1$ s, the QPN limit is $\sigma_y \sim 3\times10^{-17}/\sqrt{\tau/\text{s}}$. (source: A Ludlow et al. RMP 2015.pdf)

## Dick Effect

In pulsed interrogation, the clock laser frequency noise is sampled only during the interrogation window ($T_\text{int} < T_c$). Noise components at harmonics of $1/T_c$ are aliased into the measurement band, degrading stability beyond the QPN limit. This is the **Dick effect** (or aliasing noise).

The Dick-effect-limited Allan deviation scales as:

$$\sigma_y^\text{Dick}(\tau) \propto \frac{S_y^{1/2}(1/T_c)}{\sqrt{\tau}}$$

where $S_y(f)$ is the laser fractional frequency noise power spectral density. For a typical ultrastable cavity laser with $S_y \sim 10^{-31} (1\text{ Hz}/f)$ (flicker floor), the Dick-limited stability at cycle time $T_c \sim 1$ s is $\sim 10^{-16}/\sqrt{\tau}$. (source: A Ludlow et al. RMP 2015.pdf)

The Dick effect is the dominant stability limitation in most current lattice clocks and motivates:
1. **Long interrogation times** ($T_\text{int}/T_c$ close to 1)
2. **Synchronous comparison** between two clocks (Dick noise cancels if they share the same laser)
3. **Optical frequency combs** linking to ultra-stable references

## Synchronous Comparison (Gao 2018)

Gao 2018 (ECNU) implemented a dual-lattice-clock comparison where two independent ensembles are loaded from the same MOT and interrogated simultaneously by the same clock laser. In this configuration, the Dick effect noise is **common-mode** and cancels in the frequency difference. The resulting differential stability is limited by QPN:

$$\sigma_y^\text{sync}(\tau) \approx \frac{1}{\pi\nu_0} \sqrt{\frac{T_c}{N \cdot T_\text{int} \cdot \tau}}$$

(factor of $\sqrt{2}$ worse than single clock because two independent measurements are combined). This technique gave a measured instability of $\sim 2\times10^{-17}/\sqrt{\tau}$, enabling precise evaluation of density shifts and other differential systematics without long averaging. (source: Q Gao et al. SR 2018.pdf)

## Dual-Ensemble Technique (Bothwell 2025)

Bothwell 2025 (NIST) used a **dual-ensemble** apparatus where two spatially separated atomic clouds are prepared and interrogated within the same vacuum apparatus. The two ensembles experience the same clock laser, enabling synchronous comparison with excellent common-mode rejection. This allowed evaluation of the lattice light shifts (multipolarizability and hyperpolarizability) at the $10^{-19}$ level by comparing ensembles at different trap depths. (source: T Bothwell et al. PRL 2025.pdf)

## Lemke 2009 Stability

The Lemke 2009 evaluation at NIST reported:
- Systematic uncertainty: $3.4\times10^{-16}$
- Fractional instability: consistent with Dick-effect-limited operation at that era

The frequency was determined to $1.3\times10^{-15}$ fractional uncertainty (dominated by systematics). (source: N D Lemke et al. PRL 2009.pdf)

## Takamoto 2005 First Demonstration (Sr)

The first OLC stability measurement (Takamoto 2005) achieved $\sigma_y(\tau) \approx 1.5\times10^{-15}/\sqrt{\tau}$, limited by Dick effect and modest atom numbers. The frequency was measured to $\pm 15$ Hz at 429 THz, demonstrating the concept. (source: Takamoto et al. nature 2005.pdf)

## Factors Limiting Stability

| Noise source | Scaling | Mitigation |
|-------------|---------|------------|
| Quantum projection noise | $1/\sqrt{N T_\text{int} \tau}$ | More atoms, longer interrogation |
| Dick effect | $\propto S_y^{1/2}/\sqrt{\tau}$ | Better cavity, synchronous operation |
| Laser frequency noise during interrogation | $\propto T_\text{int}^{3/2}$ | Better cavity, shorter $T_\text{int}$ |
| Servo noise (gain, slope) | Apparatus-dependent | High-SNR detection |
| Photon shot noise (detection) | $\propto 1/\sqrt{N}$ | Many detected photons |

## Related pages

- [[optical-lattice-clock]]
- [[systematic-uncertainty-budget]]
- [[clock-transition-yb]]
- [[density-shift]]
