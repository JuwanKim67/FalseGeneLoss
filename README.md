# FalseGeneLoss
[FalseGeneLoss.py]
Version 1.0

- (1) To do: compare annotation of different assemblies of the same species
- (2) OS: Ubuntu 18.04.3 LTS (GNU/Linux 5.4.0-42-generic x86_64)
- (3) Necessary input files:

[mandatory]
- Assembly A from NCBI (.fasta, should be softmasked by windowmasker)
- Assembly A's annotation from NCBI (.gff)
- Assembly B (.fasta, should be softmasked by windowmasker)
- Assembly B's annotation from CAT (.gff, Comparative annotation toolkit; https://github.com/ComparativeGenomicsToolkit/Comparative-Annotation-Toolkit)
- Hal file from the cactus alignment between Assembly A & B (.hal)
- Bam file of assembly A with illumina genomic reads (.bam, should be sorted and indexed)
- Bam file of assembly B with illumina genomic reads (.bam, should be sorted and indexed)
- NCBI gap coordinate file of assembly A
- NCBI gap coordinate file of assembly B
- CAT working directory and out directory

[optional]
- (if want to perform false indel/SNP analyses) false indel/SNP bed file based on assembly A
- (if want to compare NCBI remap result with cactus) NCBI remap excel file

(4) variable_suffix:
- [variable name]_s: string
- [variable name]_chr: character (=length 1 string)
- [variable name]_l: list
- [variable name]_nl: nested list
- [variable name]_i: integer
- [variable name]_bool: boolean
- [variable name]_d: dictonary
- [variable name]_f: file
- [variable name]_fl: float
- [variable name]_rec: gffutils record
