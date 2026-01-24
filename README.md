Hello, I'm Thomas Campagna! I am an undergraduate Physics and Math student at Austin Peay State University. I am an aspiring Computational Physicist specializing in Photonics and Environmental Physics. I have a particular interest in studying climate physics and how it relates to sustainable energy.


Research Interests:
- Condensed Matter
- Fluid Dynamics
- Thermodynamics
- Photonics

# Current Research & Projects

This page tracks my ongoing work in computational physics and experimental optics. My primary focus is on atmospheric modeling and optimizing the way we simulate complex physical systems.

---

## Atmospheric Unified Radiation Assessment (AURA-MF)

**The Goal:** Simulating how light and heat move through air is computationally "expensive." My work involves coupling the **Boltzmann Transport Equation** (radiation travel) with **Navier-Stokes** (fluid flow) to create a more efficient model.

### The Methodology
Standard high-fidelity models take a long time to run. I am implementing a **multi-fidelity approach** where a fast, low-fidelity model guides the high-fidelity one. This allows the simulation to maintain high physical accuracy while significantly cutting down on processing time and energy costs.

* **Technical Stack:** Written in **Fortran 90** with **OpenMP** for parallelization.
* **Key Techniques:** Monte-Carlo methods, diffusion approximations, and coarse discretization.
* **Current Status:** As of December 2025, the proof of concept is stable. I'm currently focused on further optimization and benchmarking against high-fidelity-only results.



**[Explore the AURA-MF Repository](https://github.com/THMSCMPG/AURA-MF){:target="_blank"}**

---

## Experimental Optics: Index of Refraction Study

**The Project:** "Comparing 5 Methods for Determining the Index of Refraction of a Glass Prism."

We are evaluating different experimental techniques to see which offers the best balance of accuracy and pedagogical value. The methods include:
* Minimum Deviation
* Fresnel Reflectance
* Fitting to the Minimum Deviation Curve
* Brewster’s Angle
* Rotating Analyzer Ellipsometry (RAE)

<img width="883" alt="Index of Refraction Data" src="https://github.com/user-attachments/assets/6463f09c-22e5-47a2-8dfa-a9c4c0bbf42f" />

> **Note on Figure:** This plot compares our experimental data against the Sellmeier Equation. Our most recent RAE data is currently being integrated into the final analysis.

**Next Steps:** Moving forward, our team will be expanding this research to look specifically at total internal reflection.

---

## Engineering & Electronics

Beyond my primary research, I maintain **CircuitNotes**—a library for hardware documentation and circuit theory.

* **[CircuitNotes Library](https://thmscmpg.github.io/CircuitNotes/)**
* **Focus:** 5V DC fundamentals, Arduino integration, and sensor theory.
