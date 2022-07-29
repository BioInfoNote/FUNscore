
# calFUNscore

The goal of calFUNscore is to evaluate functional score of tumor cells/tissue using scRNA or bulk transcriptomic data.

## Installation

You can install the development version of calFUNscore from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("BioInfoNote/calFUNscore")
```

## Example 

``` r
library(FUNscore)
data("expr")
data("funRelatedGeneSet")
fungeneset = funRelatedGeneSet[["Angiogenesis"]]@geneIds
cfs <- calFUNscore(expr = expr, fungeneset = fungeneset, study.type = "bulk_RNAseq")
}

```
