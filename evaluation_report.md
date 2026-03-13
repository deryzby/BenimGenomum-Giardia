# Evaluation Report

## Selected Organism and Rationale
I selected *Giardia duodenalis* because it has a relatively small genome and is suitable for a first genome assembly project. Small eukaryotic genomes are easier to analyze than plant or vertebrate genomes. In addition, *Giardia* is biologically important as an intestinal protozoan parasite.

## Data Source
- Organism: *Giardia duodenalis*
- Run accession: SRR26410993
- Source: NCBI / ENA public sequencing databases
- Sequencing type: long-read whole genome sequencing data

## Workflow Used
Although the original guide suggested GenoDiplo/Snakemake, in this project I used an equivalent manual workflow:
1. Download raw sequencing data
2. Perform quality control with FastQC
3. Assemble the genome with Flye
4. Evaluate assembly quality with QUAST
5. Compare the assembly to a reference genome with QUAST

## Assembly Results
- Total assembly length: 11,716,747 bp
- Number of contigs: 23
- Largest contig: 2,951,713 bp
- N50: 2,412,838 bp
- GC content: 49.8%

## Reference-Based QUAST Results
- Reference length: 12,078,186 bp
- Genome fraction: 97.324%
- Duplication ratio: 1.009
- Misassemblies: 59
- Misassembled contigs: 7
- Unaligned contigs: 3 + 7 part
- Unaligned length: 138,132
- Total aligned length: 11,466,550
- Mismatches per 100 kbp: 70.21
- Indels per 100 kbp: 471.64

## Interpretation
The final draft assembly is consistent with the expected genome size of *Giardia* and shows strong agreement with the reference genome. The GC content is nearly identical to the reference. The assembly recovers 97.3% of the reference genome, which indicates a strong draft-level assembly. Although several misassemblies were detected, this is acceptable for a student-level draft genome project and may reflect repetitive or structurally complex regions.

## Problems Encountered and Solutions
1. FastQC initially failed because of memory limits. This was solved by rerunning with increased memory allocation.
2. Flye could not be installed in the base environment due to dependency conflicts. A separate Conda environment was created.
3. QUAST also required a separate environment because of package conflicts.
4. GitHub terminal authentication failed with a normal password. A GitHub Personal Access Token was used instead.
5. The Git remote URL initially pointed to the wrong repository name and was corrected.

## What I Would Explore Next
If I continued this project, I would next perform BUSCO analysis to estimate genome completeness, then attempt basic genome annotation and compare possible strain-specific regions against the reference genome.

