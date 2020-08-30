---
title: "Map Using Leaflet"
author: "Rajashree Ghosh"
date: "19 April 2020"
output:
  ioslides_presentation: default
  beamer_presentation: default
  slidy_presentation: default
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

##Maps using Leaflet

**MAP 1**

```{r,echo=FALSE}
library(leaflet)
my_map<-leaflet()  %>%
  addTiles() %>%
  addMarkers(lat=22.478730,lng=88.375890,popup = "*Aradhana Appartment*")
my_map
```

##Adding many Markers

**MAP 2**


```{r,echo=FALSE}
set.seed(2020-04-19)
df<-data.frame(lat=runif(20,min=22,max=23),
               lng=runif(20,min=88,max=89))
df %>%
  leaflet() %>%
  addTiles() %>%
  addMarkers()
```

##LAST SLIDE

**THANK YOu**