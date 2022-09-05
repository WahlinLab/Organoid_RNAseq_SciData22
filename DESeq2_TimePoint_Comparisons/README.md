This folder contains .tabular files outputted by DESeq2 comparing differential gene expression for organoid samples from each time point pair.
DESeq2 generates a tabular file containing the different columns in the following order (left to right):
| Column      | Description |
| ----------- | ----------- |
| 1   | Gene Identifiers       |
| 2   | mean normalised counts, averaged over all samples from both conditions        |
| 3   | the logarithm (to basis 2) of the fold change      |
| 4   | standard error estimate for the log2 fold change estimate        |
| 5   | Wald statistic       |
| 6   | p value for the statistical significance of this change        |
| 7   | p value adjusted for multiple testing with the Benjamini-Hochberg procedure which controls false discovery rate (FDR)        |
