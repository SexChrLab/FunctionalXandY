This directory contains resources (lookup tables) for scientists working with GTEx, TCGA, and CCLE genomics gene expression data. 

```InferredSCC.xlsx```

This Excel file includes the inferred sex chromosome complement for these three data sets based on expression of select sex chromosome genes. DNA ploidy is included when available.

```UnexpectedSCC.xlsx```

This  Excel file lists samples in the three data sets that have a sex chromosome complement that might reflect mislabelling, sample swapping, or contamination.  These include samples from female individuals where expression of chromosome Y genes is observed or samples from male individuals where expression of XIST is observed (indicating XX ploidy). 

```TCGA_*All.csv```

These comma separated value (csv) files are merged differential expression tables from tissues in which various sex chromosome complement related profiles are generated.  LOX stands for loss of chromosome X in samples from female individuals.  LOY stands for loss of chromosome Y in male in samples from male individuals.  XaXa stands for X chromosome reactivation (loss of X chromosome inactivation) in samples from female individuals.


```TCGA_*Consistent.csv```

These comma separated value (csv) files are filtered for just the genes that are consistent between tissues (same direction, p-value < 0.05 in at least 60% of tissues).

