This directory contains R Markdown files to show how analysis was done for Plaisier et al. 2025: 

https://www.biorxiv.org/content/10.1101/2025.09.24.678401v1



```Heatmaps_Consistent.Rmd```

This Rmd shows how to take differential gene expression results across multiple tissues and produce the annotated heatmaps in Figure 3.
1. Input: limma voom differential expression results from multiple tissues (output of topTable with all genes)
2. Selects Consistent Genes: Changing the same direction in all tissues (logFC sign) and significant (p-value < 0.05) in at least 60% of tissues  
3. Once these genes have been selected, the genes can be written out and entered into Metascape (https://metascape.org/gp/index.html#/main/step1)
4.  An Excel can be downloaded with the results-- the Annotation tab should be saved as a comma-separated file (csv)
5.  This is entered as an additional input and used to create row annotations with specific fields
6.  This also includes code to create a circos plot of all the consistent gene profiles we created (Figure 4).


```TCGA_co_aneuploidy.Rmd```

This Rmd shows how to plot the aneuploidy score and APC expression for Figure S12 (Supplementary Figure).

This makes use of data available in this publication: Taylor, Alison M., Juliann Shih, Gavin Ha, Galen F. Gao, Xiaoyang Zhang, Ashton C. Berger, Steven E. Schumacher, et al. 2018. “Genomic and Functional Approaches to Understanding Cancer Aneuploidy.” Cancer Cell 33 (4): 676–689.


```TCGA_compare_survival.Rmd```

This Rmd shows how to create the Kaplan Meyer curve and associated summary values in Figure 5.  

This makes use of data available in this publication: Thorsson, Vésteinn, David L. Gibbs, Scott D. Brown, Denise Wolf, Dante S. Bortone, Tai-Hsien Ou Yang, Eduard Porta-Pardo, et al. 2018. “The Immune Landscape of Cancer.” Immunity 48 (4): 812–830.e14.


```TCGA_gene_expression.Rmd```

This Rmd is an example of how we generated differential gene expression profiles for various sample groups using the limma-voom pipeline.
