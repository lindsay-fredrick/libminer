
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->

[![R-CMD-check](https://github.com/lindsay-fredrick/libminer/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/lindsay-fredrick/libminer/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of libminer is to provide a summary of a user’s R libraries.
It’s a toy package developed in a workshop and not meant for serious
use.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("lindsay-fredrick/libminer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer)

lib_summary()
#>                                                                    library
#> 1                                       C:/Program Files/R/R-4.2.1/library
#> 2                        C:/Users/lforeste/AppData/Local/R/win-library/4.2
#> 3 C:/Users/lforeste/AppData/Local/Temp/Rtmpewlfsw/temp_libpath517c12e42592
#>   n_packages
#> 1         30
#> 2        172
#> 3          1

# You can also ask it to calculate sizes:
lib_summary(sizes = TRUE)
#>                                                                    library
#> 1                                       C:/Program Files/R/R-4.2.1/library
#> 2                        C:/Users/lforeste/AppData/Local/R/win-library/4.2
#> 3 C:/Users/lforeste/AppData/Local/Temp/Rtmpewlfsw/temp_libpath517c12e42592
#>   n_packages  lib_size
#> 1         30  69711557
#> 2        172 511330907
#> 3          1     13058
```
