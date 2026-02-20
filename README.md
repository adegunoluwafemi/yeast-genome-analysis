# Yeast Genome Analysis: Loading, Subsetting, and RNA-to-DNA Conversion

**Author:** Adegun Oluwafemi Joseph  
**Linkedin:** www.linkedin.com/in/oluwafemi-adegun 

**Date:** 2025-04-09

## Overview

This repository contains an R-based analysis of the *Saccharomyces cerevisiae* (baker's yeast) genome. It demonstrates:

- Loading the complete reference genome (sacCer3 assembly) using Bioconductor packages.
- Subsetting chromosomes and extracting specific regions.
- Converting between DNA and RNA sequences.

The analysis is fully reproducible and serves as a template for handling genome-scale data in R.

## Requirements

- R (version ≥ 4.0)
- Bioconductor packages: `Biostrings`, `BSgenome.Scerevisiae.UCSC.sacCer3`

Install the required packages with:

```r
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(c("Biostrings", "BSgenome.Scerevisiae.UCSC.sacCer3"))
