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

date: 11 August 2020
bibliography: paper.bib
---

# Summary
Thermoelasticity is a growing measurement techinque based on the thermoelastic effect, discovered by Weber [@Weber1830UberMetalle] in the 1830 and analytically described by Thomson [@Thomson1853OnHeat] in the 1853. If a structure is cyclically excited, its surface-temperature response variations are proportional to the change in the stress- and strain-tensor traces [@Thomson1853OnHeat].

# Statement of need 
Time- and frequency-domain-based approaches are generally used to estimate the damage intensity occurred on a flexible structures under random loads. While the established spectral methods for the damage intensity identification give good results if high-dynamic range sensors (e.g, piezo accelerometers) are used, these methods have a relatively large
uncertainty with considering small-dynamic-range sensors (e.g., thermal cameras). Moreover, the spatial information from a thermal camera can be used to obtain spatial damage-intensity information. Thus, based on the modal-decomposition theory, a modal damage-intensity identification based on the thermoelastic principle has been proposed [@Capponi..]. Due to the fact that the modal-damage-intensity method relies on the modal information at the natural frequency, the uncertainty is significantly reduced, if compared to classic spectral methods. More importantly, the damage intensity can be decomposed to particular mode shapes. With the modal damage information, the source of the damage is clearly revealed.

# Mathematics

Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{pix}$

Double dollars make self-standing equations

$$Theta(x) = left{begin{array}{l}
0textrm{ if } x  0cr
1textrm{ else}
end{array}right.$$

You can also use plain LaTeX for equations
begin{equation}label{eqfourier}
hat f(omega) = int_{-infty}^{infty} f(x) e^{iomega x} dx
end{equation}
and refer to autoref{eqfourier} from text.

# Citations

Citations to entries in paper.bib should be in
[rMarkdown](httprmarkdown.rstudio.comauthoring_bibliographies_and_citations.html)
format.

If you want to cite a software repository URL (e.g. something on GitHub without a preferred
citation) then you can do it with the example BibTeX entry below for @fidgit.

For a quick reference, the following citation commands can be used
- `@author2001`  -  Author et al. (2001)
- `[@author2001]` - (Author et al., 2001)
- `[@author12001; @author22001]` - (Author1 et al., 2001; Author2 et al., 2002)

# Figures

Figures can be included like this
![Caption for example figure.label{figexample}](figure.png)
and referenced from text using autoref{figexample}.

Fenced code blocks are rendered with syntax highlighting
```python
for n in range(10)
    yield f(n)
```	

# Acknowledgements

I acknowledge contributions from Janko Slavič, Domen Gorjup and Klemen Zaletelj during the genesis of this project.

# References