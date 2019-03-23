## Addin for RStudio:
# sortLines (Ascending) or (Descending)

Sort selected lines in RStudio's editor with this addin.

Credits to Gregory R. Warnes for the sort algorithm from [gtools](https://cran.r-project.org/web/packages/gtools/index.html), which is "number-smart". 

## How to install

#### Recommended Method : addinslist  

If you don't have [addinslist](https://github.com/daattali/addinslist) installed, I recommend you do install it, 
as it gives access to a multitude of useful addins through a simple GUI.

```r
install.packages('addinslist')
```

Then, refer to the [addinslist](https://github.com/daattali/addinslist) documentation to proceed and install `sortLines`.

#### Alternative Method : devtools or remotes  

**Using `devtools`**

If you have `devtools` installed, use

```r
devtools::install_github('dcomtois/sortLines')
```

**Using `remotes`**

If you don't have nor need the functionalities of `devtools`, install the lightweight
[remotes](https://github.com/r-lib/remotes) and use it to install `sortLines`:

```r
install.packages("remotes")
remotes::install_github("dcomtois/sortLines")
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

