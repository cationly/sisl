.. highlight:: python

.. sisl documentation master file, created by
   sphinx-quickstart on Wed Dec  2 19:55:34 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


|buildstatus|_
|pypi|_
|conda|_
|codecov|_
|donate|_


Welcome to sisl's documentation!
==============================

This documentation has been created from version: |release|.

`sisl` is a tool to easily create geometries and, in general, handle
data output files from various DFT codes.
It is particularly developed with SIESTA_ /TranSIESTA_ /TBtrans_ in mind
due to my own development of TranSIESTA_ and TBtrans_.

Secondly it provides an *easy* interface for creating and examining
tight-binding Hamiltonians (dynamical matrices, self-energies, etc.)
using a fast an intuitive Python class.
Any Hamiltonian, from tight-binding or DFT, may be written in to a NetCDF4
file and passed to TBtrans_ for *N*-terminal transport calculations.


Features
--------

* Command line utilities for processing of data files for a wide
  variety of file formats:

  * :ref:`script_sdata`
    Read and transform *any* `sisl` data file. 
    This script is capable of handling geometries, grids, special
    data files such as binary files etc.

  * :ref:`script_sgeom` a geometry conversion tool which reads and writes
    many commonly encounted files for geometries, such as XYZ files etc.
    as well as DFT related input and output files.

  * :ref:`script_sgrid` a real-space grid conversion tool which reads and writes
    many commonly encounted files for real-space grids. *Mainly targetted SIESTA_*.

* Python script which does all the above things *and more*.
  `sisl` implements many classes for manipulating geometries and nano-structure
  related physical quantities, e.g. atomic species, unit-cells (with user-defined periodicity), Hamiltonians (orthogonal and non-orthogonal), real-space grids.



Installation
------------

The easiest way to install `sisl` is via the :program:`pypi` interface.
Install via:

.. code-block:: bash

   pip install sisl

In case you are using `conda` simply do:
   
.. code-block:: bash

   conda install -c zerothi sisl

Alternatively you can download the releases on the
`release page <gh-releases_>`_. And install via the regular :program:`setup.py`
interface:

.. code-block:: bash

   python setup.py install

which will install `sisl` in your default location, use :program:`--prefix <path>` for
manual control of the placement.


Requirements
------------

To succesfully use `sisl` these Python packages must be installed:

 - `six`_
 - `setuptools`_
 - `numpy`_ (`>=1.9`)
 - `scipy`_ 
 - `netcdf4-python`_

Indices and Tables
==================

.. toctree::
   :maxdepth: 3
   :titlesonly:
   :hidden:
   
   scripts/sgeom
   scripts/sgrid
   scripts/sdata

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

Documentation in other themes
=============================

The `sisl` documentation has been created with several different themes
of documentation.
This is mainly of convenience until I have figured out which one is the
best suited theme for this documentation.

If you have any preferences please let me know.

* `Alabaster`_ theme (good)
* `Agogo`_ theme (good)
* `Bizstyle`_ theme (default, good)
* `Classic`_ theme (ok)
* `Scrolls`_ theme (good)
* `Sphinx RTD`_ theme (ok)


.. _Alabaster: ../alabaster/index.html
.. _Agogo: ../agogo/index.html
.. _Bizstyle: ../bizstyle/index.html
.. _Classic: ../classic/index.html
.. _Scrolls: ../scrolls/index.html
.. _Sphinx RTD: ../sphinx_rtd_theme/index.html
.. _gh-releases: http://github.com/zerothi/sisl/releases
.. _pypi-releases: http://pypi.python.org/pypi/sisl/

.. These are external links:
.. _six: https://pypi.python.org/pypi/six
.. _netcdf4-python: http://github.com/Unidata/netcdf4-python
.. _numpy: http://github.com/numpy/numpy
.. _scipy: http://github.com/scipy/scipy
.. _SIESTA: https://departments.icmab.es/leem/siesta/
.. _TranSIESTA: https://launchpad.net/siesta
.. _TBtrans: https://launchpad.net/siesta


.. |buildstatus| image:: https://travis-ci.org/zerothi/sisl.svg
.. _buildstatus: https://travis-ci.org/zerothi/sisl

.. |pypi| image:: https://badge.fury.io/py/sisl.svg
.. _pypi: https://badge.fury.io/py/sisl

.. |conda| image:: https://anaconda.org/zerothi/sisl/badges/installer/conda.svg
.. _conda: https://anaconda.org/zerothi/sisl

.. |codecov| image:: https://codecov.io/gh/zerothi/sisl/branch/master/graph/badge.svg
.. _codecov: https://codecov.io/gh/zerothi/sisl

.. |donate| image:: https://img.shields.io/badge/Donate-PayPal-green.svg
.. _donate: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=NGNU2AA3JXX94&lc=DK&item_name=Papior%2dCodes&item_number=codes&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted
