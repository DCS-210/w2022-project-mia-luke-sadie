Project proposal
================
Team name

``` r
library(tidyverse)
library(broom)
```

## 1. Introduction

In this project, we will be using a dataset from “Freedom in the World”
- Freedom House’s flagship publication to analyze trends in global
political rights and civil liberties. The data we are using comes from
tidytuesday an open data source. The dataset has been published annually
since 1972 up until today and contains the survey ratings and narrative
reports on 195 countries and 15 related and disputed territories. This
dataset, which tracks individual availability to obtain freedom, is used
by policymakers, the media, international corporations, civic activists,
and human rights defenders to argue for change. We attempt to examine
the question of *how national political freedoms change comparatively
over time and why this is so*.

The survey data is broken down into multiple categories including
guaranteed civil liberties, guaranteed political rights, status of
individuals, and the development status of the country in question.
Freedom House has written about their index - notably an article in 2018
on \[“Democracy in Crisis”\]
(<https://freedomhouse.org/report/freedom-world/2018/democracy-crisis>)
and \[“10 years of Decline in Global Freedom”\]
(<https://freedomhouse.org/article/q-10-years-decline-global-freedom>).
This data will be assessed in conjunction with outside factors to
determine the trajectory of freedom for countries.

The specific questions we want to answer using this data set are:

-   Does the stage of development of a country determine its level of
    political freedoms?
-   How long does it take for a country to obtain political freedom and
    civil liberties? Is this a discernable pattern across nations?
-   What appears to be a limiting factor in achieving political freedom
    and civil liberties?
-   Do the overall amount of countries achieving positive trends in
    civil liberties and political freedom trend positive as time passes?
    Why do we think this is so?
-   Should we be alarmed by these figures?
-   How many countries have experienced a decline in democracy? How many
    countries have experienced an expansion in democracy?

## 2. Data

freedom \<-
readr::read_csv(‘<https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2022/2022-02-22/freedom.csv>’)

## 3. Data analysis plan
