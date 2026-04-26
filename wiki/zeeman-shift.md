# Zeeman Shift

**Summary**: The shift of the clock transition frequency due to static and oscillating magnetic fields, including first-order (linear) and second-order (quadratic) contributions for ¹⁷¹Yb.

**Sources**: N D Lemke et al. PRL 2009.pdf, Z W Barber et al. PRL 2005.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## First-Order Zeeman Shift in ¹⁷¹Yb

For ¹⁷¹Yb (I=1/2), the 1S₀ and 3P₀ clock states both have $F=1/2$. Each has two magnetic sub-levels: $m_F = +1/2$ and $m_F = -1/2$. The first-order Zeeman shift is:

$$\delta\nu_{m_F} = m_F \cdot g_F \cdot \mu_B \cdot B / h$$

where $g_F$ is the hyperfine $g$-factor. For the clock transition 1S₀→3P₀, the differential $g$-factor $\Delta g_F = g_F(3P_0) - g_F(1S_0)$ gives the net splitting:

$$\delta\nu_{+1/2} - \delta\nu_{-1/2} = \Delta g_F \cdot \mu_B \cdot B / h \approx 210 \text{ Hz/G}$$

(source: N D Lemke et al. PRL 2009.pdf)

So the two clock transitions ($m_F = +1/2 \to +1/2$ and $m_F = -1/2 \to -1/2$) are split by ~210 Hz at 1 G (1 mT). In practice both transitions are measured and their average taken to cancel the first-order Zeeman shift:

$$\nu_\text{clock} = \frac{\nu(m_F=+1/2) + \nu(m_F=-1/2)}{2}$$

This averaging is a key systematic control technique in ¹⁷¹Yb clocks. (source: N D Lemke et al. PRL 2009.pdf)

## Second-Order (Quadratic) Zeeman Shift

Beyond the first-order effect, the second-order Zeeman interaction shifts the average of the two $m_F$ lines by:

$$\delta\nu_\text{QZ} = -\beta_\text{QZ} B^2$$

For the ¹⁷¹Yb clock transition, $\beta_\text{QZ}$ is small because both clock states have $J=0$ and the shift arises only from the nuclear $g$-factor and virtual state mixing. The coefficient is of order $\sim 10^{-3}$ Hz/G², making the quadratic Zeeman shift below $10^{-16}$ for typical bias fields of $\sim 1-10$ mT.

**Important**: For ¹⁷⁴Yb with [[magnetic-field-induced-spectroscopy]], the effective quadratic Zeeman coefficient is much larger — $\beta_\text{QZ} = 6.6(0.4)$ MHz/T² — because the applied field mixes in the 3P₁ state. See [[magnetic-field-induced-spectroscopy]] for details.

## Vector Light Shift as an Effective Zeeman Shift

The vector component of the lattice light shift acts like a fictitious magnetic field and can produce an effective first-order Zeeman shift. For ¹⁷¹Yb (J=0 clock states), this arises from the hyperfine-induced polarizability. The vector light shift for $m_F = \pm 1/2$ states is:

$$\delta\nu_\text{vector} = \pm \frac{1}{2} \tilde{\alpha}_\text{vector} \cdot A \cdot U$$

where $A$ is the degree of circular polarization of the lattice. This can be suppressed to below $10^{-18}$ by:
1. Linear polarization ($A \approx 0$)
2. Lattice propagation along the quantization axis
3. Averaging over $m_F = \pm 1/2$ transitions

(source: N D Lemke et al. PRL 2009.pdf)

## Magnetic Field Measurement

In Lemke 2009, the bias magnetic field is determined from the measured splitting between the $m_F = \pm 1/2$ clock transitions:

$$B = \frac{\nu(m_F=+1/2) - \nu(m_F=-1/2)}{210 \text{ Hz/G}}$$

Typical fields: 0.1–1 mT, determined to $\sim 1\%$ accuracy from the frequency splitting. The resulting quadratic Zeeman uncertainty is well below $10^{-17}$. (source: N D Lemke et al. PRL 2009.pdf)

## Uncertainty in Lemke 2009 Budget

In the Lemke 2009 systematic budget, the Zeeman shift contributes:
- Second-order Zeeman: $< 10^{-17}$ (negligible)
- Vector light shift: $3.4\times10^{-17}$ (residual after $m_F$ averaging and polarization control)

(source: N D Lemke et al. PRL 2009.pdf)

## Related pages

- [[clock-transition-yb]]
- [[magnetic-field-induced-spectroscopy]]
- [[lattice-light-shift]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
