# Overview

This respository shows single cell analysis on gastrulation stage mouse embryo (E6.5-E8.5), focusing of the relationship of Wt1 with smooth muscle and mesothelial marker genes. 
Analysis pipeline for assessing vascular density and branching in whole-mount E12.5 mouse embryo with Wt1 knock-out at E7.5 also included.

# Repository Content

## R Markdown
R markdown for single cell analysis, CD31 density and branching analysis

## Datafiles
master_gene_count.csv- CSV file contains processed gene expression counts for Wt1 and its associated marker genes from the raw data, organized by each embryonic stage and cell types.

CD31_density_master_data.csv-  CSV file contains surface area of CD31 and total area of ROI in Wt1 knock-out and controls.

raw_branch_result.csv- CSV file contains raw branch types count and length generated from FIJI in Wt1 knock-out and controls.

# System Requirement

The `R` packages require only a standard computer with enough RAM to support the operations defined by a user. For minimal performance, this will be a computer with about 2 GB of RAM. For optimal performance, we recommend a computer with the following specs:

RAM: 16+ GB  
CPU: 4+ cores, 3.3+ GHz/core

# Software Requirement
The R scripts were tested on *Windows* operating system.

Before running the listed 'R' scripts, users should have `R` version 4.4.1 or higher, and several packages set up from CRAN.

## Package Installation
Users should install the following packages prior to running the script, from an `R` terminal:
````
install.packages("ggplot2, tidyr, "BiocManager", "ggpubr", "paletter","dplyr", "factoextra", "FactoMineR", "outliers", "ggforce")
BiocManager::install("GSEABase", "MouseGastrulationData", "scuttle",'AUCell", "DESeq2")
````
