# R for Archaeologists: Visualisation

This repository contains the slides and source code for a workshop on visualisation in R, part of the [R for Archaeologists (R4R) winter school](http://www.mappaproject.org/r4rchaeologists/) held at the University of Pisa on:

* 22nd January – 2nd February 2024
* 30th January – 10th February 2023
* 24th January – 4th February 2022
* 25th January – 5th February 2021
* 27th January – 7th February 2020

The slides use `remark.js` and are generated from an RMarkdown file using the [`xaringan`](https://github.com/yihui/xaringan) package. 
You may find it useful to look at the RMarkdown file to see the R code for some of the examples.

## How to view the slides

### Online

The built slides are available online at <http://joeroe.io/r4r_visualisation/r4r_visualisation_slides.html>.

Press `p` in the presentation window to view the speaker notes and `c` to open a new window.

### In RStudio

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) or download this repository from GitHub and open `r4r_visualisation.Rproj` in RStudio.

Make sure you have the following packages installed:

```r
install.packages(c("tidyverse", "scales", "rcarbon", "sf", "rnaturalearth", "tidygraph", "ggraph", "remotes", "gt", "archdata", "raster", "xaringan", "xaringanthemer"))
remotes::install_github("joeroe/stratigraphr")
remotes::install_github("rstudio/fontawesome")
```

You should then be able to open `r4r_visualisation_slides.Rmd` in RStudio and view the slides using the "knit" button at the top of the editor pane or `knitr::knit("r4r_visualisation_slides.Rmd")`.

Press `p` in the presentation window to view the speaker notes and `c` to open a new window.
