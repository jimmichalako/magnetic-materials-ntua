# NTUA ECE Magnetic Materials and Applications Course

This repository showcases the theoretical assignments, laboratory exercises, and computational analysis I completed during the Magnetic Materials and Applications course at NTUA. Through this coursework, I gained hands-on experience in magnetic hysteresis characterization, coherent rotation modeling (Stoner-Wohlfarth), magnetostrictive delay line (MDL) dynamics, electromagnetic coil design, and non-destructive testing (NDT) using Hall effect and AMR magnetic sensors.

## Theoretical Exercises

### Exercise 1: Magnetic Hysteresis Characterization
*Analysis of hysteresis loops and fundamental magnetic properties of soft magnetic materials.*

* **Key Tasks:**
  * **Part A (Loop Construction & Comparison):** Plotted and compared fully dimensioned $B(H)$ and $M(H)$ loops for two distinct magnetic materials to classify softness, magnetic sensitivity, and saturation.
  * **Part B (Permeability & Susceptibility):** Computed and evaluated normal permeability $\mu(H)$, magnetic susceptibility $\chi(H)$, and differential permeability $\mu_d(H) = dB/dH$.
  * **Part C (Parameter Extraction):** Extracted coercive field ($H_c$), remanent magnetization ($B_r$), maximum differential permeability ($\mu_{0,\text{max}}$), and total hysteresis loss (loop area).
* **Tech Stack:** Python, NumPy, Matplotlib, Data Analysis.

### Exercise 2: Solenoid & Core Magnetic Circuit Design
*Electromagnetic design, wire sizing, and parameter derivation for air-core and ferromagnetic-core inductors.*

* **Key Tasks:**
  * **Part A (Straight Solenoid Design):** Designed an air-core copper solenoid ($l = 100\text{ mm}$, $r = 5\text{ mm}$) to achieve an internal field of $H = 10\text{ kA/m}$. Selected appropriate wire gauge (AWG 14) and computed DC ohmic resistance ($R$) and self-inductance ($L$).
  * **Part B (Magnetic Circuit with Air Gap):** Designed an excitation coil on a ferromagnetic core ($\mu = 2000\mu_0$) with an air gap ($l_g = 2\text{ mm}$) to generate $H_{\text{gap}} \approx 10\text{ kA/m}$, accounting for ampere-turns, wire limits, and dissipation.
* **Tech Stack:** Electromagnetic Theory, Analytical Circuit Modeling.

### Exercise 3: Stoner-Wohlfarth Coherent Rotation Model
*Simulation of magnetization reversal in single-domain uniaxial nanoparticles.*

* **Key Tasks:**
  * **Part A (Energy Minimization & Astroid):** Formulated total free energy $E(\phi)$ and derived the Stoner-Wohlfarth astroid switching criterion ($h_x^{2/3} + h_y^{2/3} = 1$) via first and second derivatives.
  * **Part B (Root Finding & Tracking):** Transformed equilibrium conditions into a 4th-degree polynomial in $k = \tan(\phi/2)$ and tracked stable roots to capture abrupt magnetization jumps.
  * **Part C (Hysteresis Simulation):** Simulated normalized hysteresis loops $m(h)$ for field angles $\theta \in [0^\circ, 90^\circ]$ stepping $h$ between $+1.0$ and $-1.0$.
* **Tech Stack:** Python, SciPy, Polynomial Root Finding, Numerical Simulation.

## Laboratory Exercises

### Lab 1: Amorphous Materials Hysteresis & Fluxgate Sensors
*Characterization of CoFeSiB / FeSiB amorphous ribbons/wires and fluxgate sensor mechanisms.*

* **Key Tasks:**
  * **Part A (Fluxgate Field Sensor):** Analyzed time asymmetry ($\Delta t$) between waveform extrema under varying DC bias offsets ($-3\text{ V}$ to $+3\text{ V}$) at $1\text{ kHz}$ and $5\text{ kHz}$ excitation.
  * **Part B (Fluxgate Position Sensor):** Measured output amplitude variation as a function of magnetic core displacement ($x = 0$ to $50\text{ mm}$).
  * **Part C (Dynamic Hysteresis & Integration):** Digitized $I_{\text{in}}(t)$ and $V_{\text{out}}(t)$, performed numerical integration ($\int V_{\text{out}}\,dt$) in Python/Jupyter to reconstruct dynamic $B$–$H$ hysteresis loops across frequencies ($100\text{ Hz}$–$1\text{ kHz}$) and driving voltages.
* **Tech Stack:** Jupyter Notebook, Python, NumPy, Matplotlib, Numerical Integration.

### Lab 2: Magnetostrictive Delay Lines (MDL)
*Investigation of acoustic longitudinal wave propagation in magnetostrictive delay lines for sensor applications.*

* **Key Tasks:**
  * **Part A (Pulse Propagation & Echoes):** Evaluated acoustic pulse transmission along an amorphous delay line at varying coil separations ($0$, $100$, and $200\text{ mm}$), measuring propagation delay ($\Delta t$) and identifying end-reflections.
  * **Part B (Position Sensing):** Built calibration curves relating acoustic time-of-flight ($\Delta t$) to coil distance ($100$–$250\text{ mm}$).
  * **Part C (Mechanical Pressure/Load Sensing):** Measured output pulse amplitude degradation under calibrated loading weights ($5\text{ g}$–$200\text{ g}$) to construct a mass-response calibration curve.
* **Tech Stack:** Jupyter Notebook, Python, Matplotlib, Signal Analysis.

### Lab 3: Non-Destructive Testing (NDT) via Magnetic Sensors
*Detection of structural defects and stress-induced permeability shifts using Hall and AMR sensors.*

* **Key Tasks:**
  * **Part A (Stress-Induced Permeability):** Evaluated magnetoelastic behavior of electrical steel under tensile ($\sigma > 0$) and compressive ($\sigma < 0$) mechanical stress.
  * **Part B (Hall Sensor Defect Detection):** Analyzed surface magnetic field leakage across steel specimens (flawless, single defect, dual defect) using moving average noise filtering.
  * **Part C (AMR Sensor Weld Inspection):** Processed Anisotropic Magnetoresistive (AMR) scanner data across welded plates and double-defect specimens to identify fault signatures.
* **Tech Stack:** Jupyter Notebook, Python, Pandas, Signal Smoothing / Moving Average Filters.

## Technologies Used

* **Languages:** Python (Jupyter Notebooks)
* **Libraries & Tools:** NumPy, SciPy, Matplotlib, Pandas, Microsoft Excel
* **Core Concepts:** Magnetic Hysteresis, Stoner-Wohlfarth Model, Magnetostriction (MDL), Fluxgate Sensor Principles, Hall Effect, Anisotropic Magnetoresistance (AMR), Non-Destructive Testing (NDT), Electromagnetic Coil Design
* **Environments:** Jupyter Lab / Google Colab, Technical Reports (PDF)
