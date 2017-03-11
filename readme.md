# Addins for RStudio

## sortLines

Sort selected lines in RStudio's editor with this addin.

Credits to Gregory R. Warnes for the sort algorithm from [gtools](https://cran.r-project.org/web/packages/gtools/index.html), which is "number-smart".

## How to install

First, install `devtools` if you don't have it yet.
```r
install.packages("devtools")
```

To install, use `install_github`:
```r
library(devtools)
install_github('dcomtois/RStudioAddinsDC')
```
## About the package
For now, only the sortLines addin is included, but I might write other addins in the future.
