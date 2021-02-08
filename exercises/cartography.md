---
title: 'R4Rchaeologists: Advanced visualisation exercises'
subtitle: 'Exercise A: Cartography'
output: pdf_document
---

R has extensive support for vector and raster spatial data (using `sf` and `raster` respectively).
`ggplot2` and its extensions allow you to use this data to produce maps and other spatial visualisations.
Cartography in R differs from a GIS in that you need to do it programmatically, but this opens up the possibility of generating multiple data-driven maps in a way that can be difficult to replicate in point-and-click GIS software.

Your objectives for this exercise are to:

1. Read vector spatial data into R
2. Plot the data using ggplot2
3. Use categorical data to produce a faceted map
4. Add suitable base maps and cartographic elements (e.g. scale, legend)

## Data

* `cartography_data/tavo-a27.tsv` (from <https://github.com/joeroe/tavo-a27>): a table of archaeological sites with coordinates, periods, and species occurrence data
* <https://naturalearthdata.com> for generic base map data

## R packages and functions

The following packages will be useful for this exercise:

* `ggplot2`
* `dplyr`
* `ggspatial`
* `tidyr`
* `stringr`

\* These packages are not on CRAN. You will need to install them with `devtools::install_github()`

Remember that you can open the documentation for any function with `?function_name()`. 
Google is also your friend – most packages have websites or GitHub repositories with extended documentation.
There are also many tutorials and StackOverflow questions about common problems in R.

## Hints

* You can facet the map with either the period or occurrence columns, but both will require some transformation:
  * For occurrences, see `?tidyr::pivot_longer`
  * For periods, see `?stringr::str_split` and `?tidyr::pivot_longer`
* Apart from Natural Earth data, there are R packages that provide base maps directly (e.g. `maptools`, `ggmap`)
