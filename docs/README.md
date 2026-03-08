# FragPipe-Analyst

FragPipe-Analyst is an easy-to-use, interactive web application developed to perform various computational analyses and to visualize quantitative mass spectrometry-based proteomic datasets processed using [FragPipe](https://fragpipe.nesvilab.org/) computational pipeline. It is compatible with the LFQ-MBR, spectral counts, TMT, and DIA quantification workflows in FragPipe, and supports protein-level, peptide-level, and PTM site-level analyses.

FragPipe-Analyst provides multiple useful analysis features, including differential expression (DE) analysis using [Limma](https://bioconductor.org/packages/release/bioc/html/limma.html), enrichment analysis (GO/Pathways) using [Enrichr](https://maayanlab.cloud/Enrichr/), and multiple options for missing value imputation. It provides rich data visualization capabilities, including PCA and volcano plots, sample correlation plots, heatmaps, plots for missing value and sample coverage inspection, feature abundance plots for selected features, imputation effect evaluation, dual-comparison scatter plots, and absence/presence analysis with Venn, UpSet, and Jaccard similarity plots. The user can also export results in table format for further analysis, such as DE results (FC and p-values), imputed data matrix (feature abundances after performing selected imputation method), and GO/pathway enrichment results.

## Public Servers
There are two server instances
- Production (stable) server is available at [https://fragpipe-analyst.org/](https://fragpipe-analyst.org/).
- Development server is hosted at [http://fragpipe-analyst.nesvilab.org/](http://fragpipe-analyst.nesvilab.org/). It provides the most up to date version, including bug fixes, but may not be stable 

## Quick Start
- [Formatting input files and upload them for analysis](Formatting.md)
- [Interpret the results](Interpretation.md)

## Tutorial

- [TMT](TMT-tutorial/README.md): A clear cell renal cell carcinoma TMT experiment example from [CPTAC study](https://doi.org/10.1016/j.cell.2019.10.007) published in Cell.
- [LFQ](LFQ-AP-MS-tutorial/README.md): An LFQ AP-MS example of head and neck cancer from [Swantey et al.](https://doi.org/10.1126%2Fscience.abf2911) published in Science.
- [DIA](DIA-tutorial/README.md): A tutorial using subset of clear cell renal cell carcinoma data independent acquisition (DIA) experiment. It's the second part of a tutorial using collection of FragPipe softwares for DIA analysis. You can also find the first part [here](DIA-tutorial/DIA.md).
- [LFQ Hands-On Tutorial](LFQ-tutorial): An hands-on tutorial of analyzing a gliomas data-dependent label-free quantification (LFQ) dataset. It's the second part of a tutorial using collection of FragPipe softwares for LFQ analysis. You can find the first part [here](LFQ-tutorial/LFQ.md).

## Documentation
Detailed information of functionalities are provided for each module. Readers are recommended to read [our manuscript published in Journal of Proteome Research](https://pubs.acs.org/doi/10.1021/acs.jproteome.4c00294) first for the overview.
- [Interpretation](Interpretation.md): Descriptions of all plots and analysis outputs
- [Normalization](documentation/normalization.md)
- [Imputation](documentation/imputation.md)

## Advanced Usage
- [Installation](documentation/installation.md): Install your own copy on your computer or server
- [GSEA](advanced.md): After getting differential expression analysis result from FragPipe-Analyst, users could perform Gene Set Enrichment Analysis (GSEA) by themselves easily.
- We also recommend advanced users to use [FragPipeAnalystR](https://www.nesvilab.org/FragPipeAnalystR/) R package for further downstream analysis. It covers the same functionality as FragPipe-Analyst.

## Questions, and Technical Support 
This repository is intended to provide documentation and a user forum for questions, suggestions, and bug reports. For bug report, please make sure you provide enough details for reproducing the errors. If you feel safer sharing data via email, please email it to [yihsiao@umich.edu](yihsiao@umich.edu). 

- [Questions/Suggestions](https://github.com/Nesvilab/FragPipe-Analyst/discussions)
- [Bug Reports](https://github.com/Nesvilab/FragPipe-Analyst/issues)

## Reference
[Yi Hsiao, Haijian Zhang, Ginny Xiaohe Li, Yamei Deng, Fengchao Yu, Hossein Valipour Kahrood, Joel R. Steele, Ralf B. Schittenhelm, and Alexey I. Nesvizhskii
Journal of Proteome Research (2024), DOI: 10.1021/acs.jproteome.4c00294](https://pubs.acs.org/doi/10.1021/acs.jproteome.4c00294)

## Source Code
The source code of FragPipe-Analyst can be found [here](https://github.com/MonashProteomics/FragPipe-Analyst).
The code is available under GNU General Public License v3.0

## Credits
FragPipe-Analyst is being developed by the [Nesvizhskii Lab](https://www.nesvilab.org/) (University of Michigan) in collaboration with the Monash Proteomics and Metabolomics Facility & Monash Bioinformatics Platform, Monash University (PI Ralf Schittenhelm). FragPipe-Analyst is based on the original LFQ-Analyst code developed by the Monash University team.   

