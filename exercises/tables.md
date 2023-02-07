---
title: 'R4Rchaeologists: Advanced visualisation exercises'
subtitle: 'Exercise C: tables'
output: pdf_document
---

Tables are often overlooked as a visualisation – but they are one!
Tufte (1983), for example, recommends tables as the most effective way to visualise small datasets, and/or when it is useful to compare exact values.
As a rule of thumb, if you find yourself making a bar chart with or worse, a pie chart, consider whether the data would be better presented in a table.

[gt](https://github.com/rstudio/gt) provides a ggplot-inspired grammar for tables that makes it possible to make sophisticated and publication-ready tables in R.

Your objectives for this exercise are to:

1. Display the `RBPottery` dataset (from `archdata`) in a table
2. Apply appropriate grouping and formatting
3. Add metadata (title, subtitle, caption and footnotes), including highlighting suspicious values (see `?RBPottery`)

## Data

* `archdata::RBPottery`

## R packages and functions

The following packages will be useful for this exercise:

* gt
* dplyr

Remember that you can open the documentation for any function with `?function_name()`. 
Google is also your friend – most packages have websites or GitHub repositories with extended documentation.
There are also many tutorials and StackOverflow questions about common problems in R.

## Hints

* Like ggplot, gt works best with 'tidy' data. You will need to do some tidying of the RBPottery dataset first.
* Look at the documentation for the `RBPottery` dataset first, to understand what it is and where it comes from.