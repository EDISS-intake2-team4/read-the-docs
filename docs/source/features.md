# Feature Selection
--------------------

## Feature Selection Algorithms
On the feature selection page the user can select the feature selection algorithms to run.
The following feature selection algorithms are available:
- Pearson Correlation: Pearson product-moment correlation coefficients. [Link](https://numpy.org/doc/stable/reference/generated/numpy.corrcoef.html)

- Chi Square: Computing chi-squared stats between each non-negative feature and class. [Link](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.chi2.html) Chi-Square was used for feature selection because it was found to be an effective feature selection method for biomarker detection for Alzheimer's disease [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10217314/).

- False Discovery Rate: Use the Benjamini-Hochberg procedure to select the p-values for an estimated false discovery rate. [Link](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.SelectFdr.html)

- Recursive Feature Elimination: Select features by recursively considering smaller and smaller set of features. [Link](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.RFE.html)

- Joint Mutual Information: Use estimated mutual information for a discrete target variable. [Link](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_classif.html)

- Protein Marker Selection: uses multiview feature selection especially targeted for proteomics or multi-omics datasets. [PyPI](https://pypi.org/project/proms/)

- Fold Change: Fold change was computed using the following formula to measure how much a quantity changes between an original and a subsequent measurement: Fold Change = (Mean of intensity values for experimental samples (Samples with Parkinson's))/(Mean of intensity values for control samples (Healthy samples)) [Reference](https://www.computabio.com/fold-change-analysis.html)

- P-value: P-value is computed using T-test for the means of two independent samples of scores. This is a test for the null hypothesis that 2 independent samples have identical average (expected) values. This test assumes that the populations have identical variances by default. [Link](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html)

- ROTS: (only available if ROTS was calculated on the ROTS page) Reproducibility optimized test statistic for for ranking genes/proteins based on evidence for differential expression. [Link](https://pypi.org/project/rots-py/1.2.2/)

Once the feature selection algorithms are selected, the **Run Feature Selection** button applies the selected algorithms to identify a subset of features based on the default parameters of each algorithm. Once completed, the results of the algorithms can be examined by expanding the boxes with the algorithm name. Additionally, algorithm parameters can be edited within the algorithm expanded box directly or by unchecking the "Use Default Parameters" checkbox which will allow to specify custom parameters. 

## Results Intersection 
After different feature selection algorithms are run, the results of the algorithms can be intersected to identify features that are common to all algorithms. In the **Intersect** box a subset of all the executed algorithms is displayed and the user can choose the results of which algorithms they want to intersect. The **Intersect** button applies the intersection to the results of the algorithms. The results of the intersection can be examined by expanding the **Intersection Results** box. The Intersection Results are displayed in a table with a column at the end which shows the number of algorithm that selected a particular feature. The user can also download the results of the intersection as a csv file by clicking the **Download** button.