# sortLines Addin for RStudio

Sort selected lines in RStudio's editor with this addin.

Credits to Gregory R. Warnes for the sort algorithm from [gtools](https://cran.r-project.org/web/packages/gtools/index.html), which is "number-smart".

# How to install

First, install `devtools` if you don't have it yet. Then use `install_github`:
```r
install.packages("devtools")
library(devtools)
install_github('dcomtois/RStudioAddinsDC')
```
# About the package name
For now, only the sortLines Addin is included, but I might write other Addins in the future. That's why I gave it a generic name. 
