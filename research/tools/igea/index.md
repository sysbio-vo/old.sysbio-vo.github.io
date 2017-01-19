---
layout: page
title: IGEA
description: "Web-based tool for integrative gene expression analysis"
share: true
---

![alt text]({{site.url}}/IGEA.png "IGEA site picture")

### **IGEA** is a web-based tool for Integrative Gene Expression profiles Analysis

This tool enables academic scientists and medical researchers to conduct integrative gene expression analysis. Users are able to construct cross-experiment case-control study groups, search for differentially expressed genes and reverse-engineer gene regulatory networks based on gene expression profiles. The expected result of such analyses includes, but not limited to, relevant data-based hypotheses on etiology and pathogenesis of preeclampsia.

#### Key features:

* The service provides an easy to use access to quality tested, normalized and annotated gene expression profiles obtained from microarray experiments raw data stored in public repositories such as Gene Expression Omnibus or ArrayExpress. 
* Users are able to exploit the benefits of manually standardized (using relevant ontologies such as MeSH) and extended (based on data from corresponding articles and authors personally) sample-wise clinical and other metadata, such as tissue type, diagnosis or gestational age. Such manually curated metadata is a distinctive feature of our service and a crucial component of cross-experiment integration as one can merge and compare gene expression data only from those samples which are similar enough to be put into the same study group. 
* Users can search for differentially expressed genes between manually defined study groups on integrated datasets from different experiments. 
* IGEA allows to reverse-engineer gene regulatory networks based on differentially expressed genes list and corresponding gene expression profiles. We use Bayesian networks as underlying graph model as it is able to grasp nonlinear nature of genes interaction. Learning optimal Bayesian networks is a computationally challenging task, which is impossible without distributed parallel environments. 
* Users are welcome to extend the service database with their experimental data after service providers approval.

Although IGEA can in principle be used to analyse expression profiles of any biological specimen obtained using any technology this tool was originally designed to analyse cDNA microarrays of human placenta under pregnancy complications, namely, pre-eclampsia - pregnancy disorder with unknown etiology, which affects up to 10% of women worldwide and is a major cause of death of both mother and child. Moreover, there is an increased risk for cardiovascular complications, including hypertension and ischemic heart disease, and kidney disease later in life, making preeclampsia a highly studies topic.

The use of IGEA may be especially valuable when the disease like pre-eclampsia is not so “mainstream” as, say, lung cancer. In those cases the experiment’s average sample size is small which makes results prone to statistical errors. The integration of data allows constructing study groups of larger size, thus, increasing statistical significance.

### Prototype

This tool is currently under development. We have developed web-interface to access standardized metadata and experiments description. Namely, we have gathered, extended, and standardized metadata on a total of 32 relevant pre-eclampsia related microarray experiments from ArrayExpress, which is more than 1000 biological samples. The results are stored in Postgres database. Data can be accessed via either admin or user interface.

User’s web-interface at its current stage can be found <a href="http://194.44.31.241:24173/">here</a>.

Watch for updates at project's <a href="https://github.com/Sashkow/placenta-preeclampsia/">GitHub page</a>.