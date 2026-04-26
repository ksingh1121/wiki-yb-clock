# Fundamental Constants Variation

**Summary**: The use of optical atomic clocks to search for time-variation of fundamental constants, particularly the fine-structure constant α and the proton-to-electron mass ratio μ, through frequency ratio measurements.

**Sources**: M S Safronova et al. PRL 2018.pdf, V Dzuba et al. PRA 2018.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Motivation

Several theories beyond the Standard Model predict slow temporal or spatial variation of dimensionless fundamental constants such as:

- The fine-structure constant: $\alpha = e^2 / (4\pi\epsilon_0 \hbar c) \approx 1/137$
- The proton-to-electron mass ratio: $\mu = m_p / m_e \approx 1836$

Optical atomic clocks are among the most sensitive probes of such variations because:
1. Their transition frequencies depend on $\alpha$ through relativistic corrections, and on $\mu$ through proton mass contributions to hyperfine structure.
2. Fractional frequency ratios between two different clock transitions can be measured with uncertainties below $10^{-17}$.
3. A time-varying fundamental constant would show up as a drift in the frequency ratio between two clocks with different sensitivities.

## Sensitivity Coefficients

For a clock transition at frequency $\nu$, the sensitivity to variation in $\alpha$ is parameterized by:

$$K_\alpha = \frac{\partial \ln \nu}{\partial \ln \alpha} \bigg|_\text{const }\mu$$

If $\alpha$ varies at rate $\dot{\alpha}/\alpha$, the clock frequency drifts as $\dot{\nu}/\nu = K_\alpha \cdot \dot{\alpha}/\alpha$. By comparing two clocks with different $K_\alpha$ values, one can constrain $\dot{\alpha}/\alpha$.

Similarly, the sensitivity to $\mu$ variation is given by:

$$K_\mu = \frac{\partial \ln \nu}{\partial \ln \mu}$$

## Yb as a Platform for Constants Variation

Yb is particularly attractive because it offers **two clock transitions** with very different sensitivity coefficients, enabling an in-situ differential measurement:

| Transition | Frequency | $K_\alpha$ | Sensitivity |
|-----------|-----------|------------|-------------|
| 1S₀ → 3P₀ | ~518 THz (578 nm) | $K_\alpha \approx -0.6$ | Moderate, well-studied |
| 3P₀ → 4f¹³5d6s²(J=2) | ~177 THz (~1695 nm) | $K_\alpha \approx -15$ | Very high, factor ~25 larger |

The second transition's large $K_\alpha = -15$ arises from the 4f-hole configuration of the J=2 state, which has strong relativistic corrections. See [[dual-clock-transitions-yb]]. (source: M S Safronova et al. PRL 2018.pdf)

## Frequency Ratio Approach

The key observable is the ratio of two transition frequencies within the same atom or between two different atomic species. If both transitions are measured simultaneously in the same apparatus, systematic errors largely cancel (common-mode rejection). The ratio:

$$R = \frac{\nu_1}{\nu_2}$$

is predicted by the Standard Model to be a constant. Any observed drift $\dot{R}/R \neq 0$ would be evidence for new physics.

Combining a sensitive clock (high $|K_\alpha|$) with a well-understood reference (low $|K_\alpha|$) maximizes the sensitivity to $\dot{\alpha}$.

## Dzuba 2018 Transitions

Dzuba et al. (2018) calculated the sensitivity coefficients for multiple Yb transitions including:

- 1S₀ → 3P₀ (standard clock transition): moderate $K_\alpha$
- 1S₀ → 3P₂ at 507/431 nm: different $K_\alpha$ due to M2 character
- 3P₀ → 4f¹³5d6s²(J=2) at ~1695 nm: $K_\alpha = -15$ (very high, from 4f-hole relativistic effects)

The large negative $K_\alpha$ of the 4f-open-shell state means its frequency is very sensitive to changes in $\alpha$. A fractional change $\delta\alpha/\alpha = 10^{-18}$ would shift this transition by $\Delta\nu/\nu = K_\alpha \cdot \delta\alpha/\alpha = 15\times10^{-18}$, at the edge of measurability with a $10^{-18}$ clock. (source: V Dzuba et al. PRA 2018.pdf)

## Current Bounds from Clock Comparisons

State-of-the-art bounds on $\dot{\alpha}/\alpha$ from optical clock comparisons:

$$\dot{\alpha}/\alpha < 10^{-17} \text{ yr}^{-1}$$

obtained by comparing Yb/Sr/Al⁺ and other species over multi-year baselines. The Yb dual-transition proposal (Safronova 2018) would improve sensitivity by leveraging the large $K_\alpha$ difference within a single atom. (source: M S Safronova et al. PRL 2018.pdf)

## Related pages

- [[dual-clock-transitions-yb]]
- [[yb-atomic-structure]]
- [[clock-transition-yb]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
