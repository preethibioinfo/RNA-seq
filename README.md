# RNA-seq Differential Expression Analysis

This repository contains RNA-seq analysis pipelines and scripts used for differential gene expression studies.

## Project Description
This project performs transcriptomic profiling using DESeq2 to identify differentially expressed genes between biological conditions. The workflow includes normalization, statistical testing with multiple testing correction, dimensionality reduction (PCA), and functional enrichment analysis (GO & KEGG).

## Tools Used
- R
- DESeq2
- PCA analysis
- Volcano plots
- GO & KEGG enrichment

## Author
D. Preethi  
M.Sc. Biochemistry  
Stem Cell Biology Laboratory  


## Workflow
RNA-seq/
│
├── README.md
├── data/
├── scripts/
│   ├── 01_DESeq2_analysis.R
│   ├── 02_PCA_analysis.R
│   ├── 03_volcano_plot.R
│   ├── 04_GO_enrichment.R
│   ├── 05_KEGG_enrichment.R
│   ├── 06_Heatmap_top50.R
│
├── results/
├── figures/
└── sessionInfo.txt
