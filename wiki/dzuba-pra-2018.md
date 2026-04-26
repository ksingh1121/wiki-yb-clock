# Dzuba et al. PRA 2018

**Summary**: Ab initio calculations of transition properties for multiple Yb clock transition candidates, including the 1S₀→3P₂ M2 transition and the 4f¹³5d6s²(J=2) state, using CIPT methods with Breit interaction and QED corrections.

**Sources**: V Dzuba et al. PRA 2018.pdf

**Last updated**: 2026-04-26

---

## Reference

V. A. Dzuba, V. V. Flambaum, and S. G. Porsev, "Proposal to Search for New Physics with Atoms Having a Partially Filled Inner Shell," *Phys. Rev. A* **98**, 032519 (2018).

*Note*: The exact PRA article number (032519) should be verified against the source PDF.

## Context

This paper provides theoretical support for the experimental proposals in Safronova 2018 and surveys additional transition candidates in Yb and related systems. The focus is on transitions with large sensitivity to variation of fundamental constants, particularly involving states with open inner shells (4f¹³ configurations in Yb). The calculations use CIPT (Configuration Interaction plus Perturbation Theory) with relativistic corrections.

## Key Transitions Calculated

### 1S₀ → 3P₂ (at ~507 nm)

The 3P₂ state lies at 19710 cm⁻¹ above the ground state. The 1S₀(J=0)→3P₂(J=2) transition is magnetic quadrupole (M2) and has different sensitivity to $\alpha$ variation than the 1S₀→3P₀ transition. Properties:
- Lifetime: ~15 cs for even isotopes (longer for odd due to hyperfine contributions)
- J=2: has tensor, vector, and scalar polarizability components
- $K_\alpha$: calculated to differ from the 1S₀→3P₀ value, enabling a complementary probe

### 4f¹³6s²5d(J=2) State (at ~23188 cm⁻¹ above 1S₀)

This is the same state proposed in Safronova 2018 for the dual-clock scheme. Dzuba 2018 provides:
- **Energy**: ~23188 cm⁻¹ (agrees with Safronova; the 3P₀→J=2 transition at ~5900 cm⁻¹ ~1695 nm)
- **Lifetime**: Long-lived due to highly forbidden character; specific value depends on M2/E3 matrix elements to ground state
- **$K_\alpha$**: Large negative value ($\approx -15$), consistent with Safronova 2018
- **Polarizability**: Calculated static polarizability for use in BBR shift estimates

## Computational Methods

The CIPT method used here combines:
1. **Configuration Interaction (CI)**: Treats electron correlation among valence electrons
2. **Many-Body Perturbation Theory (MBPT)**: Adds core-valence correlations
3. **Breit interaction**: Magnetic and retardation corrections to the Coulomb Hamiltonian, important for heavy elements
4. **QED corrections**: Self-energy and vacuum polarization, estimated via model-potential approach

For 4f-open-shell states, the CI space must include 4f excitations explicitly, making the calculation substantially more demanding than for 4f¹⁴ states. Dzuba 2018 validates their approach against experimentally known energy levels.

## Level Structure and Energy Tables

The paper provides calculated energy levels for:
- The 4f¹³ series of levels (4f¹³5d6s²J=2 and others)
- Comparison of calculated vs. experimental energies (where available from spectroscopic measurements) to validate accuracy

For the J=2 state, the dominant configuration is 4f¹³5d6s² but there is mixing with other nearby states. The CIPT calculation gives the mixing coefficients.

## Sensitivity to Fundamental Constants

Dzuba 2018 calculates $K_\alpha$ and $K_\mu$ for multiple Yb transitions, finding:

| Transition | $K_\alpha$ |
|-----------|------------|
| 1S₀→3P₀ | $\approx -0.6$ |
| 1S₀→3P₂ | Different sign/magnitude |
| 3P₀→J=2 (1695 nm) | $\approx -15$ |

The large negative $K_\alpha$ for the 4f-hole state makes the dual-clock scheme (Safronova 2018) a compelling proposal.

## Relationship to Safronova 2018

Dzuba 2018 and Safronova 2018 are closely related companion papers that appeared in 2018 addressing the same proposal from complementary angles. Dzuba 2018 provides the detailed atomic structure calculations supporting the energy levels, lifetimes, and polarizabilities quoted in Safronova 2018.

## Related pages

- [[dual-clock-transitions-yb]]
- [[fundamental-constants-variation]]
- [[yb-atomic-structure]]
- [[safronova-prl-2018]]
