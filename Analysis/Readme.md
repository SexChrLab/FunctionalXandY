This directory contains R Markdown files to show how analysis was done for Plaisier et al. 2025: 

https://www.biorxiv.org/content/10.1101/2025.09.24.678401v1

Heatmaps_Consistent.Rmd

This Rmd shows how to take differential gene expression results across multiple tissues and produce the annotated heatmaps in Figure 3.
1. Input: limma voom differential expression results from multiple tissues (output of topTable with all genes)
2. Selects Consistent Genes: Changing the same direction in all tissues (logFC sign) and significant (p-value < 0.05) in at least 60% of tissues  
3. Once these genes have been selected, the genes can be written out and entered into Metascape (https://metascape.org/gp/index.html#/main/step1)
4.  An Excel can be downloaded with the results-- the Annotation tab should be saved as a comma-separated file (csv)
5.  This is entered as an additional input and used to create row annotations with specific fields



