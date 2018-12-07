WDdata
=======

**Copyright 2018- The DA WD Calibration Team (contact: gsnarayan@gmail.com)**

About
-----
|githubWDmodel| |docsWDmodel| |doi|

This ``WDdata`` repository contains combined HST Cycle 20 and Cycle 22 DA White
Dwarf (DAWD) photometry (GO 12967, 13711, P.I. Saha) and ground-based
spectroscopy. This data can be used together with the ``WDmodel`` to infer SEDs of the DAWDs from their
observed spectroscopy and photometry. The data are described in Calamida et al.
(2018, submitted) and the analysis in Narayan et al. (2018, submitted).

Click on the badges above  for code, licensing and documentation.

.. |githubWDmodel| image:: https://img.shields.io/badge/Github-gnarayan%2FWDmodel-blue.svg
    :alt: Github Link
    :target: http://github.com/gnarayan/WDmodel

.. |docsWDmodel| image:: http://readthedocs.org/projects/wdmodel/badge/?version=latest
    :alt: Documentation Status
    :target: http://wdmodel.readthedocs.io/en/latest/?badge=latest

.. |doi| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2032365.svg
   :target: https://doi.org/10.5281/zenodo.2032365

Structure
---------

This data release contains::

|    WDdata                                  - this directory
|        ├── LICENSE                         - MIT boilerplate
|        ├── README.rst                      - this file
|        ├── wdcalib_target_list.dat         - coordinates of targets (bad = #), cycle specifies which HST cycle (01 = CALSPEC, 15 = secondary)
|        ├── photometry                      - photometry directory
|        │   ├── src                         - instrumental magnitudes + scripts to regenerate apparent magnitudes
|        │   ├── WDphot_ILAPHv5_abmag.dat    - Apparent magnitudes of C20+C22 targets + CALSPEC primary standards as ABmag
|        │   └── <synphot tables>            - Files for the WFC3 bandpasses from STScI 
|        ├── spectroscopy                    - spectroscopy directory
|        │   ├── gemini                      - Gemini GMOS spectroscopy of C20 targets
|        │   ├── mmt                         - MMT Blue Channel spectroscopy of C20+C22 targets
|        │   ├── imacs                       - A lone Magellan IMACS spectrum we got to assess the suitability of IMACS 
|        │   └── spectable_resolution.dat    - Upper limits on the resolution of each spectrum + any wavelength shift to be applied
|        └── out
|             ├── <specname>                 - Files containing the SED, and fit properties for each object's best spectrum in spectroscopy dir 
|             └── tables                     - Contains summary tables of photometric residuals, fit results, synthetic photometry 
