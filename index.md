
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![](https://www.r-pkg.org/badges/version-ago/MODIStsp)](http://cran.rstudio.com/web/packages/MODIStsp/index.html) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.290683.svg)](https://doi.org/10.5281/zenodo.290683) [![Downloads](http://cranlogs.r-pkg.org/badges/grand-total/MODIStsp?color=red)](http://cran.rstudio.com/web/packages/MODIStsp/index.html) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Travis-CI Build Status](https://travis-ci.org/lbusett/MODIStsp.svg?branch=master)](https://travis-ci.org/lbusett/MODIStsp) [![Coverage Status](https://img.shields.io/codecov/c/github/lbusett/MODIStsp/master.svg)](https://codecov.io/github/lbusett/MODIStsp?branch=master)

<i class="fa fa-globe" aria-hidden="true"></i> MODIStsp: a "R" package for preprocessing MODIS time series <img src="docs/logo.png" width="147" height="170" align="right" />
=============================================================================================================================================================================

**MODIStsp** is a "R" package devoted to **automatizing the creation of time series of raster images derived from MODIS Land Products data**.

**MODIStsp** allows to perform several preprocessing steps *(e.g., download, mosaicing, reprojection, resize, data extraction)* on MODIS data available within a given time period. Users have the ability to select which specific layers of the original MODIS HDF files they want to process. They also can select which additional **Quality Indicators** should be extracted from the aggregated MODIS Quality Assurance layers and, in the case of Surface Reflectance products, which **Spectral Indexes** should be computed from the original reflectance bands.

All processing parameters can be easily selected with a **powerful and user-friendly GUI**, although non-interactive execution exploiting a previously created Options File is possible. Stand-alone execution outside an "R" environment is also possible, allowing to use scheduled execution of MODIStsp to automatically update time series related to a MODIS product and extent whenever a new image is available.

For each output layer, outputs are saved as **single-band raster** files corresponding to each available acquisition date. **Virtual files** allowing access to the entire time series as a single file can be also created.

*The package is developed and maintained by L.Busetto and L.Ranghetti, from the Institute of Remote Sensing of Environment - National Research Council - Italy ([CNR-IREA](http://www.irea.cnr.it/en/))*

------------------------------------------------------------------------

<i class="fa fa-cog" aria-hidden="true"></i> Getting Started
------------------------------------------------------------

-   To install `MODIStsp`, please follow instructions reported [here](articles/installation.html), both for [<i class="fa fa-windows" aria-hidden="true"></i>](articles/installation.html#installing-on-windows) , [<i class="fa fa-linux" aria-hidden="true"></i>](articles/installation.html#installing-on-linux-systems) and [<i class="fa fa-apple" aria-hidden="true"></i>](articles/installation.html#installing-on-mac)

-   `MODIStsp` can be used either in [interactive mode](articles/interactive_execution.html) exploiting its user-friendly GUI, or in [non-interactive mode](articles/noninteractive_execution.html) from within `R` scripts

-   [Scheduled Processing](articles/noninteractive_execution.html#scheduled-processing) allows automatic updating of MODIS time series through scheduled jobs, both on [<i class="fa fa-windows" aria-hidden="true"></i>](articles/standalone_execution.html#on-windows) and [<i class="fa fa-linux" aria-hidden="true"></i>](articles/standalone_execution.html#on-linux)

-   Solutions to common **installation, data download and processing problems** can be found in our [<i class="fa fa-question-circle-o aria-hidden="true"></i> faq](articles/faq.html)

-   Please **report any issues** you may encounter in our [issues page on github <i class="fa fa-github-square" aria-hidden="true"></i>](https://github.com/lbusett/MODIStsp/issues) .

------------------------------------------------------------------------

<i class="fa fa-newspaper-o" aria-hidden="true"></i> What's New
---------------------------------------------------------------

-   11/08/2017 - MODIStp 1.3.3 was released today. It provides improvements in processing speed, as well as the usual bug fixes. See our [<i class="fa fa-newspaper-o aria-hidden="true"></i> news](news/index.html) page for a detailed changelog. **We thank to all the users that signalled problems for their feedback for imporoving the package!**

------------------------------------------------------------------------

<i class="fa fa-pencil" aria-hidden="true"></i>Citation
-------------------------------------------------------

To cite MODIStsp in publications, please use:

L. Busetto, L. Ranghetti (2016) MODIStsp: An R package for automatic preprocessing of MODIS Land Products time series, Computers & Geosciences, Volume 97, Pages 40-48, ISSN 0098-3004, <https://doi.org/10.1016/j.cageo.2016.08.020>, URL: <https://github.com/lbusett/MODIStsp>.

A BibTeX entry for LaTeX users is:

      @Article{,
        author  = {Lorenzo Busetto and Luigi Ranghetti},
        title   = {MODIStsp: an R package for preprocessing of MODIS Land Products time series},
        journal = {Computers & Geosciences},
        year    = {2016},
        volume  = {97},
        pages   = {40-48},
        issn    = {0098-3004},
        doi     = {10.1016/j.cageo.2016.08.020},
        url     = {https://github.com/lbusett/MODIStsp},
      }
