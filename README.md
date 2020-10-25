mrIML: Multivariate--multi-response--interpretable machine learning
================
Author: **Nick Fountain-Jones**
  -affiliation: **University of Tasmania**
Author: **Gustavo Machado**
  -affiliation: **North Carolina State University**
  -url: https://gustavoetal.org/
  
<img src = "https://user-images.githubusercontent.com/33707823/88988817-531ad080-d31d-11ea-8d76-f1ad0506e405.png" width="200" height="200"/>

This package aims to enable users to build and interpret multivariate
machine learning models harnessing the tidyverse (tidy model syntax in
particular). This package builds off ideas from Gradient Forests (Ellis
et al 2012), ecological genomic approaches (Fitzpatrick and Keller,
2014) and multi-response stacking algorithms (Xing et al 2019).

This package can be of use for any multi-response machine learning
problem, but was designed to handle data common to community ecology
(site by species data) and ecological genomics (individual or population
by SNP loci).

## Installation

Install the stable version of the package:

``` r
#install.packages("devtools")
devtools::install_github('nfj1380/mrIML')
```

## Quick start

`{mrIML}` is designed to be used with a single function call or to be
used in an ad-hoc fashion via individual function calls. In the
following section we give an overview of the simple use case. For more
on using each function see the [function documentation](xx). The core
functions for both regression and classification are:
[`mrIMLpredicts`](xx), [`mrIMLperformance`](xx), and
[`mrInteractions`](xx),for plotting and visualization [`mrVip`](xx),
[`mrFlashlight`](xx), and[`plot_vi`](xx). Estimating the interactions
alone can be substantially computationally demanding depending on the
number of outcomes you want to test. The first step to using the package
is to load it as follows.

``` r
library(mrIML)
```

## References

Xing, L, Lesperance, ML and Zhang, X (2020). Simultaneous prediction of
multiple outcomes using revised stacking algorithms. Bioinformatics, 36,
65-72.

Fitzpatrick, M.C. & Keller, S.R. (2015) Ecological genomics meets
community-level modelling of biodiversity: mapping the genomic landscape
of current and future environmental adaptation. Ecology Letters 18,
1–16.

Ellis, N., Smith, S.J. and Pitcher, C.R. (2012), Gradient forests:
calculating importance gradients on physical predictors. Ecology, 93:
156-168. <doi:10.1890/11-0252.1>
