# ROTS 

Reproducibility optimized test statistic (ROTS) is a method for identifying differentially expressed genes in RNA-seq data. It is based on a generalized linear model (GLM) framework and uses a novel test statistic that is optimized for reproducibility. ROTS is implemented in the R package [ROTS](https://bioconductor.org/packages/release/bioc/html/ROTS.html) and a python package [rots-py](https://pypi.org/project/rots-py/1.0.3/).

## ROTS parameters
There are two parameters you need to set in order to run ROTS analysis: the number of permutations (B) and the top list size (K). The number of permutations is the number of times the data will be permuted. The top list size is the number of genes that will be selected as differentially expressed. The default values are 1000 permutations and 1000 genes in the top list.

A seed value can also be set for reproducibility. The seed value is used to initialize the random number generator. The default value is 123.

If you want to skip the parameter optimization and set the a1 and a2 paramers manually you can do so by checking the "Set advanced parameters" checkbox. The a1 and a2 parameters can be set in the text boxes below. For more information see [ROTS documentation](https://bioconductor.org/packages/release/bioc/vignettes/ROTS/inst/doc/ROTS.pdf).

## ROTS results
The results of the ROTS analysis are shown in the table below. The table contains the top list of genes that are differentially expressed. The table contains the following columns:
- **Gene/protein**: the gene/protein name
- **log2FC**: the log2 fold change
- **PValue**: the p-value
- **FDR**: the false discovery rate

In addition to the table, z score, top list size, and the optimization parameters are shown.

