# pkgcheck-editor-extra

<!-- badges: start -->

[![R build
status](https://github.com/ropensci-review-tools/pkgcheck-editor-extra/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/ropensci-review-tools/pkgcheck-editor-extra/actions?query=workflow%3AR-CMD-check.yaml)
[![codecov](https://codecov.io/gh/ropensci-review-tools/pkgcheck-editor-extra/branch/main/graph/badge.svg)](https://codecov.io/gh/ropensci-review-tools/pkgcheck-editor-extra)
[![Project Status:
Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: end -->

Check whether a package is ready for submission to
[rOpenSci](https://ropensci.org)’s peer review system. The primary
function collates the output of
[`goodpractice`](https://github.com/ropensci-review-tools/goodpractice),
including `R CMD check` results, a number of statistics via the
[`pkgstats` package](https://github.com/ropensci-review-tools/pkgstats),
and checks for package structure expected for rOpenSci submissions. The
output of this function immediately indicates whether or not a package
is “Ready to Submit”.

## Installation

The easiest way to install this package is via the [associated
`r-universe`](https://ropensci-review-tools.r-universe.dev/ui#builds).
As shown there, simply enable the universe with

``` r
options (repos = c (
    ropenscireviewtools = "https://ropensci-review-tools.r-universe.dev",
    CRAN = "https://cloud.r-project.org"
))
```

And then install the usual way with,

``` r
install.packages ("pkgcheckEditorExtra")
```

Alternatively, the package can be installed by first installing either
the [remotes](https://remotes.r-lib.org) or
[pak](https://pak.r-lib.org/) packages and running one of the following
lines:

``` r
remotes::install_github ("ropensci-review-tools/pkgcheck-editor-extra")
pak::pkg_install ("ropensci-review-tools/pkgcheck-editor-extra")
```

The package can then loaded for use with

``` r
library (pkgcheckEditorExtra)
```

## Code of Conduct

Please note that this package is released with a [Contributor Code of
Conduct](https://ropensci.org/code-of-conduct/). By contributing to this
project, you agree to abide by its terms.
