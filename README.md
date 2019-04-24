# Gorram shiny! An accessible interface for reproducible landscape archaeology with `R` and `fieldwalkr`
Joe Roe <<jwg983@hum.ku.dk>>  
Centre for the Study of Early Agricultural Societies, University of Copenhagen

This is the source repository for slides presented at CAA 2019, Kraków, 23–27 April.
The slides are an interactive RMarkdown document using ioslides and shiny widgets.
You can view a live version at **https://joeroe.shinyapps.io/caa2019_fieldwalkr/**.
Alternatively, the slides can be run locally using RStudio; see instructions below.

## Abstract


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
