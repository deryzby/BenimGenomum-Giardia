# Final Project Summary

## Project Title
Draft Genome Assembly and Quality Assessment of *Giardia* Using Public Sequencing Data

## Objective
The aim of this project was to perform a draft genome assembly of *Giardia* using publicly available sequencing data and to evaluate assembly quality with standard bioinformatics tools.

## Data Source
- Organism: *Giardia*
- Run accession: SRR26410993
- Source: NCBI / ENA public sequencing database

## Workflow
1. Raw sequencing data were downloaded from the public archive.
2. Read quality was checked using FastQC.
3. Draft genome assembly was generated using Flye.
4. Assembly quality was evaluated using QUAST.
5. Results and workflow were documented in GitHub.

## Main Results
- Total assembly length: 11,716,747 bp
- Number of contigs: 23
- Largest contig: 2,951,713 bp
- N50: 2,412,838 bp
- L50: 3
- GC content: 49.8%
- N per 100 kbp: 0

## Interpretation
The total assembly length is consistent with the expected genome size of *Giardia*.
The QUAST statistics indicate that the draft assembly is of good quality for an educational and comparative bioinformatics project.

## Tools Used
- WSL2 / Ubuntu
- Conda
- FastQC
- Flye
- QUAST
- Git / GitHub

## Conclusion
This project successfully produced a draft genome assembly of *Giardia* from public sequencing data and demonstrated a complete basic genome assembly workflow from raw reads to assembly evaluation.

