# Early Neurodevelopmental Drivers of Autism: A Transcriptomic Analysis of Chd8 Dysregulation

## Project Overview
This project performs an exploratory transcriptomic analysis of the **Chd8** gene, a high-risk factor for Autism Spectrum Disorder (ASD). Using mouse model data (GSE263334), I analyzed gene expression changes during the **E14 embryonic stage**—a critical window for neurogenesis. 

As a professional with experience in **special education**, my goal was to bridge the gap between molecular biology and neurodevelopmental outcomes to better understand the "genetic blueprint" that shapes diverse learning and behavioral profiles.

## Dataset
*   **Source:** [GEO GSE263334](https://www.ncbi.nlm.nih.gov)
*   **Model:** Mouse (Mus musculus) - Embryonic Brain Tissue
*   **Condition:** Chd8 Knock-In (KI) vs. Wild-Type (WT)
*   **Stage:** E14 (Embryonic Day 14)

## Key Questions
1. Which genes are significantly up- or down-regulated when *Chd8* is overexpressed?
2. What is the magnitude (Fold Change) and statistical confidence (p-value) of these changes?
3. How do these molecular shifts relate to the foundational development of the autistic brain?

## Technical Workflow
1.  **Data Acquisition:** Programmatic retrieval of supplementary DESeq2 results using `GEOquery`.
2.  **Data Preprocessing:** Cleaning and reformatting matrix structures, mapping gene IDs to row names.
3.  **Statistical Filtering:** Applying thresholds of $p_{adj} < 0.05$ and $|log_2FoldChange| ≥ 1$.
4.  **Visualization:** Generation of a Volcano Plot using `ggplot2` to map the transcriptomic landscape.

## Results & Discussion Summary
This analysis isolated a subset of genes where expression was at least doubled or halved. As a "master regulator," the dysregulation of *Chd8* creates a downstream ripple effect. In a classroom context, this reinforces that neurodivergence is not a "breakdown" in development, but a result of an altered genetic instruction manual during the earliest stages of brain formation.

## Tools Used
*   **Language:** R
*   **Libraries:** `DESeq2`, `tidyverse`, `GEOquery`, `ggplot2`
