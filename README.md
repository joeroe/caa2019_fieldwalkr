# Gorram shiny! An accessible interface for reproducible landscape archaeology with `R` and `fieldwalkr`
Joe Roe <<jwg983@hum.ku.dk>>  
Centre for the Study of Early Agricultural Societies, University of Copenhagen

This is the source repository for slides presented at CAA 2019, Kraków, 23–27 April.
The slides are an interactive RMarkdown document using ioslides and shiny widgets.
You can view a live version at **https://joeroe.shinyapps.io/caa2019_fieldwalkr/**.
Alternatively, the slides can be run locally using RStudio; see instructions below.

## Abstract

Reproducibility is one of the driving concerns behind the recent adoption of R as an archaeological tool. However, the computational skills needed to actually conduct reproducible research in R are a "rarity" amongst archaeologists (Marwick 2017). Moreover, *computational* reproducibility comes only at the very end of the research process. Computational archaeologists are therefore presented with two challenges. How can we take reproducibility beyond our computers and into the field? And how can we get our tools into the hands of non-specialists? I will demonstrate a new package which I hope makes progress on both these problems. `fieldwalkr` (<https://github.com/joeroe/fieldwalkr>) is an R package for spatial sampling and survey simulation. It includes tools for simulating the effect of different sample frames, sampling strategies and detection functions on the estimation of spatial point patterns. It promotes reproducible field research by facilitating more informed and statistically rigorous survey designs, and as a framework for the theoretical analysis of sampling effects. In this paper, I will focus particularly on the development of a graphical user interface for the package. Built using `shiny`, this alternative interface makes the package more accessible to a wider range of users. At the same time, the core benefits of a scripted tool are maintained by running `fieldwalkr` 'under the hood'. I will suggest that developing tools that are as accessible to as many other researchers as possible is the most impactful contribution computational specialists can make to improving the reproducibility of archaeological research as a whole.

## Run slides locally via RStudio

To view the slides locally, you will first need to clone or download this repository, and make you have all the following packages are installed:

```{r}
# fieldwalkr package
devtools::install_github("joeroe/fieldwalkr")

# CRAN dependencies
install.packages(c("tidyverse", "magrittr", "sf", "maptools", "RandomFields", "RandomFieldsUtils", "spatstat"))
```

Then simply open `caa2019_fieldwalkr.Rmd` in RStudio and click "Run Presentation" above the editing window.
RStudio will knit the document and start a local server to view it.
