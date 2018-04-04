WDdata
=======

**Copyright 2018- The DA WD Calibration Team (contact: gsnarayan@gmail.com)**

About
-----
|githubWDmodel| |docsWDmodel| |githubWDFitPhot|

This ``WDdata`` repository contains combined HST Cycle 20 and Cycle 22 DA White
Dwarf (DAWD) photometry (GO 12967, 13711, P.I. Saha) and ground-based
spectroscopy. This data can be used together with the ``WDmodel``  or the
``WDFitPhot`` calibration code to infer the SEDs of the DAWDs from their
observed spectroscopy and photometry. The data are described in Calamida et al.
(2018, in prep) and the analysis in Narayan et al. (2018, in prep).

Click on the badges above  for code, licensing and documentation.

.. |githubWDmodel| image:: https://img.shields.io/badge/Github-gnarayan%2FWDmodel-blue.svg
    :alt: Github Link
    :target: http://github.com/gnarayan/WDmodel

.. |docsWDmodel| image:: http://readthedocs.org/projects/wdmodel/badge/?version=latest
    :alt: Documentation Status
    :target: http://wdmodel.readthedocs.io/en/latest/?badge=latest

.. |githubWDFitPhot| image:: https://img.shields.io/badge/Github-taxelrod%2FWDFitPhot-blue.svg
    :alt: Github Link
    :target: http://github.com/taxelrod/WDFitPhot


Structure
---------

.. code-block:: text
::
WDdata                                  - this directory
    ├── LICENSE                         - MIT boilerplate
    ├── README.rst                      - this file
    ├── photometry                      - photometry directory
    │   ├── src                         - instrumental magnitudes + scripts to regenerate apparent magnitudes
    │   └── WDPhot_ILAPHv3.dat          - Apparent magnitudes of C20+C22 targets + CALSPEC primary standards as Vegamag 
    └── spectroscopy                    - spectroscopy directory
        ├── gemini                      - Gemini GMOS spectroscopy of C20 targets
        ├── mmt                         - MMT Blue Channel spectroscopy of C20+C22 targets
        ├── imacs                       - A lone Magellan IMACS spectrum we got to assess the suitability of IMACS 
        └── spectable_resolution.dat    - Upper limits on the resolution of each spectrum 

