<div style="text-align: center; background-color: #2e353d; padding: 10px; border-radius: 5px; margin-bottom: 30px;">
<span style="color: white;">
<a href="{{ '/' | relative_url }}">Home</a> | 
<a href="{{ '/projects' | relative_url }}">Research</a> | 
<a href="{{ '/reports' | relative_url }}">Lab Reports</a> | 
<a href="{{ '/assets/Campagna_CV_2025.pdf' | relative_url }}" target="_blank">CV</a>
</span>
</div>

# My Research Projects

## Comparing 5 Methods to Determine the Index of Refraction of a Glass Prism
**The Objective:** This research evaluates the precision and pedagogical utility of five distinct experimental methodologies for determining the refractive index of optical glass. We quantify the systematic uncertainties inherent in each approach. A central component of this study involves fitting experimental dispersion data to the Sellmeier Equation, allowing for a robust comparison against theoretical values. This work serves not only to validate high-precision optical techniques but also to identify the most effective methodologies for undergraduate-level optics.

**The Methods List:**
- Minimum Deviation
- Fresnel Reflectance
- Minimum Deviation Curve Fitting
- Brewster’s Angle
- Rotating Analyzer Ellipsometry (RAE)

**The Math:** The Sellmeier Equation is the standard for refractive index dispersion.
It displays an empirical relationship between the index of refraction and the wavelength for any transparent medium. The Sellmeier Equation makes use of two experimentally determined coefficients representing physical features of the transparent medium and the lasers wavelength in nanometers.

**The Findings:** The angle of minimum deviation has shown the highest accuracy (≤ 0.03% error from Sellmeier values).

**Current Progress:** We are currently wrapping up RAE and beginning our sixth and final method, **Total Internal Reflection**.

## Atmospheric-Unified Radiation Assessment with Multi-Fidelity (AURA-MF)
**The Scientific Problem:** I am coupling the Boltzmann Transport Equation (BTE) (for photon/radiation travel) with Navier-Stokes (N-S) (for air/fluid flow). Solving both at a high resolution is too computationally expensive, as such I am implementing various degrees of fidelity in order to approximate accurate values with fewer resources.

**The Methodology:** Currently, I am using a low-fidelity model (fast, less accurate) to guide a high-fidelity model (slow, very accurate) to save time without losing physics for each set of equations. The resulting outputs are compared with the data produced by a coupled high-fidelity only model.

**Technical Stack:** The simulation's program is written in Fortran 90 and OpenMP. I take advantage of Monte-Carlo simulations, the diffusion approximation, the poisson approximation, and coarse discretization.

**Current Progress:** As of December 2025, the proof of concept has been finalized and I am moving forwards with optimization.

<img width="640" alt="temperature_result" src="https://github.com/user-attachments/assets/8335d10a-f222-475d-8fde-8c1e0b626a56" />
| Fig. 1: 2D temperature graph |

<img width="640" alt="space_time_3d_surface" src="https://github.com/user-attachments/assets/6463f09c-22e5-47a2-8dfa-a9c4c0bbf42f" />
| Fig. 2: 3D temperature graph for x-coordinate over time |
