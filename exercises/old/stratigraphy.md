---
title: 'R4Rchaeologists: Advanced visualisation exercises'
subtitle: 'Exercise C: Stratigraphy'
output: pdf_document
---

Stratigraphic data is usually presented in section plans or a 'Harris matrix'.
Unfortunately, neither of these formats make it easy to incorporate the data into further analyses in R.
My package `stratigraphr` (in development) offers a means of reading stratigraphic data into R as a network graph.
This allows us to manipulate and visualising it with the packages `tidygraph` and `ggraph`.

Your objectives for this exercise are to:

1. Transcribe stratigraphic data in a format that you can read into R 
2. Use the data to produce a 'stratigraphic graph'
3. Reproduce the traditional Harris matrix as an R plot
4. Experiment with other ways of presenting this data using `ggraph`

## Data

* `stratigraphy_data/strat.docx` – a section plan and Harris matrix

## R packages and functions

The following packages will be useful for this exercise:

* `stratigraphr`*
* `tidygraph`
* `ggraph`

\* These packages are not on CRAN. You will need to install them with `devtools::install_github()`

Remember that you can open the documentation for any function with `?function_name()`. 
Google is also your friend – most packages have websites or GitHub repositories with extended documentation.
There are also many tutorials and StackOverflow questions about common problems in R.

## Hints

* For objective 4, think about alternative visualisations that could, for example, expose the clustering or node centrality of stratigraphic units better than the Harris matrix.
