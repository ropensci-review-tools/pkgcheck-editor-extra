# Contributing to -editor-extra

## Opening issues

The easiest way to note any behavioural curiosities or to request any new
features is by opening a [github
issue](https://github.com/ropensci-review-tools/pkgcheck-editor-extra/issues).


## Development guidelines

If you'd like to contribute changes to `pkgcheck-editor-extra`, we use [the GitHub
flow](https://docs.github.com/en/get-started/quickstart/github-flow) for proposing,
submitting, reviewing, and accepting changes. If you haven't done this before,
there's a nice [overview of git](https://r-pkgs.org/git.html), as well
as [best practices for submitting pull requests](http://r-pkgs.org/git.html#pr-make)
in the R packages book by Hadley Wickham and Jenny Bryan.

The `pkgcheck-editor-extra` coding style diverges somewhat from [the commonly used tidyverse style
guide](https://style.tidyverse.org/syntax.html#spacing), primarily through judicious use of
whitespace, which aims to improve code readability. Code references in
`pkgcheck-editor-extra` are separated by whitespace, just like words of text. Just like it
is easier to understand "these three words" than "thesethreewords", code is not
formatted like this:

``` r
these <- three(words(x))
```
rather like this:

``` r
these <- three (words (x))
```

The position of brackets is then arbitrary, and we could also write

``` r
these <- three( words (x))
```

`pkgcheck-editor-extra` code opts for the former style, with the natural result that one
ends up writing

```r
this <- function ()
```

with a space between `function` and `()`. That's it.

## Adding new checks

New checks are a welcome contribution to `pkgcheck-editor-extra`, for which there is a
[dedicated
vignette in the `pkgcheck` package](https://docs.ropensci.org/pkgcheck-editor-extra/articles/extending-checks.html).
Please discuss any proposed new checks by opening an issue on the GitHub
repository.


## Code of Conduct

We want to encourage a warm, welcoming, and safe environment for contributing to
this project. See the [code of
conduct](https://ropensci.org/code-of-conduct/) for
more information.
