---
title: 'R4Rchaeologists: Advanced visualisation exercises'
subtitle: 'Exercise D: 3D landscapes'
output: pdf_document
---

3D visualistions are often treated with scepticism – for good reason!
But used careful, they can be an effective way of visualising data, especially when that data has a natural third dimension.
One example of this is landscapes, where the [rayshader](https://github.com/tylermorganwall/rayshader) package can be used to create 3D renders that evoke the work of 20th century cartographers such as Erwin Raisz.

Your objectives for this exercise are to:

1. Create a 3D visualisation of the Razavar Valley (Kermanshah, Iran)
2. Overlay the map with the results of an archaeological survey of the valley 
3. Add appropriate map elements to help readers understand the visualiation

## Data

* `rzvr_e_srtm1v3s.tif` – SRTM 1 arc-second DEM of the Razavar Valley
* `rzvr_streams.png` – raster representation of waterways in the Razavar Valley (aligned to `rzvr_e_srtm1v3s.tif`)
* `rzvr_survey_intensity.png` – estimated of the surveyed area (aligned to `rzvr_e_srtm1v3s.tif`)
* `rzvr_sites.csv` – sites recorded in the survey

## R packages and functions

The following packages will be useful for this exercise:

* rayshader
* raster
* png
* dplyr

Remember that you can open the documentation for any function with `?function_name()`. 
Google is also your friend – most packages have websites or GitHub repositories with extended documentation.
There are also many tutorials and StackOverflow questions about common problems in R.

## Hints

* rayshader has an excellent README
* Experiment with the texture and rayshading options to find a visualisation that matches to the nature of the study region (an arid mountain valley)
* You can use `render_label()` to add the site locations.
* There are several attributes in the sites table that you could use to enrich the visualisation.