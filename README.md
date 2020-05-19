# Introduction
This repository contains all scripts used for our publication "A kinase-deficient NTRK2 splice variant predominates in glioma and amplifies several oncogenic signaling pathways"

## References 
1) Vivian J, Rao AA, Nothaft FA, et al. (2017) Toil enables reproducible, open source, big biomedical data analyses. Nature biotechnology. 
2) The GTEx Consortium. The Genotype-Tissue Expression (GTEx) project. (2013) Nature genetics.
3) R Core Team (2018). R: A language and environment for statistical computing. R Foundation for Statistical Computing, Vienna, Austria. URL https://www.R-project.org/.

## Tools used for analysis 

All our analysis is done in R using the following  R/Biocondcutor packages.

1) [ggplot2](https://ggplot2.tidyverse.org/) for making most of the plots in our paper. 
2) [pheatmap](https://cran.r-project.org/web/packages/pheatmap/index.html) and [RColorBrewer](https://cran.r-project.org/web/packages/RColorBrewer/index.html) for making heatmaps 
3) [DGCA](https://cran.r-project.org/web/packages/DGCA/index.html) for Differential gene correlation analysis
4) [edgeR](https://www.bioconductor.org/packages/release/bioc/html/edgeR.html) and [DESeq2](https://www.bioconductor.org/packages/release/bioc/html/DESeq2.html) for finding differentially expressed genes.
5) [clusterProfiler](https://www.bioconductor.org/packages/release/bioc/html/clusterProfiler.html) and [ReactomePA](https://www.bioconductor.org/packages/release/bioc/html/ReactomePA.html) for GO and pathway enrichment analysis

To ensure smooth execution of code in this repository, please install the 
following packages 

```{r eval=FALSE}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(c("DGCA", "edgeR", "DESeq2", 
                       "clusterProfiler",  "ReactomePA",
                       "pheatmap", "RColorBrewer", "ggplot2", "gridExtra"))
```
