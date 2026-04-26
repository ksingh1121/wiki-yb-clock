# Safronova et al. PRL 2018

**Summary**: Theoretical proposal for a dual-clock-transition scheme in ¹⁷¹Yb using the 3P₀→4f¹³5d6s²(J=2) transition at ~1695 nm as a highly sensitive probe for fine-structure constant variation, with K_α ≈ −15.

**Sources**: M S Safronova et al. PRL 2018.pdf

**Last updated**: 2026-04-26

---

## Reference

M. S. Safronova, S. G. Porsev, C. Sanner, and J. Ye, "Two Clock Transitions in Neutral Yb for the Ultimate Search for Variation of the Fine-Structure Constant," *Phys. Rev. Lett.* **120**, 173001 (2018).

## Context

The sensitivity of an optical clock to variation of the fine-structure constant $\alpha$ is parameterized by $K_\alpha = \partial \ln\nu / \partial \ln\alpha$. Most optical clock transitions have $|K_\alpha| < 1$. The 4f-open-shell configuration in certain heavy atoms can yield $|K_\alpha| \gg 1$, dramatically enhancing sensitivity to $\alpha$-variation. This paper identified a transition in neutral Yb — the 3P₀→J=2 at 1695 nm — as having $K_\alpha \approx -15$, one of the largest known for any neutral atom clock candidate.

## Key Physics

The J=2 upper state of the proposed transition has configuration 4f¹³5d6s²: the normally filled 4f subshell (4f¹⁴) has one hole. 4f electrons are highly relativistic, and the 4f-hole state has strong coupling between relativistic and non-relativistic components. This gives an unusually large relativistic correction to the energy level, and therefore a large sensitivity to $\alpha$.

## Calculated Transition Properties

| Property | Value | Notes |
|----------|-------|-------|
| Frequency | ~177 THz | ~1695 nm wavelength |
| $K_\alpha$ | $\approx -15$ | Very high; from relativistic CIPT calculation |
| $K_\mu$ | Small | Proton mass sensitivity via hyperfine is indirect |
| Sensitivity ratio vs. 1S₀→3P₀ | ~25× | In terms of $|K_\alpha|$ difference |

(source: M S Safronova et al. PRL 2018.pdf)

## Dual-Clock Scheme

The proposal is to simultaneously interrogate two transitions in the **same Yb atom** (or same ensemble):
1. **Primary clock**: 1S₀→3P₀ at 578 nm (well-characterized, $K_\alpha \approx -0.6$)
2. **Secondary clock**: 3P₀→J=2 at 1695 nm ($K_\alpha \approx -15$)

Since both measurements are made on the same atoms in the same environment, many systematic uncertainties cancel. The frequency ratio:

$$R = \frac{\nu(3P_0 \to J=2)}{\nu(1S_0 \to 3P_0)}$$

is the observable. Any variation in $\alpha$ would change $R$ by:

$$\frac{\dot{R}}{R} = (K_\alpha^{(2)} - K_\alpha^{(1)}) \cdot \frac{\dot{\alpha}}{\alpha} \approx (-15 - (-0.6)) \cdot \frac{\dot{\alpha}}{\alpha} = -14.4 \cdot \frac{\dot{\alpha}}{\alpha}$$

This ~14× enhancement means that a $10^{-17}$/yr limit on $\dot{\alpha}/\alpha$ from standard single-clock comparisons translates to a $\sim 10^{-18}$/yr sensitivity with this dual-transition approach.

## Theoretical Methods

The calculations used a combination of:
- Coupled cluster method for valence electrons
- Configuration interaction plus perturbation theory (CIPT) for core contributions
- Breit interaction and quantum electrodynamics corrections

The 4f-hole state is particularly challenging computationally because correlation between the 4f hole and valence electrons is strong. The uncertainty in $K_\alpha$ is estimated at ~10–20%.

## Practical Challenges

1. **Magic wavelength for the secondary transition**: The 3P₀→J=2 transition must also be Lamb-Dicke confined. The magic wavelength for this transition must be found — it will differ from the 759 nm primary clock magic wavelength.
2. **Probe laser at 1695 nm**: Telecom-band laser technology is mature, but sub-Hz linewidth requires a ULE cavity system at 1695 nm.
3. **BBR shift of the J=2 state**: The differential static polarizability for the 3P₀→J=2 transition must be characterized.
4. **Lifetime**: The J=2 state lifetime determines the interrogation time limit. If the lifetime is very long (as expected for this type of transition), the lifetime is not a constraint.

## Status

As of this wiki's source base (up to Bothwell 2025), this proposal has not yet been experimentally demonstrated. It represents a future direction for Yb lattice clocks as a platform for fundamental physics beyond precision timekeeping.

## Related pages

- [[dual-clock-transitions-yb]]
- [[fundamental-constants-variation]]
- [[yb-atomic-structure]]
- [[clock-transition-yb]]
- [[dzuba-pra-2018]]
