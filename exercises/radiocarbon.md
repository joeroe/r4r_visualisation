---
title: 'R4Rchaeologists: Advanced visualisation exercises'
subtitle: 'Exercise B: radiocarbon data'
output: pdf_document
---

Basic visualisation of radiocarbon data in R is fairly straightforward using the skills in data manipulation and visualisation we have learned so far.
`c14bazAAR` offers a convenient interface for retrieving dates from a large number of published datasets,
and there are several packages available for calibration (e.g. `rcarbon`, `Bchron`).
The key is then to transform the calibrated dates to a 'tidy' format suitable for use with `ggplot2`.

Your objectives for this exercise are to:

1. Read radiocarbon data into R
2. Calibrate a set of radiocarbon dates
3. Plot the calibrated dates
4. Produce a faceted plot of calibrated dates by site

## Data

* Use [c14bazAAR](https://docs.ropensci.org/c14bazAAR/) to download radiocarbon dates from a region of your choice.

## R packages and functions

The following packages will be useful for this exercise:

* c14bazAAR*
* stratigraphr (`c14_calibrate()`)*
* dplyr
* ggplot2
* ggridges

\* These packages are not on CRAN. You will need to install them with `devtools::install_github()`

Remember that you can open the documentation for any function with `?function_name()`. 
Google is also your friend – most packages have websites or GitHub repositories with extended documentation.
There are also many tutorials and StackOverflow questions about common problems in R.

## Hints

* You will probably need to filter the data to 20–30 dates from 2–3 dates to get a manageable plot.
* Calibrated dates are not immediately in a format that ggplot2 can understand.
  You will need to use `unnest()` from dplyr.
* The dates can be seperated within the plot using either facets or `ggridges` – why might you use one or the other?