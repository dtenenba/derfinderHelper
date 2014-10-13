derfinderHelper [![Build Status](https://travis-ci.org/lcolladotor/derfinderHelper.svg?branch=master)](https://travis-ci.org/lcolladotor/derfinderHelper)
===============

Helper package for [derfinder](https://github.com/lcolladotor/derfinder).

# Installation instructions

Get R 3.1.1 or newer from [CRAN](http://cran.r-project.org/).

```R
## If needed
install.packages('devtools')

## Pre-requisites from CRAN
install.packages('Matrix', 'testthat', 'knitr', 'knitrBoostrap', 'rmarkdown')

## Pre-requisites from Bioconductor
source('http://bioconductor.org/biocLite.R')
biocLite(c('IRanges', 'S4Vectors'))

## derfinderHelper itself
library('devtools')
install_github('lcolladotor/derfinderHelper')
```

# Vignette

The vignette for this package can be viewed [here](http://lcolladotor.github.io/derfinderHelper/). If you want to re-build the vignette when installing this package, you will need to use:

```R
## Install building the vignette
install_github('lcolladotor/derfinderHelper', build_vignettes = TRUE)
```

Note that this can take longer than installing the package without the vignette.


# Citation

Use [derfinder's citation](https://github.com/lcolladotor/derfinder#citation) information.


## Travis CI

This package is automatically tested thanks to [Travis CI](travis-ci.org) and [r-travis](https://github.com/craigcitro/r-travis). If you want to add this to your own package use:

```R
## Use devtools to create the .travis.yml file
library('devtools')
use_travis('yourPackage')

## Read https://github.com/craigcitro/r-travis/wiki to configure .travis.yml appropriately

## Add a status image by following the info at http://docs.travis-ci.com/user/status-images/
```
