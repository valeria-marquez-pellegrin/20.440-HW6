# 20.440-HW6

**Project title:**

Analyzing the skin transcriptome of Alopecia areata patients pre- and post-treatment with ruxolitinib, a JAK inhibitor

**Overview:**

This repository's Formal_analysis.py notebook conducts advanced biological data analysis, with a particular focus on pathway analysis using data from the KEGG database. The notebook is designed to analyze and understand the interactions and functions within biological pathways, specifically through the lens of gene expression data from Affymetrix microarrays.

The main goal of this analysis is to identify significant pathways under different biological conditions, such as upregulated or downregulated genes. This involves fetching detailed pathway information from the KEGG database and conducting a thorough examination of gene interactions within these pathways. Through a combination of data retrieval, processing, and analysis techniques, the notebook serves as a tool for exploring the complex dynamics of biological systems. It facilitates a deeper understanding of how gene expressions are modulated within pathways, offering a foundation for further exploration and investigation in molecular biology and genetics.

**Data**

Dataset is publicly available under GEO Accession GSE80342 (https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE80342). This dataset contains data from 3 controls and 12 patients across 2 timepoints (baseline and 12 weeks post-treatment with ruxolitinib and a set of control participants that did not have alopecia areata and were not given the drug.

**Folder structure**

* Data: This folder contains the raw data extracted from the GEO Accession GSE80342.

* Results: This folder is subdivided into Figures and Dataframes.
	* Figures: It contains all the resulting figures from the analysis (Volcano Plots, Heatmap, KEGG/GO analysis)
	* Dataframes: It has the different dataframes after processing the data. This also includes the results for the KEGG and GO analysis for the different groups.

* Code: This folder contains the main code to run the analysis.

**Installation:**

To run this notebook, you need to set up a Python environment with Jupyter Notebook or JupyterLab. The following packages and their dependencies are required:

* google.colab for running the notebook in Google Colab.
* seaborn, matplotlib, pandas for data visualization and analysis.
* gseapy for gene set enrichment analysis.
* graphviz for graph visualization.
* biopython for importing a set of tools for biological computation.
* biomart for querying databases like Ensembl, useful in bioinformatics for retrieving large datasets.


**References:**

[1] L. Petukhova et al., "Genome-wide association study in alopecia areata implicates both innate and adaptive immunity," in Nature, vol. 466, no. 7302, pp. 113-117, 2010. Available: https://doi.org/10.1038/nature09114

[2] A. Jabbari, L. Xing, et al., "A transcriptomic map of murine and human alopecia areata," JCI Insight, vol. 5, no. 13, e137424, 2020. [Online]. Available: https://doi.org/10.1172/jci.insight.137424

[3] Bioconductor Project, "An end to end workflow for differential gene expression using Affymetrix microarrays," Bioconductor. [Online]. Available: https://www.bioconductor.org/help/workflows/arrays/
