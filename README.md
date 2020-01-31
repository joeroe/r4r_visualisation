# R for Archaeologists: Visualisation

<!-- badges: start -->
<!-- badges: end -->

This repository contains the slides and source code for a workshop on visualisation in R, part of the 'R for Archaeologists' (R4R) winter school held at the University of Pisa, 27th January – 7th February 2020.

The slides use `remark.js` and are generated from an RMarkdown file using the [`xaringan`](https://github.com/yihui/xaringan) package. 
You may find it useful to look at the RMarkdown file to see the R code for some of the examples.

## How to view the slides

### In RStudio

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) or download this repository from GitHub and open `r4r_2020_visualisation.Rproj` in RStudio.

Make sure you have the following packages installed:

```r
install.packages(c("tidyverse", "scales", "rcarbon", "sf", "rnaturalearth", "tidygraph", "ggraph", "remotes"))
remotes::install_github("rstudio/gt")
remotes::install_github("joeroe/stratigraph")
```

You should then be able to open `r4r_2020_visualisation_slides.Rmd` in RStudio and view the slides using the "knit" button at the top of the editor pane or `knitr::knit("r4r_2020_visualisation_slides.Rmd")`.

Press `c` in the presentation window to view the speaker notes.

### In a browser

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) or download this repository from GitHub and open `r4r_2020_visualisation_slides.html` in a browser to view the pre-knit slides.

Press `c` in the presentation window to view the speaker notes.

### As a PDF

This repository also contains a PDF version of the slides [`r4r_2020_visualisation_slides.pdf`](r4r_2020_visualisation_slides.pdf), but this may contain formatting errors and does not include the speaker notes.