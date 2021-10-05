Data Manipulation
================

## Import some data

I want to import ‘FAS\_litters.csv’

``` r
litter_df <- read_csv("data/FAS_litters.csv")
```

    ## Rows: 49 Columns: 8

    ## -- Column specification --------------------------------------------------------
    ## Delimiter: ","
    ## chr (2): Group, Litter Number
    ## dbl (6): GD0 weight, GD18 weight, GD of Birth, Pups born alive, Pups dead @ ...

    ## 
    ## i Use `spec()` to retrieve the full column specification for this data.
    ## i Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
litter_df = janitor::clean_names(litter_df)

pups_df <- read_csv("data/FAS_pups.csv")
```

    ## Rows: 313 Columns: 6

    ## -- Column specification --------------------------------------------------------
    ## Delimiter: ","
    ## chr (1): Litter Number
    ## dbl (5): Sex, PD ears, PD eyes, PD pivot, PD walk

    ## 
    ## i Use `spec()` to retrieve the full column specification for this data.
    ## i Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
pups_df = janitor::clean_names(pups_df)
```
