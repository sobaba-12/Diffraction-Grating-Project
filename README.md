# Diffraction-Grating-Project
A 2nd Year project that involved creating a data analysis process for producing results on data from a sensor.

This assessed project analysed simulated data using Python, with the final goal of preparing a simple report displaying key results and a discription of how the code works.

## Background

The tasks in this assessed coursework centre around the interpretation of diffraction patterns generated when laser light is shone through a small aperture in a screen. It builds upon some of the physics covered in the optics part of Physics 2.

### Intensity Equations

- $I(\phi) = I_0sinc^2\left(k(L/2)\sin\phi\right)$, this is the function for testing for *square* aperture
- $I(\theta)=I_0sinc^4\left[kW\sin\theta/(2\sqrt{2})\right]$, where $W$ is the length of one side of the diamond, this is the function for testing *diamond* apertures
- $I(\theta) = I_0\left(\frac{2 J_1(\pi kD\sin\theta)}{\pi kD\sin\theta}\right)^2$, this is the function for testing for *circle* aperture

The two important properties of the diffraction pattern are:
1. The symmetry of the diffraction pattern is the same as the symmetry of the aperture - thus  diamond aperture has 4 
fold rotation symmetry and mirror planes every 45 degrees, as does its diffraction pattern - while a rectangular 
aperture only has 2-fold rotation and 2 sets of mirror planes, as does it diffraction pattern. The diffraction pattern 
of a circular aperture is itself ring-like.
2. There is a reciprocal relationship between the dimensions of the diffraction pattern and the dimensions of the aperture. A rectangular aperture's diffraction is more 'bunched up' in the aperture's long direction and more spread out in he
aperture's short direction.


### Analysing the Diffraction Patterns

- This was simply achieved using Chi Squared Testing
