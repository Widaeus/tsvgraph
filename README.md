tsvgraph
================

<!-- README.md is generated from README.Rmd. Please edit that file -->
<!-- badges: start -->
<!-- badges: end -->

The `tsvgraph` package facilitates the importation of graph data.

## Prerequisites

This package is specifically designed for use with PIMsoft version
1.5.8.2090555 (64-bit) developed by Perimed AB. It assumes that the XML
files are generated using the built-in report function with the
following options selected: “Recording info”, “Calculations”, “Mean
perfusion”, and “Percent change per ROI”. Furthermore, ROIs must be
named “ACH”, “SNP”, and “ref”, and TOIs must include “rest”, “ACHmax”,
and “SNPmax”.

## Installation

`tsvgraph` can be installed directly from GitHub using the `devtools`
package. If you do not have `devtools` installed, you can install it
using the command `install.packages("devtools")`. Then, install
`tsvgraph` using:

``` r
# install.packages("devtools")
devtools::install_github("Widaeus/tsvgraph")
```

## Usage

The `pimxml` package includes one primary functions: `tsv_import`

It accepts a tsv file containing graph data generated from PimSOFT using
above prerequisites. It can thereafter be exported to a data frame and
incorporated to a plot.
