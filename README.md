Hello, I'm Thomas Campagna! I am an undergraduate Physics and Math student at Austin Peay State University. I am an aspiring Computational Physicist specializing in Photonics and Environmental Physics. I have a particular interest in studying climate physics and how it relates to sustainable energy.


Research Interests:
- Condensed Matter
- Fluid Dynamics
- Thermodynamics
- Photonics

# Current Research & Projects

This page tracks my ongoing work in computational physics and experimental optics. My primary focus is on atmospheric modeling and optimizing the way we simulate complex physical systems.

---

## AURA-MPC: Model Predictive Control for Photovoltaic Panel Orientation

**The Goal:** Find the best pose for a 3-axis solar panel mount using model predictive control (MPC). Every 15 minutes the controller measures the weather, panel temperature, and pose, forecasts the next 15 minutes for each candidate pose, and applies the first move of the best plan.

### The Methodology
A lumped energy balance for the panel generates synthetic training data with an RK4 integrator written in Fortran. A neural surrogate and a physics-constrained model that learns only three physical constants forecast panel temperature 15 minutes ahead, and the MPC searches a pitch-yaw grid for the pose that maximizes electrical power.

* **Technical Stack:** Fortran (data generator), Python and PyTorch (surrogates and MPC), Raspberry Pi Pico data acquisition.
* **Key Results:** The surrogate matches its generator to 0.06 K. Under a power objective the best pose is always the max-irradiance pose. On a year of Sandia module data, a physics-calibrated model beats persistence (2.21 K vs 3.20 K RMSE), and in a closed-loop sandbox the MPC captures 98.7% of oracle energy.
* **Current Status:** Presented at SESAPS in November 2026. Next step is collecting thermocouple data on our own panel in Clarksville, TN.

**[AURA-MPC Project Page](https://thmscmpg.github.io/AURA-MF/){:target="_blank"}**

---

## Experimental Optics: Index of Refraction Study

**The Project:** "Comparative Analysis on the Refractive Index of a Prism Using a Versatile Spectrometer-Goniometer Setup" (Jair Martinez, Keira Scott, W. Thomas Campagna, Michael Graff, and Eugenii U. Donev)

We compare seven methods for determining the refractive index of a glass prism across five laser wavelengths, all on one spectrometer-goniometer setup, to see which offers the best balance of accuracy and pedagogical value. The methods include:
* **Geometric:** Angle of Minimum Deviation, Angle of Deviation Fit
* **Intensity-based:** Brewster's Angle, Fresnel Reflectance Fit
* **Phase-sensitive:** Rotating Analyzer Ellipsometry Fit, Total Internal Reflection, Polarized Total Internal Reflection

The angle of minimum deviation has been the most accurate so far (maximum 0.048%, average 0.023% error from Sellmeier values).

<img width="883" alt="Index of Refraction Data" src="https://github.com/user-attachments/assets/6463f09c-22e5-47a2-8dfa-a9c4c0bbf42f" />

> **Note on Figure:** This plot compares an earlier set of our experimental data against the Sellmeier Equation.

**Next Steps:** We are preparing the paper for the European Journal of Physics.

---

## Engineering & Electronics

Beyond my primary research, I maintain **CircuitNotes**—a library for hardware documentation and circuit theory.

* **[CircuitNotes Library](https://thmscmpg.github.io/CircuitNotes/)**
* **Focus:** 5V DC fundamentals, Arduino integration, and sensor theory.

---

## Other Projects

**Game Developer, Train Wreck Company.** I program gameplay and engine systems in C++ for BREACHPUNK, a 2D narrative game in development, and work on the studio's in-house engine and editor.

* **[Train Wreck Company](https://trainwreckcompany.github.io/)**
