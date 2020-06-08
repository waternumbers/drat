This is waternumbers CRAN-style repository for authored packages either are either not on CRAN or have been updated since the last CRAN release.

This allows users to install development versions of our software without specialized functions such as install_github(), allows dependencies not hosted on CRAN to still be resolved automatically, and permits the use of update.packages().
Using the repository

To use, simply add waternumbers.github.io/drat to your existing list of R repos, such as:

```r
options(repos = c("https://waternumbers.github.io/drat", getOption("repos"))
```

(If you don’t have any default CRAN mirrors selected yet by getOption("repos"), you may want to add one now). You can also include this line in specific install.packages() requests:

```r
install.packages("dynatop", repos = c("https://waternumbers.github.io/drat", "http://cran.rstudio.com"))
```

To see all the available packages for your system use 

```r
available.packages(contrib.url( "https://waternumbers.github.io/drat/", "both"))[,c("Package","Version")]
```
