# Dual Clock Transitions in Yb

**Summary**: The proposal and theoretical characterization of a second clock transition in ¹⁷¹Yb at ~1695 nm connecting 3P₀ to the 4f¹³5d6s²(J=2) state, which has exceptional sensitivity to fine-structure constant variation due to its open 4f-shell configuration.

**Sources**: M S Safronova et al. PRL 2018.pdf, V Dzuba et al. PRA 2018.pdf

**Last updated**: 2026-04-26

---

## The Second Clock Transition

The standard Yb clock uses the 1S₀→3P₀ transition at 578 nm. Safronova et al. (2018) proposed operating a second clock transition from the **3P₀ clock state** to the 4f¹³5d6s²(J=2) level at approximately **1695 nm** (~177 THz).

This transition has several unusual properties:

- The upper state has an **open 4f shell** (configuration 4f¹³), unlike all other Yb clock candidates which have filled 4f shells (4f¹⁴).
- The 4f-open-shell state has very large relativistic corrections, giving it an exceptionally high **sensitivity to fine-structure constant variation**: $K_\alpha \approx -15$.
- The transition lies in the near-infrared at 1695 nm, accessible to standard telecom-band laser technology.

(source: M S Safronova et al. PRL 2018.pdf)

## Fine-Structure Constant Sensitivity

The key figure of merit for probing $\alpha$-variation is the enhancement factor $K_\alpha$:

$$\frac{\delta\nu}{\nu} = K_\alpha \cdot \frac{\delta\alpha}{\alpha}$$

| Transition | $K_\alpha$ |
|-----------|------------|
| 1S₀ → 3P₀ (578 nm) | $\approx -0.6$ |
| 3P₀ → J=2 (1695 nm) | $\approx -15$ |
| **Ratio difference** | **~25×** |

By comparing the two transitions in the same Yb atom simultaneously, the combination:

$$R = \frac{\nu_{3P_0 \to J=2}}{\nu_{1S_0 \to 3P_0}} \propto \alpha^{K_\alpha^{(2)} - K_\alpha^{(1)}} \approx \alpha^{-14}$$

would give a constraint on $\dot{\alpha}/\alpha$ approximately 14× better (per unit measurement uncertainty) than comparing either transition to an external reference. (source: M S Safronova et al. PRL 2018.pdf)

## Properties of the J=2 State

The 4f¹³5d6s²(J=2) state at ~23188 cm⁻¹ (1695 nm above 3P₀) has:
- Finite lifetime due to M2 and E3 decay channels to the ground state and 3P₀
- J=2 angular momentum, allowing it to be probed via the 3P₀→J=2 transition using M1 or E2 amplitude
- Sensitivity to BBR: the static polarizability of the J=2 state differs from 3P₀, so the BBR shift on the 3P₀→J=2 transition must be evaluated
- Sensitivity to lattice light shifts: a magic wavelength for the 3P₀→J=2 transition must be identified

(source: V Dzuba et al. PRA 2018.pdf, M S Safronova et al. PRL 2018.pdf)

## Dzuba 2018 Calculations

Dzuba et al. (2018) performed configuration interaction plus perturbation theory (CIPT) calculations of transition properties in Yb. Their work covered:

1. **1S₀→3P₂ transition** at 507 nm (M2): another candidate clock transition with different $K_\alpha$
2. **4f¹³5d6s²(J=2) state** properties: energy, lifetime, polarizability, $K_\alpha$
3. Comparison of multiple Yb transitions as probes of $\alpha$-variation

The key result is that the 4f-open-shell J=2 state has $K_\alpha = -15$ — the largest known value for a state accessible from the 3P₀ metastable level in Yb or any alkaline-earth-like atom. (source: V Dzuba et al. PRA 2018.pdf)

## Experimental Status

As of the sources in this wiki (up to Bothwell 2025), the 3P₀→J=2 transition has not yet been demonstrated experimentally in an optical lattice clock. The Safronova 2018 and Dzuba 2018 papers are theoretical proposals. The practical challenges include:

1. Finding a magic wavelength for the two-state system (1S₀, 3P₀, and J=2 must all be compatible)
2. The J=2 state may require a different lattice depth or wavelength than the standard clock operation
3. The 1695 nm clock laser must achieve sub-Hz linewidth at telecom wavelengths

## Related pages

- [[yb-atomic-structure]]
- [[fundamental-constants-variation]]
- [[clock-transition-yb]]
- [[optical-lattice-clock]]
- [[magic-wavelength]]
