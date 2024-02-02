
<!-- README.md is generated from README.Rmd. Please edit that file -->

# fmr

<!-- badges: start -->
<!-- badges: end -->

The goal of {fmr} is to:

- Establish R-connection to Fisheries Technology Management (FTM) Oracle
  database
- Provide convenient functions to FTM tables and views
- Provide Rmarkdown report templates for various standardized reports
- R-code examples for data analysis and graphical presentations

## Quick start

``` r
remotes::install_github("einarhjorleifsson/fmr")
```

``` r
library(fmr)
library(tidyverse)
key <- "your FM API key"
```

``` r
fm_survey(key) |> glimpse()
#> Rows: 2,277
#> Columns: 5
#> $ site      <chr> "Basseterre West", "Basseterre West", "Basseterre West", "Ba…
#> $ island    <chr> "Saint Kitts", "Saint Kitts", "Saint Kitts", "Saint Kitts", …
#> $ date      <date> 2023-01-05, 2023-01-09, 2023-01-12, 2023-01-08, 2023-01-08,…
#> $ time      <dttm> 2023-01-05 10:00:00, 2023-01-09 10:00:00, 2023-01-12 10:00:…
#> $ survey_id <int> 1478, 1484, 1489, 1492, 1495, 1497, 1500, 1502, 1503, 1505, …
```
