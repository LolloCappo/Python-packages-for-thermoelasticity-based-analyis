---
title: 'Thermoelasticity-based analysis: collection of python packages'
tags:
  - Python
  - Thermoelasticity
  - Vibration fatigue
  - Lock-in amplifier
  - Thermal camera
authors:
  - name: Lorenzo Capponi
    orcid: 0000-0002-1333-9930
    affiliation: 1
affiliations:
  - name: CISAS G. Colombo, University of Padova, Italy
    index: 1
date: 11 August 2020
bibliography: paper.bib
---

# Summary

Thermoelasticity is a measurement techinque based on the thermoelastic effect, discovered by Weber [@Weber:1830] in the 1830 and analytically described by Thomson [@Thomson:1853] in the 1853. If a structure is cyclically excited, its surface-temperature response variations are proportional to the change in the stress- and strain-tensor traces [@Thomson:1853]:
\begin{equation}\label{eqtsa_0}
\rho\, C_\sigma \frac{\Delta T}{T_0} = -\alpha\,\left(\Delta \sigma_x+\Delta \sigma_y+\Delta \sigma_z\right)
\end{equation}
where $\rho$ is the material density, $C_\sigma$ is the specific heat at constant pressure, $T_0$ is the ambient temperature, $\Delta T$ is the temperature change, $\alpha$ is the thermal expansion coefficient and $\Delta \sigma_i$ are the stress tensor components.
As a non-contact, full-field and image-based measurement technique, multiple applications of thermoelasticity have been developed in recent years, as non-destructive testing [@Guo:2015], defects and material properties identification [@Allevi:2019], stress-intensity factor definition and residual fatigue-life estimation [@Li:2012],[@Capponi:2020]. Due to this, four different python packages have been developed in order to allow to easily perform thermoelasticity-based data manipulation procedures.

# Statement of need 

In order to open .sfmov file extension saved from the thermal camera software, `pysfmov` package has been published. It allows to get the raw data and the meta data informations from the acquisition files. Install it via pip using:
```python
    $ pip install pysfmov
```	
In order to perform a digital lock-in analysis, `pyLIA` has been also released. Lock-in analysis is necessary as preliminary step in order to single out the informations from the noise inherent into the techinque [@Montanini:2020]. Install it via pip using:
```python
    $ pip install pyLIA
```	
To allow the identification of the thermoelastic coefficient, thorugh different ways, `ThermCoeff` module has been developed: coefficients of standard materials are given from literature, but also classic strain-gauge calibration procedure is available. Install it via pip using:
```python
    $ pip install ThermCoeff
```	
For the fatigue life estimation from thermal acquisitions, `IR_FLife` module has been published. Time- and frequency-domain-based approaches are generally used to estimate the damage intensity occurred on a flexible structures under random loads. While the established spectral methods for the damage intensity identification give good results if high-dynamic range sensors (e.g, piezo accelerometers) are used, these methods have a relatively large uncertainty with considering small-dynamic-range sensors (e.g., thermal cameras). Moreover, the spatial information from a thermal camera can be used to obtain spatial damage-intensity information. Thus, based on the modal-decomposition theory, a modal damage-intensity identification based on the thermoelastic principle has been proposed [@Capponi:2020]. Due to the fact that the modal-damage-intensity method relies on the modal information at a particular natural frequency, the uncertainty is significantly reduced, if compared to classic spectral methods. More importantly, the damage intensity can be decomposed to particular mode shapes, and with the modal damage information, the source of the damage is clearly revealed. Install it via pip using:
```python
    $ pip install IR_FLife
```	

# Acknowledgements

I acknowledge contributions from Janko Slavič, Domen Gorjup and Klemen Zaletelj (members of the LADISK of the Faculty of Engineering of the University of Ljubljana) during the genesis of each pyhton package.

# References