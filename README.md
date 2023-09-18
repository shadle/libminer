
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer is to provide an overview of your R library setup.
It is a toy package created as part of a workshop.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("shadle/libminer")
```

## Example

To get a count of installed packages in each of your libraries,
optionally with the total sizes, use `lib_summary()`:

``` r
library(libminer)

lib_summary()
#>                                                                   Library
#> 1               C:/Users/jshadle/AppData/Local/Programs/R/R-4.3.1/library
#> 2 C:/Users/jshadle/AppData/Local/Temp/Rtmpe48qyA/temp_libpatha1846ad110af
#>   n_packages
#> 1        339
#> 2          1
# specify sizes = TRUE
lib_summary(sizes = TRUE)
#>                                                                   Library
#> 1               C:/Users/jshadle/AppData/Local/Programs/R/R-4.3.1/library
#> 2 C:/Users/jshadle/AppData/Local/Temp/Rtmpe48qyA/temp_libpatha1846ad110af
#>   n_packages  lib_size
#> 1        339 970592467
#> 2          1     17301
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
