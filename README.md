
<!-- README.md is generated from README.Rmd. Please edit that file -->

# mydesc

<!-- badges: start -->
<!-- badges: end -->

This is a quick demo package to serve as a sort of reprex.

## Installation

You can install the development version of mydesc like so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
```

## Example

You should never reexport `dplyr::desc`. Here’s why:

``` r
df <- data.frame(x = 1:2)
dplyr::arrange(df, dplyr::desc(x))
#>   x
#> 1 2
#> 2 1
dplyr::arrange(df, mydesc::desc(x))
#>   x
#> 1 1
#> 2 2
```
