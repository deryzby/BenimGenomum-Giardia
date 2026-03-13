# Troubleshooting and Solutions

## 1. FastQC memory error
### Problem
FastQC terminated with `java.lang.OutOfMemoryError: Java heap space`.

### Solution
FastQC was rerun with increased memory allocation:
```bash
fastqc --memory 4096 SRR26410993_1.fastq

