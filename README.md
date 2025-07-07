# HayfaB
Python-based pipeline for variant calling from FASTQ to annotated VCF using Trimmomatic, BWA, GATK, and SnpEff.
Title: Variant Calling Pipeline in Python

Description:
This Python script automates a full variant calling workflow using:
- Trimmomatic for quality trimming
- BWA for genome alignment
- SAMtools for file conversion and indexing
- GATK HaplotypeCaller for variant calling
- SnpEff (via Docker) for variant annotation

The pipeline was developed as part of a training project during my Master's program in Bioinformatics.

Requirements:
- Java, BWA, SAMtools, GATK (local installation), Docker
- Reference genome: Homo_sapiens.GRCh38.dna.primary_assembly.fa
- Paired-end FASTQ files 

Each step is modular and wrapped in a function. The script is run from the command line and includes basic file handling and subprocess management.
Note:
This script is a simplified version applied to a single sample (one patient) for demonstration purposes, due to limited storage space on my HPC account. However, the full version of this pipeline was used to process sequencing data from 26 patients as part of my research project.

The full pipeline includes looping through multiple FASTQ files and handling multiple sample IDs in a batch format.


Author: Hayfa Bououd
