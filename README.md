
`mgrs` : Convert 'MGRS' Coordinates To and From Other Coordiante Systems

NOTE: These will be vectorized soon.

The following functions are implemented:

-   `latlng_to_mgrs`: Convert latitude/longitude to MGRS string
-   `mgrs_to_latlng`: Convert an MGRS string to latitude/longitude

### Installation

``` r
devtools::install_github("hrbrmstr/mgrs")
```

### Usage

``` r
library(mgrs)

# current verison
packageVersion("mgrs")
```

    ## [1] '0.1.0'

``` r
mgrs_to_latlng("33UXP04")
```

    ##      lat      lng 
    ## 48.20535 16.34593

``` r
latlng_to_mgrs(48.20535, 16.34593)
```

    ## [1] "33UXP0000040000"

``` r
mgrs_to_latlng("33UXP0500444996")
```

    ##      lat      lng 
    ## 48.24947 16.41449

``` r
latlng_to_mgrs(48.24948, 16.41449)
```

    ## [1] "33UXP0500344996"

``` r
mgrs_to_latlng("24XWT783908")
```

    ##       lat       lng 
    ##  83.62738 -32.66879

``` r
latlng_to_mgrs(83.62738, -32.66879)
```

    ## [1] "25XEN0410486507"