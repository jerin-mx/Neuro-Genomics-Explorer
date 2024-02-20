# Single-Cell RNA-seq Analysis of Mouse Neocortex

## Overview
This project aims to analyze single-cell RNA sequencing (RNA-seq) data from the mouse neocortex, with the objective of uncovering its hierarchical structure and identifying key genes. The neocortex is crucial for higher-level brain functions such as perception and cognition. Through this analysis, we explore the complexities of cellular gene expression within this brain region, leveraging various subsets of a comprehensive dataset compiled by the Allen Institute.

## Data Description
The dataset consists of a counts matrix, where each row represents an individual cell and each column corresponds to a gene, measured in normalized transcript compatibility counts (TCC), scaled to counts per million. This structure allows us to quantify gene expression levels across different cells.

## Data Sources
The data, available in gene_analysis_data.tar.gz, is divided into three main parts for structured analysis:

- Labeled Subset (p1): A small, labeled portion of the dataset including a count matrix and clustering labels derived from domain knowledge and statistical testing. This subset serves as a foundation for initial exploratory analysis.
- Unsupervised Subset (p2_unsupervised): Contains only a count matrix for further exploration without predefined labels.
- Evaluation Subset (p2_evaluation): Includes labeled training and test sets for evaluating feature selection and model performance.
Reduced versions of the unsupervised and evaluation datasets (p2_unsupervised_reduced and p2_evaluation_reduced) are provided for efficiency in computational resource usage.

## Methodology
Our analysis consists of three main stages, each designed to progressively explore and understand the dataset's underlying structure and the role of genes in cellular differentiation:

- Exploratory Analysis: Utilizing visualization and clustering techniques to unveil the dataset's structure and identify clusters within the cell population.
- Feature Discovery: Applying clustering and logistic regression on a larger subset to identify informative features distinguishing different cell types.
- Robustness Check: Revisiting analytical decisions (e.g., T-SNE hyperparameters, cluster numbers) to assess the stability of our findings against these choices.

## Requirements
Python 3.x
Libraries: numpy, pandas, matplotlib, scikit-learn, seaborn, and others as specified in requirements.txt.

## Contributing
Contributions to the project are welcome. Please refer to the contributing guidelines for more details.
