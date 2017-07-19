---
date: 2016-04-23T15:21:22+02:00
title: High-performance R
type: homepage
menu: main
weight: 0
---

R is not a fast language. But we can make it faster. 
This tutorial covers a number of techniques we can use to parallelize and speed 
up our code.
A lot of the material is borrowed from Hadley Wickham's 
"[Advanced R](http://adv-r.had.co.nz/)" book.

In particular, this workshop combines a review of basic R syntax 
(making sure everyone is up to speed) with more advanced R concepts. 
Topics covered include the following:

* Basic R syntax
* Doing work with the "tidyverse" packages
* Common performance optimizations
* Parallelization with `doParallel` and `plyr`
* Parallelization of `dplyr` using `multidplyr`
* Serial farming strategies
* Writing executable R scripts with `argparse`

## Setup

Before you start, make sure you have both [R](https://www.r-project.org/) and 
[RStudio](https://www.rstudio.com/) installed and ready to go. 

You may also wish to install the [tidyverse](http://tidyverse.org/) packages
with `install.packages("tidyverse")` beforehand. We'll be using them a lot.

