# Blackbody Radiation Shift

**Summary**: The AC Stark shift of the clock transition due to the broad-spectrum thermal radiation field of the apparatus at room temperature, the dominant systematic uncertainty in early Yb lattice clocks and reduced to 10⁻¹⁸ by an in-vacuum cryogenic shield.

**Sources**: N D Lemke et al. PRL 2009.pdf, J A Sherman et al. PRL 2012.pdf, K Beloy et al. PRL 2014.pdf, A Ludlow et al. RMP 2015.pdf

**Last updated**: 2026-04-26

---

## Physical Mechanism

Any object at temperature $T$ emits a blackbody radiation (BBR) field whose spectral density follows the Planck distribution. This thermal field has a non-zero mean-square electric field:

$$\langle E^2 \rangle_T = \frac{(831.9\text{ V/m})^2}{1} \left(\frac{T}{300\text{ K}}\right)^4$$

This time-averaged field produces an AC Stark shift of all atomic levels. For the clock transition, the **differential** static polarizability $\Delta\alpha(0) = \alpha_{3P_0}(0) - \alpha_{1S_0}(0)$ determines the magnitude of the shift. The static (zero-frequency) polarizability is used because the thermal spectrum peaks far below any atomic resonance frequency.

The leading-order BBR fractional frequency shift is:

$$\frac{\delta\nu_\text{BBR}}{\nu_\text{clock}} \approx -\frac{\Delta\alpha(0)}{2h\epsilon_0 c} \langle E^2 \rangle_T \cdot [1 + \eta_\text{dyn}(T)]$$

where $\eta_\text{dyn}(T)$ is the **dynamic correction** that accounts for the finite-frequency distribution of the BBR spectrum and the frequency dependence of the polarizability. (source: A Ludlow et al. RMP 2015.pdf)

## Differential Static Polarizability

The key atomic parameter. For ¹⁷¹Yb:

$$\Delta\alpha(0) = 36.2612(7) \text{ kHz(kV/cm)}^{-2} = 145.726(3) \text{ a.u.}$$

(source: J A Sherman et al. PRL 2012.pdf)

This was measured by Sherman et al. (NIST 2012) using a calibrated DC electric field applied to atoms in the lattice. The clock frequency shift vs. applied field gradient gives $\Delta\alpha(0)$ directly. The uncertainty of 3 ppm was a 40× improvement over prior theoretical estimates and reduced the BBR fractional frequency uncertainty to $3\times10^{-17}$.

**Sherman 2012 method**: The DC electric field is applied via biased electrodes inside the vacuum chamber. The Stark shift of the clock frequency is measured as a function of voltage, and the electrode geometry is characterized by finite-element modeling to convert voltage to electric field at the atomic position. (source: J A Sherman et al. PRL 2012.pdf)

## BBR Shift at 300 K

For a room-temperature environment ($T = 300$ K):

$$\delta\nu_\text{BBR}(300\text{ K}) = -1.273(17) \text{ Hz}$$

corresponding to a fractional shift of:

$$\frac{\delta\nu_\text{BBR}}{\nu_\text{clock}} = -2.454(33)\times10^{-16}$$

(source: J A Sherman et al. PRL 2012.pdf)

## Dynamic Correction

At finite temperature the BBR spectrum has components at non-zero frequency where the atomic polarizability differs from its static value. The dynamic correction is:

$$\eta_\text{dyn}(T) \approx \eta_1 \left(\frac{T}{300\text{ K}}\right)^2 + \eta_2 \left(\frac{T}{300\text{ K}}\right)^4$$

For ¹⁷¹Yb (Beloy 2014 ab initio calculation):

| Parameter | Value | Uncertainty |
|-----------|-------|-------------|
| $\eta_1$ | 0.01745 | 0.00038 |
| $\eta_2$ | 0.000593 | 0.000016 |

The $\eta_1$ term contributes at the $\sim 2\%$ level at 300 K (since $\eta_1 = 0.017$) and becomes important at the $10^{-18}$ level. (source: K Beloy et al. PRL 2014.pdf)

## Uncertainty Evolution

| Year | Lab | BBR uncertainty | Method |
|------|-----|----------------|--------|
| 2009 | NIST | $9.7\times10^{-16}$ | Theory + $\pm1$ K temperature control |
| 2012 | NIST | $3\times10^{-17}$ | DC Stark shift measurement of $\Delta\alpha(0)$ |
| 2014 | NIST | $1\times10^{-18}$ | In-vacuum copper BBR shield (see [[bbr-shield]]) |

(sources: N D Lemke et al. PRL 2009.pdf, J A Sherman et al. PRL 2012.pdf, K Beloy et al. PRL 2014.pdf)

The 2009 uncertainty was dominated by the 10% uncertainty in the theoretical static polarizability. After Sherman 2012 measured $\Delta\alpha(0)$ at the ppm level, the dominant uncertainty became temperature measurement: at room temperature, 1 K uncertainty in the apparatus temperature gives a $4\times10^{-17}$ BBR uncertainty (since the shift scales as $T^4$).

The Beloy 2014 in-vacuum shield solution is described in detail in [[bbr-shield]].

## Temperature Sensitivity

Because the BBR shift scales as $T^4$:

$$\frac{d(\delta\nu_\text{BBR}/\nu)}{dT} \approx -4 \times \frac{-2.454\times10^{-16}}{300\text{ K}} \approx 3.3\times10^{-18}/\text{K}$$

at 300 K. To keep the BBR uncertainty below $10^{-18}$, the thermal environment must be known to $<0.3$ K unless the shield temperature is reduced.

## Comparison with Theoretical Estimates

Before the Sherman 2012 measurement, $\Delta\alpha(0)$ was available only from atomic structure calculations. The theoretical value from Porsev et al. (2006) was $\Delta\alpha(0) \approx 36(1)$ a.u. — a ~3% uncertainty that dominated the BBR budget. Sherman 2012's experimental value of 145.726(3) a.u. (same in different units) reduced this uncertainty by ~40×, without requiring improvement in the temperature measurement.

## Related pages

- [[bbr-shield]]
- [[systematic-uncertainty-budget]]
- [[optical-lattice-clock]]
- [[yb-atomic-structure]]
- [[clock-transition-yb]]
