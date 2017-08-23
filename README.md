# r-data-science

A set of online lesson materials for Sudo's "Data Science with R" workshop.
This is an R Markdown website built with the [blogdown](https://github.com/rstudio/blogdown) package.

The website is hosted at https://sudo-labs.github.io/r-data-science/.

## Building the website

Before you build anything, make sure you've got the following dependencies installed:

Install R from https://www.r-project.org/. 
If on Windows, install [RTools](https://cran.r-project.org/bin/windows/Rtools/) as well (might not be required, not sure though).

Open R and install the following packages used in the lessons:

```{r}
install.packages(c("tidyverse", "pryr", "nycflights13", "gapminder", "devtools"))
```

The `blogdown` package is not in the official R package repositories yet, so we'll install it using `devtools`.
If something's not working quite right, you can re-run this command to update to the latest development version as well.

```{r}
devtools::install_github('rstudio/blogdown')
```

### Building the website

Run `Rscript -e 'blogdown::serve_site()'` on the command line. 
The website will build and a browser window should open at the local development site.

### Publishing changes

To push changes to the Github site, rebuild the website, commit changes to the `gh-pages` branch, and push to Github.
The website should update within a couple minutes.
CSS changes might require you to make a commit to a file (even just adding a blank line at the end) before they take effect.

## How the site works

The files in the `content/` folder contain the actual site content and are probably what you want to edit. 
Files here can be either Markdown or R Markdown, and will be rendered when you run `blogdown::serve_site()` in R.
For a quick guide to R Markdown, either check out the [lesson materials themselves](https://sudo-labs.github.io/r-data-science/rmarkdown/)
or check out RStudio's [cheat sheet](https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf).
Any files you want to link to (that aren't online or otherwise produced by R) should be placed in the `static/` directory.
The rendered website is created in the `docs/` folder and is what gets served by Github.

The themes and CSS are provided by [hugo-alabaster-theme](https://github.com/digitalcraftsman/hugo-alabaster-theme) in the `themes/` directory.
Any theming changes should be made here. 
Alternatively, you can swap out this theme with another one from https://themes.gohugo.io/
