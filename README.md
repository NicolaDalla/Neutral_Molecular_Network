# Neutral Molecular Networks (NMN)

This repository contains the R-based workflow developed for the paper:  

**Neutral Molecular Networks: polarity-independent tool for mass spectrometry data analysis**  
*Nicola Dalla Valle, Pietro Franceschi, Mar Garcia Aloy, Peter Robatscher, Michael Oberhuber*  

---

## Overview  

Untargeted metabolomics using mass spectrometry is typically performed separately in positive and negative ionization modes, which creates redundancy and limits chemical annotation.  

In this work, we introduce **Neutral Molecular Networks (NMNs)**, a strategy that:  
- Merges positive and negative mode MS/MS fragmentation spectra into **neutral pseudo-spectra**.  
- Builds polarity-independent molecular networks, fastening MS data analysis.  
- Improves chemical informativity, and compound annotation accuracy.  

The workflow is  implemented in R Markdown files, making it reproducible.  

---

## Repository Structure  

- **`libraries_neutral_spectra_creation.Rmd`**  
  Workflow to generate **neutral pseudo-spectra** by merging positive and negative mode spectra from public MS/MS libraries. 
  
- **`MNs_structure_metrics.Rmd`**  
  Scripts for computing network structure metrics (e.g., modularity, assortativity) from neutral pseuda-spectra generated in previous step.

- **`chemical_similairty_calcualtion.Rmd`**  
  Performs chemical similarity comparisons (Tanimoto & Overlay scores) to assess structural agreement of spectral matches.  

- **`subclass_prediction.Rmd`**  
  Subclass prediction from network neighborhoods based on majority vote for MSMS library.  

- *(To be added)* **Alternaria dataset analysis**  
  Case study on fungal metabolomics. Include: MS data processing, identification of neagtive/positive feature pairs and the demostration of NMN clustering of toxin-related metabolites.  

---
