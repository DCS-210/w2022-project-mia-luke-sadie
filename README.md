Project title
================
by Team name

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.4     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   2.0.1     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

## Summary

Squirrels are often thought of as synonymous with New York City. Every
now and then, a new photo of a squirrel eating a slice of pizza will
circulate the internet, linking two of New York City’s icons together.
Although these creatures seem to be lurking in every tree, sidewalk, and
dark corner of New York City, what do we really know about them? We know
they climb trees, are chased by our dogs, and have bushy tails, but what
else can we learn about this NYC community? In our preliminary research
for this project, we stumbled upon a dataset called the New York City
Squirrel Census, and our curiosity about the cute, furry, rodents was
triggered.  
This project takes a look into the New York City squirrel population and
the factors involved in maintaining and changing numbers. We hope to
explore the influences on the NYC squirrel population in the way that
they interact with Central Park. Is there a correlation between the
squirrel population of a given hectare of the park and the environment
in which they inhabit? Or the noises that they make in relation to the
day of week? Our study attempts to answer a multitude of questions
related to the connections between squirrel behaviors and other factors.
This data comes from the New York City Squirrel Census, which is a raw
NY data file. The data was collected by a group of volunteers led by
Jamie Allen, a humorist and writer, with the hopes of tracking the
Eastern gray (Sciurus carolinensis) population in New York. When
compiling the total census population, they employed a divide and
conquer method, dividing Central Park into 350 hectares. Then, the
volunteers spread out and counted and observed squirrels once in the
morning and once at night. They then calculated the total number of
squirrels by using a formula developed by Vagn Flyger, a squirrel
biologist. There are many inherent limitations to our dataset. The
squirrel census is citizen reported, which leaves room for many count
errors and identification issues. This dataset is also centered in
Central Park which only gives us a sample of data from a single area
versus the whole of New York, or even a range of boroughs. The behavior
exhibited by squirrels in Central Park could very well differ from
behaviors exhibited in Prospect Park. Also, we don’t have significant
information on who is collecting the data, other than that they are
volunteering to count squirrels, so we have to make assumptions about
their effectiveness in data collection (i.e. are these kids? retirees?
squirrel fanatics?). In addition to that, many of the data points are
assumptions — how professional were these data collectors in recognizing
what sound the squirrel was making? And were there other sounds
happening in the park that might’ve masked the true noise the squirrel
was making? We created a number of bar graphs and pie charts to
understand the relationship between different behaviors. We created
faceted bar plots to understand how whether it was a weekend or weekday
influenced squirrel behaviors, and whether the morning or afternoon
affected squirrel behavior. We found that squirrels behaved generally
the same whether it was the weekend or weekday, and whether it was
morning or evening. Additionally, we included a number of bar graphs to
show the demographics of squirrels in the park. We found that there was
an overwhelming number of gray squirrels relative to the number of black
and “cinnamon” colored squirrels, and also that the majority of
squirrels were adults. In addition to these demographic visualizations,
we created an animated heat map that showed the density of squirrels
across the park. From this visualization we can gather information on
“squirrel hot spots” within the park. In addition to these maps, we
created leaflets to track the geographical distribution of behaviors and
characteristics of squirrels. We did not find any significant
geographical control in terms of this distribution, and that colors of
fur, noises made, and behaviors exhibited were consistent across all
areas of the park. Our project has limited negative impacts to humans as
this data is solely representative of squirrel population and its
composition rather than impacts on humans. We find it improbable that
the publishing of this data because this data can not be used to profile
an individual or be used to unfairly restrict access. We hope that our
analysis will only benefit others, as it provides interesting but rather
obscure information on the squirrel population. The only potential
negative impact we can think of is further scaring individuals who are
afraid of squirrels. We had a few suggestions on how we could improve
our research and the data set to better understand how the squirrels in
Central Park behave. One of the things that we neglected to take into
account in our investigation into the squirrel behavior in Central Park
was human activity and location. If we were to look into how human
activity was distributed over central park this might lead to greater
insights about squirrel distribution and behavior. We also think that
the heat map could have been better configured to show a more true
display of density, as the colors are on a continuous scale and they are
all fairly close (ranging from 1-20). Our greatest issue was the overall
gathering of data for this project. For one, we recognized that all of
this data is human collected and therefore very prone to error. As the
majority of this data set is descriptive behavior and subjective, it is
important to note that there is possible error within our
visualizations. For instance it is highly possible that a “kuk” sound
could have been recorded as a “quaa” or a “moan”, because quite honestly
they all sound quite similar to the average person! As well the size of
central park, with the limited number of volunteers presents another
issue - who really knows if all the squirrels in central park were
counted? While this is a citizen’s best guess, the number of squirrels
in central park is constantly in flux, making our project a better
representation of a point in time rather than squirrel patterns over
many years. Our data was as well collected over a short period of time,
three weeks, rather than a longitudinal survey, spanning years, that
might result in more accuracy.

You can also load your data here and present any analysis results /
plots, but I strongly urge you to keep that to a minimum (maybe only the
most important graphic, if you have one you can choose). And make sure
to hide your code with `echo = FALSE` unless the point you are trying to
make is about the code itself. Your results with proper output and
graphics go in your presentation, this space is for a brief summary of
your project.

    ## No vignettes or demos or help files found with alias or concept or
    ## title matching 'nyc_squirrels' using regular expression matching.

    ## Rows: 3023 Columns: 36

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (14): unique_squirrel_id, hectare, shift, age, primary_fur_color, highli...
    ## dbl  (9): long, lat, date, hectare_squirrel_number, zip_codes, community_dis...
    ## lgl (13): running, chasing, climbing, eating, foraging, kuks, quaas, moans, ...

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

## Presentation

Our presentation can be found [here](presentation/presentation.html).

## Data

NYC Open Data, NYC Squirrel Census. “2018 Central Park Squirrel Census -
Squirrel Data” Accessed March 14, 2022,
<https://data.cityofnewyork.us/Environment/2018-Central-Park-Squirrel-Census-Squirrel-Data/vfnx-vebw>

## References

List any references here. You should, at a minimum, list your data
source.
