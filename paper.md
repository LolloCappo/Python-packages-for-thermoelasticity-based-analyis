---
title: 'Python packages for thermoelasticity-based analysis'
tags:
  - Python
  - Thermoelasticity
  - Vibration fatigue
  - Lock-in amplifier
  - Thermal camera
authors:
  - name: Lorenzo Capponi
    orcid 0000-0002-1333-9930
    affiliation: 1
affiliations:
  - name: CISAS G. Colombo, University of Padova, Italy
  - index: 1 
date: 11 August 2020
bibliography: paper.bib
---

# Summary

Thermoelasticity is a growing measurement techinque based on the thermoelastic effect, discovered by Weber [@Weber1830] in the 1830 and analytically described by Thomson [@Thomson1853] in the 1853. If a structure is cyclically excited, its surface-temperature response variations are proportional to the change in the stress- and strain-tensor traces [@Thomson1853]. As a non-contact, full-field and image-based measurement technique, multiple applications of thermoelasticity have been developed in recent years, as non-destructive testing [@Guo2015], defects and material properties identification [@Allevi2019], stress-intensity factor definition and residual fatigue-life estimation [@Li2012][@Capponi2020]. Due to this, four different python packages have been developed in order to allow to easily perform thermoelasticity-based data manipulation procedures.

# Statement of need 

Time- and frequency-domain-based approaches are generally used to estimate the damage intensity occurred on a flexible structures under random loads. While the established spectral methods for the damage intensity identification give good results if high-dynamic range sensors (e.g, piezo accelerometers) are used, these methods have a relatively large uncertainty with considering small-dynamic-range sensors (e.g., thermal cameras). Moreover, the spatial information from a thermal camera can be used to obtain spatial damage-intensity information. Thus, based on the modal-decomposition theory, a modal damage-intensity identification based on the thermoelastic principle has been proposed [@Capponi2020]. Due to the fact that the modal-damage-intensity method relies on the modal information at the natural frequency, the uncertainty is significantly reduced, if compared to classic spectral methods. More importantly, the damage intensity can be decomposed to particular mode shapes. With the modal damage information, the source of the damage is clearly revealed.

# Mathematics

You can also use plain LaTeX for equations
begin{equation}label{eqfourier}
hat f(omega) = int_{-infty}^{infty} f(x) e^{iomega x} dx
end{equation}
and refer to autoref{eqfourier} from text.

Fenced code blocks are rendered with syntax highlighting
```python
    $ pip install pySFMOV
```	

# Acknowledgements

I acknowledge contributions from Janko Slavič, Domen Gorjup and Klemen Zaletelj (members of the LADISK of the Faculty of Engineering of the University of Ljubljana) during the genesis of each pyhton module and package.

# References