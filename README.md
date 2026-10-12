# Fibrosis_AAA_Sexdifferences
## 1.Introduction
This is the code we implemented for manuscript entitled "Sex-based differences in fibrosis markers in human abdominal aortic aneurysms" developed in Dr. Zayed Vascular Surgery LAB, Washington University, St. Louis, MO. This work has been accepted in priciple to be published in iScience journal. This work has previously presented at several conferences such as de Academic Surgical Congress (ASC) and the American College of Surgeons (ACS). 
## 2. Background
Abdominal aortic aneurysms (AAA) are a chronic degenerative vascular disease characterized by a progressive dilation of the abdominal aorta resulting from an imbalance in extracellular matrix (ECM) synthesis and degradation. Biological sex plays a critical factor in the progression and rupture potential of AAAs, as females experience rupture at smaller diameters compared to males. We hypothesized that fibroblast activation protein (FAP) may influence fibrosis and disease severity in AAA, with potential sex-specific differences.
## 3. Experiment Methods
A multi-centered transcriptomic analysis of aortic samples from 15 human AAA and 5 non-AAA was performed to evaluate cell-specific fibrosis gene expression profiles.
## 4. Briefly SC RNA-seq platform
Transcriptomic analysis was conducted by integrating three publicly available single-cell RNA sequencing (scRNA-seq) datasets (GSE166676, GSE237230, GSE226492) comprising human aortic samples. A total of 20 samples were consolidated for the combined gene-barcode matrix analysis using the Seurat package (v.5.2.1). The dataset was integrated using the FastMnn batch correction.
## 5. QC 
A doublet-filtering algorithm (scDblFinder) was applied to the dataset. Cells expressing 200-5000 genes were retained in the analysis. Cells with mitochondrial gene expression exceeding 30% were excluded from the analysis.
## 6. Annotation and Gene enrichment analysis
### Dependencies
This project requires the following packages:
#### •R: 4.3.0 
#### •Seurat: 5.2.1
#### •SeuratExtend: 1.2.0 
#### •here: 1.0.1
#### •stringr: 1.5.1
#### •purrr: 1.0.2
#### •readr: 2.1.5
#### •scCustomize: 3.0.1
#### •ggplot2: 3.5.1
#### •cowplot: 1.1.3
#### •dplyr: 1.1.4
#### •Matrix: 1.7.0
#### •viridis: 0.6.5
#### •harmony: 1.2.0
#### •SeuratWrappers: 0.4.0
#### •tidyverse: 2.0.0
#### •devtools: 2.4.5
#### •ggrepel: 0.9.6
#### •rlang: 1.1.5
Eight major cell clusters were identified: vascular smooth muscle cells (VSMCs), fibroblasts, endothelial cells, macrophages, neutrophils, T cells, B cells, and plasma cells utilizing canonical markers.   A specific subcluster analysis focused on VSMCs and fibroblasts was performed to evaluate fibrosis markers (FAP, COL1A1, COL1A2, and VIM).   Statistical significance was determined using Bonferroni-adjusted p-values, with a false discovery rate (FDR) adjusted p-value threshold of <0.05 using the Wilcox test. 
## 7. R Script
Detailes steps for figure generation beyond this point, can be found in the main R script (AAA_Ctrl_Merged.Rmd)
