# RNA-seq Differential Expression Analysis
A structured and reproducible transcriptomic analysis workflow for bulk RNA-seq differential expression studies.

## Project Description
This project implements a reproducible RNA-seq differential expression analysis workflow using DESeq2 to identify statistically significant transcriptional changes between biological conditions. The pipeline integrates normalization, generalized linear modeling, false discovery rate (FDR) control, dimensionality reduction (PCA), and functional enrichment analysis (GO & KEGG). 
## Organism
Homo sapiens (modifiable for other model organisms)

## Tools Used
- R (statistical computing environment)
- DESeq2 (differential expression analysis)
- clusterProfiler (functional enrichment analysis)
- ggplot2 (data visualization)
- pheatmap (heatmap visualization)
  
## Statistical Thresholds
- Adjusted p-value (FDR, Benjamini–Hochberg) < 0.05  
- |Log2 Fold Change| > 1  
- Low-count filtering: genes with row sum > 10

## Reproducibility
- Analysis performed in R (version specified in sessionInfo.txt)
- All package versions documented in sessionInfo.txt
- Modular script-based workflow for reproducible execution
- Output files generated programmatically in results/ and figures/
  
## Author
D. Preethi  
M.Sc. Biochemistry  
Stem Cell Biology Laboratory  

## How to Execute the Workflow

1. Place count matrix and metadata file inside the `data/` directory.
2. Run scripts sequentially from the `scripts/` folder:
   - 01_DESeq2_analysis.R
   - 02_PCA_analysis.R
   - 03_volcano_plot.R
   - 04_GO_enrichment.R
   - 05_KEGG_enrichment.R
   - 06_Heatmap_top50.R
3. Output files will be automatically saved in the `results/` and `figures/` directories.

## Repository Structure
RNA-seq/
├── README.md
├── data/
├── scripts/
│   ├── 01_DESeq2_analysis.R
│   ├── 02_PCA_analysis.R
│   ├── 03_volcano_plot.R
│   ├── 04_GO_enrichment.R
│   ├── 05_KEGG_enrichment.R
│   ├── 06_Heatmap_top50.R
├── results/
├── figures/
└── sessionInfo.txt

Note: Example output files are generated from demonstration data for workflow illustration purposes.

## License
This project is intended for academic and educational purposes.
