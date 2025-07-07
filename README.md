# Variant Calling Pipeline

This Python script automates a full variant calling workflow from raw FASTQ reads to annotated VCF using:

- **Trimmomatic** for quality trimming  
- **BWA** for genome alignment  
- **SAMtools** for file conversion and indexing  
- **GATK HaplotypeCaller** for variant calling  
- **SnpEff** (via Docker) for variant annotation

## Requirements

- Java
- BWA
- SAMtools
- GATK (local installation)
- Docker
- Reference genome: `Homo_sapiens.GRCh38.dna.primary_assembly.fa`
- Paired-end FASTQ files (e.g., `001_R1.fastq`, `001_R2.fastq`)

## Notes

> 🔹 This version of the script processes **a single sample** due to storage limitations on my HPC account.  
> 🔹 However, the full pipeline was used to process **26 patient samples** during my Master's project.

Each step is modular and wrapped in a Python function using `subprocess`.

## Author

**Hayfa Bououd**



