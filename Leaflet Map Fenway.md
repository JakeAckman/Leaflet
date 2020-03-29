---
title: "Leaflet Map Fenway"
author: "Jake Ackman"
date: "3/29/2020"
output:
  html_document: default
  pdf_document: default
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## R Markdown

Below is the location of Fenway Park, one of America's most iconic baseball stadiums.

```{r echo = TRUE}
library(leaflet)
     
my_map <- leaflet() %>% addTiles()
     
my_map <- addMarkers(my_map, lat = 42.3467, lng = -71.0972, popup = "Fenway Park")
     
my_map
```