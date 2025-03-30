RNA-Seq Package Comparison for Coronary Artery Disease (CAD)
Overview
This repository contains an RNA-Seq analysis comparing different bioinformatics packages used for differential gene expression (DEG) analysis, applied to published data from patients with coronary artery disease (CAD). The aim is to compare results from various RNA-Seq analysis packages and evaluate how they perform on the same dataset, focusing on identifying gene expression differences related to CAD.

Objective
The goal of this repository is to:

Compare different RNA-Seq packages: We will use packages like DESeq2, EdgeR, and limma to identify differentially expressed genes in the context of CAD.

Evaluate DEG consistency: By analyzing the same dataset with different packages, we can compare the overlap in DEGs, the strength of the associations, and how the packages handle normalization, statistical testing, and differential expression.

Create plots: Various visualizations like volcano plots, heatmaps, and PCA plots will be generated to summarize the results and compare the performance of the different packages.

Background
The dataset used in this repository comes from a published study on coronary artery disease (CAD), where RNA was extracted from whole blood samples of 177 patients undergoing coronary angiography. The original study aimed to identify RNA signatures associated with CAD, focusing on T cell regulation and Treg function.

The current analysis compares the results of three popular RNA-Seq analysis packages (DESeq2, EdgeR, and limma) to evaluate their performance in identifying DEGs related to CAD.

Methods
Data
The data used for this analysis comes from RNA-Seq of whole blood samples from 177 CAD patients. RNA was extracted, rRNA-depleted, and sequenced using Illumina platforms. The dataset contains gene expression counts that were used for differential expression analysis.

RNA-Seq Analysis Packages
The following RNA-Seq analysis packages were used to perform differential expression analysis:

DESeq2: A package in R for RNA-Seq analysis based on negative binomial distribution. It identifies DEGs by comparing gene expression between groups using fold-change and p-values.

EdgeR: Another popular R package for differential expression analysis that uses the exact test or generalized linear model (GLM) approach for RNA-Seq data.

limma: An R package that is commonly used for differential analysis of RNA-Seq data. We used the voom method, which models RNA-Seq data as continuous counts.

Key Criteria for Analysis
DEG Criteria: Genes with a fold-change ≥ 1.5 and adjusted p-value ≤ 0.05 were considered to be differentially expressed.

Package Comparison: The DEGs identified by each package were compared to evaluate overlap and consistency of results.

Visualization: Various plots were created to compare the DEGs identified by each package.

Plots Generated
Volcano Plots: Used to visualize the relationship between fold-change and statistical significance of DEGs.

Heatmaps: Displaying expression patterns of DEGs across the samples.

PCA (Principal Component Analysis) Plots: Showing clustering of samples based on gene expression data to visualize group separation.

Venn diagram: To identify the overlap

Results
Overlap of DEGs
While there was overlap in the DEGs identified by each package, the extent of overlap varied. DESeq2 and EdgeR had a higher degree of overlap, while limma identified a broader range of genes.

Example Plots
Volcano Plots: Showing DEGs from DESeq2, EdgeR, and limma.

Heatmaps: Visualizing gene expression for the most significantly differentially expressed genes.

PCA Plots: Showing the clustering of samples from CAD patients and controls based on gene expression.

Conclusion
This repository demonstrates the comparison of RNA-Seq analysis packages for the identification of differentially expressed genes in coronary artery disease (CAD) patients. The results confirm that different packages can identify consistent patterns of gene expression changes, particularly those related to immune regulation and T cell dysfunction. The comparison of packages also highlights the importance of selecting the right RNA-Seq tool for a given dataset.

Files in the Repository
RNAseq_analysis.R: R script for performing RNA-Seq differential expression analysis using DESeq2, EdgeR, and limma.

Reference
McCaffrey, Timothy A., Ian Toma, Zhaoqing Yang, Richard Katz, Jonathan Reiner, Ramesh Mazhari, Palak Shah et al. "RNAseq profiling of blood from patients with coronary artery disease: signature of a T cell imbalance." Journal of Molecular and Cellular Cardiology Plus, 4 (2023): 100033. https://doi.org/10.1016/j.jmccp.2023.100033.






