Authors:
Jérôme Kieffer, Edgar Gutierrez Fernandez,  Thomas Vincent, Loïc Huder, Gudrun Lotze

+ Probably Nils Blanc for the images of LaB6 taken on CdTe & Si detectors in same conditions

Title:
Coping with the parallax effect in 2D X-ray detectors

Abstract:

Intro (AI-gen)
The parallax effect in X-ray area detectors arises when X-rays from a point source (e.g., a scattering sample) traverse thick detection layers, causing a shift in the apparent position of detected events. This can degrade angular resolution and introduce artefacts, especially in pair distribution function (PDF) analysis and powder diffraction measurements.
In thick detectors, X-rays at high scattering angles may pass through multiple pixels, leading to discrepancies between observed and actual scattering angles (2θ)

1.state of the art:

1.1 Work in 1D:
Simple offline data corrections have been proposed to restore original scattering information, particularly for one-dimensional parallax effects
1.2 Use cylindrical/spherical or smaller detectors mounted on a goniometer arm
1.3 Neural network based 

2. Physics of the parallax effect
   1.1. Beer-Lambert Law
   1.2 Simulation of the parallax effect using Raytracing
      1.2.1: Description of the implementation
      1.2.2: blurring of a synthetic powder diffraction frame
   1.3 Correction by deconvolution (RL, MLEM, ...)
      1.3.1 Theory behind deconvolution
      1.3.2 Deconvolution of synthetic data
      1.3.3 Deconvolution of real data
3. Average parallax effect
   2.1 Calculation of the displacement
   2.2 Correction of the displacement
   2.3 Application to sythetic data
   2.4 Application to experimental data (LaB6 on CdTe & Si detectors)
4. Discussion
   4.1. Usage in pyFAI, and limitations:
   Detector thickness is only one term of peak broadening: sample height, width, pixel size, beam divergence, and wavelength dispersion are important too and not taken into account.
   4.2. Application to powder diffraction and PDF measurement 
6. Conclusion


Biblio:
1d correction a prosteriori : https://doi.org/10.1107/S1600576719011580
To read: [https://www.sciencedirect.com/science/article/abs/pii/S092056329580062X](https://doi.org/10.1016/S0920-5632(95)80062-X)
[https://www.sciencedirect.com/science/article/pii/S0168900217309555](https://doi.org/10.1016/j.nima.2017.08.060)
Something else, XRDCT: https://doi.org/10.1038/s41524-024-01389-1 
Cherni: https://doi.org/10.1107/S1600576722003089
gonio: https://pmc.ncbi.nlm.nih.gov/articles/PMC9172033/
Coelho: https://pmc.ncbi.nlm.nih.gov/articles/PMC4849620/
        https://nvlpubs.nist.gov/nistpubs/jres/109/1/j91che.pdf
Scardi: https://doi.org/10.1107/S0108767301008881


