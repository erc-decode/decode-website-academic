---
title: "Comparison of transformations for single-cell RNA-seq data"
abstract: "The count table, a numeric matrix of genes × cells, is the basic input
  data structure in the analysis of single-cell RNA-sequencing data. A common preprocessing
  step is to adjust the counts for variable sampling efficiency and to transform them
  so that the variance is similar across the dynamic range. These steps are intended
  to make subsequent application of generic statistical methods more palatable. Here,
  we describe four transformation approaches based on the delta method, model residuals,
  inferred latent expression state and factor analysis. We compare their strengths
  and weaknesses and find that the latter three have appealing theoretical properties;
  however, in benchmarks using simulated and real-world data, it turns out that a
  rather simple approach, namely, the logarithm with a pseudo-count followed by principal-component
  analysis, performs as well or better than the more sophisticated alternatives. This
  result highlights limitations of current theoretical analysis as assessed by bottom-line
  performance benchmarks.\n"
date: "2023-04-10"
authors:
- cahlmanneltze
- whuber
publication: '*Nature Methods*'
publication_short: ''
publication_types: 2
featured: no
doi: "10.1038/s41592-023-01814-1"
url_pdf: "https://www.nature.com/articles/s41592-023-01814-1"
url_code: "https://github.com/const-ae/transformGamPoi-Paper"
tags:
- Huber Group
- Bioinformatics
---

