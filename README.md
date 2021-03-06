proj
=======



[![Build Status](https://travis-ci.org/ropensci/proj.svg)](https://travis-ci.org/ropensci/proj)
[![Build status](https://ci.appveyor.com/api/projects/status/kkeuanj6a2badvea?svg=true)](https://ci.appveyor.com/project/sckott/proj)


`proj` is an R wrapper for [proj4js](https://github.com/proj4js/proj4js).

## Install


```r
install.packages("devtools")
devtools::install_github("ropensci/proj")
```


```r
library("proj")
```

## Project


```r
pts <- c(-71,41)
to <- '"+proj=gnom +lat_0=90 +lon_0=0 +x_0=6300000 +y_0=6300000 +ellps=WGS84
   +datum=WGS84 +units=m +no_defs"'
project(pts, to = to)
#> [1] "-637465.7968061864,3911238.9599070395"
```

## Meta

* Please [report any issues or bugs](https://github.com/ropensci/proj/issues).
* License: MIT
* Get citation information for `proj` in R doing `citation(package = 'proj')`

[![rofooter](http://ropensci.org/public_images/github_footer.png)](http://ropensci.org)
