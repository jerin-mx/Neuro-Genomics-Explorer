# Single-Cell RNA-seq Analysis of Mouse Neocortex

## Overview
This project focuses on analyzing a single-cell RNA sequencing (RNA-seq) dataset from the mouse neocortex, aiming to unveil hierarchical structures and identify significant genes. The dataset, compiled by the Allen Institute, encompasses various subsets of a larger single-cell RNA-seq dataset, offering insights into the cellular composition of the neocortex, a critical brain region responsible for higher-level functions like perception and cognition.

## Data Description
The RNA-seq data is structured as a counts matrix, with rows representing individual cells and columns corresponding to genes, measured as normalized transcript compatibility counts (TCC) in counts per million. This setup allows for the quantitative analysis of gene expression levels across cells.

## Dataset Structure
- p1 (Labeled Subset): A small portion of the data with both a counts matrix (X) and "ground truth" clustering labels (y), derived from domain knowledge and statistical testing, for initial analysis.
- p2_unsupervised: Contains only a count matrix for exploratory analysis without predefined labels.
- p2_evaluation: Includes a labeled training and test set for feature selection evaluation.
Reduced versions of the datasets ('p2_unsupervised_reduced' and 'p2_evaluation_reduced') are available for more resource-efficient analysis.

## Methodology
### Phase 1: Exploratory Analysis
Objective: Explore a small subset of the data using visualization and clustering methods to understand its structure.
Tools: Various visualization techniques and clustering algorithms.
### Phase 2: Feature Discovery
Objective: Expand analysis to a larger subset, employing clustering and logistic regression to unearth features that distinguish cell types.
Approach: Utilize insights from Phase 1 to guide feature selection and model evaluation.
### Phase 3: Robustness and Reevaluation
Objective: Reassess analytical decisions (e.g., T-SNE hyperparameters, cluster count) to evaluate the robustness of findings.
Method: Critical examination of methodological choices and their impact on the results.

## Requirements
Python 3.x
Libraries: numpy, pandas, matplotlib, scikit-learn, seaborn, and others as specified in requirements.txt.

## Contributing
Contributions to the project are welcome. Please refer to the contributing guidelines for more details.
