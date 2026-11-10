# Differential Expression & GO Enrichment Pipeline

An automated R pipeline for differential expression analysis and functional enrichment of proteomics/transcriptomics data.

## Overview
This script performs a complete downstream analysis of expression data, identifying differentially expressed features between sample groups (BT vs CJK) and highlighting enriched biological pathways. 

## Workflow
1. **Data Preprocessing & EDA:** Filtering missing values and KNN imputation (`impute`).
2. **Normalization:** Log2 transformation and quantile normalization (`limma`).
3. **Dimensionality Reduction:** PCA for sample clustering assessment.
4. **Differential Expression:** Empirical Bayes statistics using `limma`.
5. **Visualization:** MA-plots, Volcano plots (`ggplot2`), and Heatmaps (`gplots`).
6. **Functional Annotation:** GO enrichment analysis for biological processes using `gprofiler2` and `enrichplot`.

## Tech Stack
* **Language:** R
* **Key Packages:** `limma`, `gprofiler2`, `ggplot2`, `impute`, `vegan`, `Biobase`
