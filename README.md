# Giardia-Genome-Assembly

This repository documents a genome analysis project conducted using publicly available sequencing data for *Giardia*. The project follows a step-by-step bioinformatics workflow starting from raw sequencing reads to genome assembly and basic quality evaluation.

## Project Goal

The goal of this project is to explore and document the fundamental steps involved in genome analysis, including data acquisition, quality control, genome assembly, and assembly evaluation.

## Organism

*Giardia*

## Sequencing Data

- Run accession: SRR26410993  
- Data source: NCBI / ENA Sequence Read Archive (SRA)  
- Library strategy: Whole Genome Sequencing (WGS)  
- Library source: Genomic DNA  

## Computational Environment

The analysis is performed using the following tools and environment:

- WSL2 with Ubuntu
- Conda / Miniconda
- SRA Toolkit
- FastQC
- GenoDiplo
- Snakemake
- QUAST

## Workflow Overview

The project follows these main steps:

1. Downloading raw sequencing data from public repositories  
2. Quality control of raw sequencing reads  
3. Read preprocessing (if required)  
4. Genome assembly  
5. Assembly quality assessment  
6. Documentation of the workflow  

## Project Status

Project setup and initial data acquisition are currently in progress.
## Assembly Results

Draft genome assembly was generated using Flye and evaluated with QUAST.

### Assembly statistics

- Total length: 11,716,747 bp
- Number of contigs: 23
- Largest contig: 2,951,713 bp
- N50: 2,412,838 bp
- L50: 3
- GC content: 49.8%
- N per 100 kbp: 0

### Interpretation

The assembly size is consistent with the expected genome size of *Giardia*.
QUAST results suggest that the assembly is suitable as a draft genome assembly for downstream analysis and project presentation.

