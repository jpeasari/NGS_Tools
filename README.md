# NGS_Tools

## Basic Linux commands

## blast

Installation from https://anaconda.org/bioconda/blast : ***conda install -c bioconda blast*** \
Documentation : https://www.ncbi.nlm.nih.gov/books/NBK279690/\

Performing blast: \
Step 1: Creating a database locally - ***makeblastdb -in reference_sequences.fasta -out your_database_name -dbtype nucl -parse_seqids*** \
replace nucl to prot to create database with amino acid sequences 

Step 2: Performing blast - ***blastn -query query.fasta -db your_database_name -out blast_result_file_name.out -outfmt 6*** \
replace blastn to blastp to perfomr protein blast 

Links to understand blast output:\ 
https://www.biostars.org/p/88944/  
http://www.metagenomics.wiki/tools/blast/blastn-output-format-6

## Getting NGS data

### SRA tool-kit


## Quality Control
### fastqc
### multiqc
### fastp
### Qualimap

## Read alignment

### STAR
### bowtie2
### hisat2
### BWA
### SPades
# Tophat2

## Quantification
### featureCounts
### Htseq2


## xxxtools
### samtools
### deeptools
### bedtools


## SNP analysis

## Chip-Seq






