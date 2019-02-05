# curatedTCGAData: integration of The Cancer Genome Atlas data in Bioconductor

February 7, 2019
BiocNYC R/Bioconductor meet-up

Marcel Ramos and Levi Waldron

curatedTCGAData is a Bioconductor experiment data package built using The
Cancer Genome Atlas data and RTCGAToolbox to provide integrative, curated, and
ready-to-use datasets. TCGAutils is a companion package for working with
several aspects of TCGA data including the translation of patient identifiers,
conversion of gene symbols to genomic ranges, and provision of useful metadata
to facilitate the understanding of TCGA assays and annotation.

To install the workshop dependencies on your own RStudio desktop (the first line
installs experimental data packages not installed automatically):

```
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(
    c("org.Hs.eg.db", "mirbase.db", "EnsDb.Hsapiens.v86")
)

BiocManager::install(
    "waldronlab/curatedTCGAWorkshop",
    dependencies = TRUE
)
```
