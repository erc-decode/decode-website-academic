---
title: 'Transformation and Preprocessing of Single-Cell RNA-Seq Data'
abstract: |
    The count table, a numeric matrix of genes × cells, is the basic input data structure in the analysis of single-cell RNA-seq data. A common preprocessing step is to adjust the counts for variable sampling efficiency and to transform them so that the variance is similar across the dynamic range. These steps are intended to make subsequent application of generic statistical methods more palatable. Here, we describe three transformations (based on the delta method, model residuals, or inferred latent expression state) and compare their strengths and weaknesses. We find that although the residuals and latent expression state-based models have appealing theoretical properties, in benchmarks using simulated and real-world data the simple shifted logarithm in combination with principal component analysis performs surprisingly well.

    **Software:** An R package implementing the delta method and residuals-based variance-stabilizing transformations is available on [github.com/const-ae/transformGamPoi](https://github.com/const-ae/transformGamPoi).

authors:
    - Constantin Ahlmann-Eltze
    - whuber
date: 2021-08-25
publication: '*bioRxiv*'
publication_short: ""
publication_types:
    - 3
featured: false
doi: 10.1101/2021.06.24.449781
url_pdf: https://www.biorxiv.org/content/10.1101/2021.06.24.449781v2.full.pdf
url_code: https://github.com/const-ae/transformGamPoi
tags: ["Huber Group", "Bioinformatics"]
---

