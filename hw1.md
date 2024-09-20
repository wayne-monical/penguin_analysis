HW 1
================
Wayne Monical
2024-09-20

Here we load the `penguins` data set from the `palmerpenguins` package.

``` r
data("penguins", package = "palmerpenguins")
```

This data set comes in the form of a data frame. It contains data on
three different penguin `species`, Adelie, Gentoo, and Chinstrap. The
penguins range over three different islands, Torgersen, Biscoe, and
Dream, given by the `island` variable. Observations come over three
years, 2007 through 2009, given by the `year` variable.

The data describes 344 penguin individuals in a total of 8 variables.
The data includes various physical measures of the penguins, such as
their flipper length in millimeters, given by the `flipper_length_mm`
variable. This variable has an average value of 200.92 in this data set.

``` r
print(unique(penguins$species))
```

    ## [1] Adelie    Gentoo    Chinstrap
    ## Levels: Adelie Chinstrap Gentoo

``` r
print(unique(penguins$island))
```

    ## [1] Torgersen Biscoe    Dream    
    ## Levels: Biscoe Dream Torgersen

``` r
print(unique(penguins$year))
```

    ## [1] 2007 2008 2009

``` r
nrow(penguins)
```

    ## [1] 344

``` r
head(penguins)
```

    ## # A tibble: 6 × 8
    ##   species island    bill_length_mm bill_depth_mm flipper_length_mm body_mass_g
    ##   <fct>   <fct>              <dbl>         <dbl>             <int>       <int>
    ## 1 Adelie  Torgersen           39.1          18.7               181        3750
    ## 2 Adelie  Torgersen           39.5          17.4               186        3800
    ## 3 Adelie  Torgersen           40.3          18                 195        3250
    ## 4 Adelie  Torgersen           NA            NA                  NA          NA
    ## 5 Adelie  Torgersen           36.7          19.3               193        3450
    ## 6 Adelie  Torgersen           39.3          20.6               190        3650
    ## # ℹ 2 more variables: sex <fct>, year <int>
