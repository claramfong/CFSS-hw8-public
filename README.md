# Homework 8: Collecting and analyzing data from the web

The purpose of this assignment was to practice collecting data from the web using APIs. This was divided into two assignments: "plug and play" packages (which was the `gapminder` assignment) or using our own method of attempting to build the data frame from scratch. 

1. Practicing "plug and play" packages, which we used `libary(geonames)` for the [gapminder](gapminder.Rmd) assignment, and,

2. An independent assignment, where I chose to build a data frame from New York Times' API (linked [here](nyt.Rmd)). Note: I found a package called `rtimes`, which is documented in both the .md and .Rmd files, but I decided to practice building the query and function from scratch using the `httr::GET()` function.

More details about the assignment can be found [here](https://cfss.uchicago.edu/homework/webdata/).

## Files in Repository

In this repository, you will find four relevant files:

1. Part One Files:
  - The [gapminder Rmarkdown file](gapminder.Rmd), and
  - The corresponding [report](gapminder.md) generated from Rmarkdown
  
2. Part Two Files:
  - The [new york times Rmarkdown file](nyt.Rmd) that built the data frame from the NYT API, and
  - The corresponding [report](nyt.md) generated from Rmarkdown, which consists of preiminary exploratory analysis and one statistical model
  
## Packages Used

```{r}
# For gapminder file
library(tidyverse)
library(geonames)
library(here)
library(countrycode)
library(tidymodels)

# For nyt file
library(tidyverse)
library(stringr)
library(httr)
library(jsonlite)
library(lubridate)
library(ggplot2)
library(tidyr)
library(tidymodels)
```