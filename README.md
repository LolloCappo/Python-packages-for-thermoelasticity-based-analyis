# Thermoelasticity-based analysis: collection of python packages

[![DOI](https://zenodo.org/badge/286753213.svg)](https://zenodo.org/badge/latestdoi/286753213)

Thermoelasticity is a measurement techinque based on the thermoelastic effect, discovered by Weber in the 1830 and analytically described by Thomson in the 1853. If a structure is cyclically excited, its surface-temperature response variations are proportional to the change in the stress- and strain-tensor traces. As a non-contact, full-field and image-based measurement technique, multiple applications of thermoelasticity have been developed in recent years, as non-destructive testing, defects and material properties identification, stress-intensity factor definition and residual fatigue-life estimation. Due to this, four different python packages have been developed in order to allow to easily perform thermoelasticity-based data manipulation procedures.

In order to open .sfmov file extension saved from the thermal camera software, `pysfmov` package has been published. It allows to get the raw data and the meta data informations from the acquisition files. Install it via pip using:
```python
    $ pip install pysfmov
```	
In order to perform a digital lock-in analysis, `pyLIA` has been also released. Lock-in analysis is necessary as preliminary step in order to single out the informations from the noise inherent into the techinque. Install it via pip using:
```python
    $ pip install pyLIA
```	
To allow the identification of the thermoelastic coefficient, thorugh different ways, `ThermCoeff` module has been developed: coefficients of standard materials are given from literature, but also classic strain-gauge calibration procedure is available. Install it via pip using:
```python
    $ pip install ThermCoeff
```	
For the fatigue life estimation from thermal acquisitions, `IR_FLife` module has been published. Time- and frequency-domain-based approaches are generally used to estimate the damage intensity occurred on a flexible structures under random loads. While the established spectral methods for the damage intensity identification give good results if high-dynamic range sensors (e.g, piezo accelerometers) are used, these methods have a relatively large uncertainty with considering small-dynamic-range sensors (e.g., thermal cameras). Moreover, the spatial information from a thermal camera can be used to obtain spatial damage-intensity information. Thus, based on the modal-decomposition theory, a modal damage-intensity identification based on the thermoelastic principle has been proposed. Due to the fact that the modal-damage-intensity method relies on the modal information at a particular natural frequency, the uncertainty is significantly reduced, if compared to classic spectral methods. More importantly, the damage intensity can be decomposed to particular mode shapes, and with the modal damage information, the source of the damage is clearly revealed. Install it via pip using:
```python
    $ pip install IR_FLife
```	

Source code for pysfmov: https://github.com/LolloCappo/pysfmov

Source code for pyLIA: https://github.com/LolloCappo/pyLIA

Source code for ThermCoeff: https://github.com/LolloCappo/ThermCoeff

Source code for IR_FLife: https://github.com/LolloCappo/IR_FLife

