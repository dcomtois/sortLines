# Addins for RStudio

## sortLines (Ascending) or (Descending)

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
install_github('dcomtois/sortLines')
```

That's it. RStudio will recognize it as an addin and it will show up in the Addins menu.

### Usage

Say you have the following lines in your editor, and want them sorted according to the numerical values in the numbering.

```
1. Some text
10. And again
100. And again
2. Still some text
```

Selecting those lines and go to Addins > Sort Selected Lines (A). You'll now have:

```
1. Some text
2. Still some text
10. And again
100. And again
```

### Possible variations

The `gtools::mixedsort` function supports roman numbers sorting; if there is a need for it, it would be easy to add this variation to the existing (A) and (D). 

## About the package
For now, only the sortLines addin is included, but I might write other addins in the future.
