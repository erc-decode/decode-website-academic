---
title: 'glmGamPoi: fitting Gamma-Poisson generalized linear models on single cell count data'
abstract: |
    **Motivation:** The Gamma-Poisson distribution is a theoretically and empirically motivated model for the sampling variability of single cell RNA-sequencing counts and an essential building block for analysis approaches including differential expression analysis, principal component analysis and factor analysis. Existing implementations for inferring its parameters from data often struggle with the size of single cell datasets, which can comprise millions of cells; at the same time, they do not take full advantage of the fact that zero and other small numbers are frequent in the data. These limitations have hampered uptake of the model, leaving room for statistically inferior approaches such as logarithm(-like) transformation.

    **Results:** We present a new R package for fitting the Gamma-Poisson distribution to data with the characteristics of modern single cell datasets more quickly and more accurately than existing methods. The software can work with data on disk without having to load them into RAM simultaneously.

    **Availability and implementation:** The package glmGamPoi is available from Bioconductor for Windows, macOS and Linux, and source code is available on [github.com/const-ae/glmGamPoi](https://github.com/const-ae/glmGamPoi) under a GPL-3 license. The scripts to reproduce the results of this paper are available on [github.com/const-ae/glmGamPoi-Paper](https://github.com/const-ae/glmGamPoi-Paper).

    **Supplementary information:** Supplementary data are available at Bioinformatics online.

authors:
    - Constantin Ahlmann-Eltze
    - whuber
date: 2020-12-09
publication: '*Bioinformatics*, Volume 36, Issue 24, 15 December 2020, Pages 5701–5702'
publication_short: ""
publication_types:
    - 2
featured: false
links:
- name: PubMed
  url: https://pubmed.ncbi.nlm.nih.gov/33295604/
doi: 10.1093/bioinformatics/btaa1009
url_pdf: https://academic.oup.com/bioinformatics/article-pdf/36/24/5701/36899440/btaa1009.pdf
url_code: https://github.com/const-ae/glmGamPoi
---

