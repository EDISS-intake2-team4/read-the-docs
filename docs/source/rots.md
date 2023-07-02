# ROTS 

Reproducibility optimized test statistic (ROTS) is a method for identifying differentially expressed genes in RNA-seq data. It is based on a generalized linear model (GLM) framework and uses a novel test statistic that is optimized for reproducibility. ROTS is implemented in the R package [ROTS](https://bioconductor.org/packages/release/bioc/html/ROTS.html) and a python package [rots-py](https://pypi.org/project/rots-py/1.0.3/).

## ROTS parameters
There are two parameters you need to set in order to run ROTS analysis: the number of permutations (B) and the top list size (K). The number of permutations is the number of times the data will be permuted. The top list size is the number of genes that will be selected as differentially expressed. 

A seed value can also be set for reproducibility. The seed value is used to initialize the random number generator.

If you want to skip the parameter optimization and set the a1 and a2 paramers manually you can do so by checking the "Set advanced parameters" checkbox. The a1 and a2 parameters can be set in the text boxes below. For more information see [rots-py](https://github.com/EDISS-intake2-team4/rots-py/blob/main/README.md) and [Bioconductor:ROTS](https://bioconductor.org/packages/release/bioc/html/ROTS.html).

## ROTS results
The results of the ROTS analysis are shown in a table. The table contains features/genes/proteins that satisfy the specified condition. Three cutoff options are available: **FDR**, **p-value**, and **Feature count**. Once the cutoff option is selected and the cutoff value is specified, the Apply cutoff button displays a table with the following columns ordered by the ROTS-statistic:
- **Row**: the gene/protein name or ID
- **ROTS-statistic**: the ROTS statistic calculated for the gene/protein based on the optimized parameters
- **pvalue**: the p-value
- **FDR**: the false discovery rate

In addition to the table, z-score **Z** , top list size **k**, reproducibility score **R**, and the optimization parameters **a1** and **a2** are shown.



