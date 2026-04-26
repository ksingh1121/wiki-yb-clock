# Gao et al. Scientific Reports 2018

**Summary**: First ¹⁷¹Yb lattice clock evaluation at ECNU (China), achieving 1.7×10⁻¹⁶ total systematic uncertainty using a synchronous comparison technique to precisely measure the density shift and magic frequency.

**Sources**: Q Gao et al. SR 2018.pdf

**Last updated**: 2026-04-26

---

## Reference

Q. Gao, M. Zhou, C. Han, S. Li, S. Zhang, Y. Yao, B. Li, H. Qiao, D. Ai, G. Lou, M. Zhang, Y. Jiang, Z. Bi, L. Ma, and X. Xu, "Systematic evaluation of a ¹⁷¹Yb optical clock by synchronous comparison between two lattice systems," *Scientific Reports* **8**, 8022 (2018).

## Context

ECNU (East China Normal University) built an independent ¹⁷¹Yb optical lattice clock, making it one of the few non-NIST and non-NMIJ Yb lattice clock groups. The novel feature of this work is the use of a **synchronous comparison** between two lattice clock systems sharing the same clock laser. This technique cancels the Dick effect noise and enables precise systematic evaluation with shorter averaging times.

## Key Results

### Systematic Uncertainty
$$\sigma_\text{sys} = 1.7\times10^{-16}$$

| Effect | Uncertainty |
|--------|-------------|
| BBR shift | Significant (room temperature, no shield) |
| Lattice light shift (first-order) | Significant |
| Density/collision shift | $4.9\times10^{-17}$ |
| Second-order Zeeman | Small |
| **Total** | **$1.7\times10^{-16}$** |

### Magic Frequency
$$\nu_\text{magic}(^{171}\text{Yb}) = 394,798,381.5(9.3) \text{ MHz}$$

This value is ~112 MHz above the Lemke 2009 value (394,798,329 MHz) and ~115 MHz above the Brown 2017 $\nu_\text{zero}$. The discrepancy (given the 10 MHz Lemke uncertainty vs. 9.3 MHz ECNU uncertainty) is marginal but suggests possible systematic errors in one or both magic frequency measurements. The ECNU value at ~9 MHz precision is consistent with Lemke 2009 at 10 MHz precision within ~1σ when comparing combined uncertainties.

### Density Shift
$$\delta\nu_\text{coll} = -0.570(25) \text{ Hz}$$

This is the most precise density shift measurement reported for Yb at that time, enabled by the synchronous comparison technique.

## Synchronous Comparison Technique

Two Yb lattice clock systems (labeled clock 1 and clock 2) are loaded from the same MOT and interrogated simultaneously using the same clock laser. Because they share the laser:

- **Dick effect noise cancels** in the frequency difference (it is common-mode)
- The differential instability is limited by **quantum projection noise** only
- Differential systematics (density, trap depth, B-field) can be measured precisely

This technique is also used (with a single apparatus, two ensembles) in the Bothwell 2025 NIST work.

The measured differential instability was $\sim 2\times10^{-17}/\sqrt{\tau}$, enabling evaluation of the $\sim 0.5$ Hz density shift with 25 mHz precision in practical measurement times.

## Density Shift Method

The density shift was measured by preparing clock 1 and clock 2 with different atom numbers (different trap loading conditions) and measuring their frequency difference. The difference $\nu_1 - \nu_2 = -0.570(25)$ Hz was attributed entirely to the differential density shift.

## SFG Clock Laser

Like NMIJ, ECNU used a sum-frequency generation approach to generate 578 nm light:
- 1030 nm Yb:fiber laser + 1319 nm Nd:YAG → 578 nm via PPLN crystal
- Locked to a ULE Fabry-Pérot reference cavity

This confirms the practicality of SFG as an alternative to dye lasers for the Yb clock laser.

## Significance

This paper demonstrated that the Yb lattice clock is reproducible across different laboratories (NIST, NMIJ, ECNU) and introduced the synchronous comparison as an evaluation method. The ECNU group's independent evaluation provides a cross-check on NIST's systematic assessments.

## Related pages

- [[optical-lattice-clock]]
- [[density-shift]]
- [[magic-wavelength]]
- [[clock-stability]]
- [[systematic-uncertainty-budget]]
