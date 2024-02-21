# Single-Cell RNA-seq Analysis of Mouse Neocortex

## Overview
This project focuses on analyzing a single-cell RNA sequencing (RNA-seq) dataset from the mouse neocortex, aiming to unveil hierarchical structures and identify significant genes. The dataset, compiled by the Allen Institute, encompasses various subsets of a larger single-cell RNA-seq dataset, offering insights into the cellular composition of the neocortex, a critical brain region responsible for higher-level functions like perception and cognition.

## Data Description
The RNA-seq data is structured as a counts matrix, with rows representing individual cells and columns corresponding to genes, measured as normalized transcript compatibility counts (TCC) in counts per million. This setup allows for the quantitative analysis of gene expression levels across cells.

## Dataset Structure
- **p1 (Labeled Subset):** A small portion of the data with both a counts matrix (X) and "ground truth" clustering labels (y), derived from domain knowledge and statistical testing, for initial analysis.
- **p2_unsupervised:** Contains only a count matrix for exploratory analysis without predefined labels.
- **p2_evaluation:** Includes a labeled training and test set for feature selection evaluation.

Reduced versions of the datasets ('p2_unsupervised_reduced' and 'p2_evaluation_reduced') are available for more resource-efficient analysis.

## Analysis Workflow

### Data Loading and Transformation
**Log Transformation:** Applied to the counts matrix to normalize gene expression magnitudes.
**PCA:** Used to reduce dimensionality and identify principal components explaining significant variance.

### Visualization Techniques
**t-SNE and MDS**: Employed for visualizing the high-dimensional data in two-dimensional space, revealing distinct cell clusters.

### Clustering
**K-Means and Hierarchical Clustering:** Applied to group cells into clusters based on their gene expression profiles.

### Feature Selection and Validation
**Logistic Regression:** Utilized for identifying genes that are informative of cell types. The analysis includes standardization, regularization, and evaluation using cross-validation and test sets.

## Requirements
Python 3.x
Libraries: numpy, pandas, matplotlib, scikit-learn, seaborn, and others as specified in requirements.txt.

## Contributing
Contributions to the project are welcome. Please refer to the contributing guidelines for more details.

## Liscense
Done under MITx Data Analysis Course
