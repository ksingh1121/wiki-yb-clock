# BBR Shield

**Summary**: An in-vacuum copper thermal enclosure developed at NIST to reduce the blackbody radiation shift uncertainty of the ¹⁷¹Yb lattice clock to 10⁻¹⁸ by providing a cold, uniform thermal environment around the atoms.

**Sources**: K Beloy et al. PRL 2014.pdf

**Last updated**: 2026-04-26

---

## Motivation

The [[blackbody-radiation-shift]] at room temperature (~300 K) is a fractional frequency shift of $-2.454\times10^{-16}$ for the ¹⁷¹Yb clock transition. After the Sherman 2012 measurement of $\Delta\alpha(0)$ reduced the atomic parameter uncertainty to ppm level, the remaining BBR uncertainty was dominated by the temperature uncertainty of the apparatus thermal environment. At 300 K, a 1 K temperature uncertainty contributes $\sim 3.3\times10^{-18}$ fractional frequency uncertainty (since the shift scales as $T^4$).

To reduce the BBR uncertainty below $10^{-18}$, NIST implemented an **in-vacuum copper shield** operating at room temperature but with greatly reduced and well-characterized thermal variation across the atomic trapping volume. (source: K Beloy et al. PRL 2014.pdf)

## Shield Design

The Beloy 2014 shield is a **closed copper enclosure** placed in the vacuum chamber surrounding the atomic trapping region. Key design features:

- **Material**: Copper, chosen for high thermal conductivity to minimize temperature gradients across the shield walls
- **Geometry**: Closed box with small apertures for the lattice laser, clock laser, MOT beams, and fluorescence detection
- **Temperature sensors**: Multiple calibrated resistance temperature detectors (RTDs) mounted directly on the shield walls, read out during clock operation
- **Thermal uniformity**: High thermal conductivity of copper ensures $\Delta T < 10$ mK across the shield interior, much smaller than for the room-temperature vacuum chamber walls
- **Surface treatment**: Inner surface coated with **carbon nanotube (CNT) paint** to achieve high emissivity ($\epsilon \approx 1$) and suppress reflections of external radiation through the apertures

(source: K Beloy et al. PRL 2014.pdf)

## Carbon Nanotube Coating

The inner surface must emit as a near-ideal blackbody. If the inner surface had low emissivity, external room-temperature radiation entering through the apertures would contribute to the effective radiation temperature seen by the atoms. By coating with high-emissivity CNT paint ($\epsilon > 0.99$), the thermal radiation inside the enclosure is dominated by emission from the copper walls at the precisely known shield temperature, not by external radiation. (source: K Beloy et al. PRL 2014.pdf)

## Temperature Characterization

The shield temperature is measured during clock operation by the RTDs. The fractional uncertainty on the temperature measurement is $<10$ mK (absolute), enabling:

$$\delta(\sigma_\text{BBR}) \approx 4 \frac{\delta T}{T} \times \sigma_\text{BBR}(T) \approx 4 \times \frac{10\text{ mK}}{300\text{ K}} \times 2.45\times10^{-16} \approx 3\times10^{-20}$$

well below $10^{-18}$. However, the dynamic correction $\eta_\text{dyn}(T)$ introduces additional uncertainty from the ab initio calculation; Beloy 2014 computed $\eta_1 = 0.01745(38)$ and $\eta_2 = 0.000593(16)$, contributing a fractional uncertainty of $\sim 10^{-19}$.

## BBR Uncertainty After Shield

With the in-vacuum shield at NIST:

$$\sigma_y^\text{BBR} = 1\times10^{-18}$$

This represents a ~30× reduction from the pre-shield uncertainty (post Sherman 2012), and enabled the total systematic uncertainty to approach $10^{-18}$ for the first time in a Yb lattice clock. (source: K Beloy et al. PRL 2014.pdf)

## Alternative Approaches

Rather than a room-temperature shield, some groups operate with **cryogenic environments** that reduce $T$ itself, shrinking the BBR shift as $T^4$. At 100 K the shift drops to $(-2.45\times10^{-16})(100/300)^4 \approx 3\times10^{-18}$. At liquid nitrogen temperatures (77 K) it falls to $\sim 1\times10^{-18}$. Cryogenic shields require more complex engineering but reduce both the shift and its uncertainty.

NIST's room-temperature approach is notable for achieving $10^{-18}$ without cryogenics, by combining precise temperature measurement with the high-conductivity copper design.

## Related pages

- [[blackbody-radiation-shift]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
