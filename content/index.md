---
title: High-performance R
type: homepage
menu: main
weight: 1
---

Although R is probably not the fastest language ever made, 
it sees a lot of use in scientific and data analysis applications.
This tutorial focus on a number of techniques we can use to parallelize and speed 
up our code, in addition to a couple other useful techniques we can use in our work. 

In particular, these materials combine a review of basic R syntax 
and concepts with more advanced performance-related content. 
The goal of this format is two-fold:
we want to make sure everyone is on the same page,
and it ensures a relatively logical progression of concepts 
(the alternative is to have two distinct lessons, 
and have the difficulty level go from 0 to 9000 real fast).
Hopefully these materials will be useful for R users of all levels.

Topics covered include the following:

* Basic R syntax and concepts
* Doing work with the "tidyverse" packages (`dplyr`, `purrr`, `ggplot2`)
* Measuring code performance
* Common performance optimizations
* Parallelization with `doParallel`, `plyr`, and `multidplyr`

## Setup

Before you start, make sure you have both [R](https://www.r-project.org/) and 
[RStudio](https://www.rstudio.com/) installed and ready to go. 

You may also wish to install the [tidyverse](http://tidyverse.org/) packages
with `install.packages("tidyverse")` beforehand. We'll be using them a lot.

## Credits

Giving credit where credit is due, 
these materials borrow liberally from
Software Carpentry's [R for Reproducible Science](https://swcarpentry.github.io/r-novice-gapminder/) workshop 
as well as a lot of concepts from 
Hadley Wickham's "[Advanced R](http://adv-r.had.co.nz/)" book.

# [Get started](./basics/)
