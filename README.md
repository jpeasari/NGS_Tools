# NGS_Tools

## Basic Linux commands

## blast

Installation from https://anaconda.org/bioconda/blast : ***conda install -c bioconda blast*** \
Documentation : https://www.ncbi.nlm.nih.gov/books/NBK279690/ 
>
Performing blast: \
Step 1: Creating a database locally - ***makeblastdb -in reference_sequences.fasta -out your_database_name -dbtype nucl -parse_seqids*** \
replace nucl to prot to create database with amino acid sequences 
>
Step 2: Performing blast - ***blastn -query query.fasta -db your_database_name -out blast_result_file_name.out -outfmt 6*** \
replace blastn to blastp to perfomr protein blast 
>
Links to understand blast output:
>
https://www.biostars.org/p/88944/  
http://www.metagenomics.wiki/tools/blast/blastn-output-format-6

## Getting NGS data

### SRA tool-kit

Installation from https://anaconda.org/bioconda/sra-tools: ***conda install -c bioconda sra-tools*** \
Documentation: https://trace.ncbi.nlm.nih.gov/Traces/sra/sra.cgi?view=toolkit_doc \
fasterq-dump : https://github.com/ncbi/sra-tools/wiki/HowTo:-fasterq-dump \
>
Commands: \
***wget paste_hyperlink_here*** \
***fastq-dump SRRXXXXXX*** \
***fastq-dump -I --split-files SRRXXXXXX*** - for paired end data \
***fasterq-dump SRRXXXXXX*** \
***fasterq-dump -I --split-files SRRXXXXXX*** - for paired end data \
>
## Quality Control
### fastqc
>
Installation from https://anaconda.org/bioconda/fastqc : ***conda install -c bioconda fastqc*** \
Tool websource : https://www.bioinformatics.babraham.ac.uk/projects/fastqc/ \
Mannual: https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/ \
Video Tutorial: https://www.youtube.com/watch?v=bz93ReOv87Y&ab_channel=BabrahamBioinf 
>
Command: \
***fastqc file_name.fastq*** 
>
### multiqc
>
Installation from https://anaconda.org/bioconda/multiqc : ***conda install -c bioconda multiqc*** \
Tool websource : https://multiqc.info/ \
Documentation: https://multiqc.info/docs/ \
Command: ***multiqc .*** 
>
### fastp
>
Installation from https://anaconda.org/bioconda/fastp: ***conda install -c bioconda fastp*** \
Documentation: https://academic.oup.com/bioinformatics/article/34/17/i884/5093234 \
GitHub page: https://github.com/OpenGene/fastp \
fastp video tutorial : https://www.youtube.com/watch?v=VrIW4EcHly4&ab_channel=MakeTheBrainHappy-ScientificExploration 
>
Basic commands: \
Single end: ***fastp -i read.fq -o out.fq*** \
Paired end: ***fastp --in1 read1.fq --in2 read2.fq*** 

### Qualimap
>
Installation from https://anaconda.org/bioconda/qualimap : ***conda install -c bioconda qualimap*** \
Tool websource: http://qualimap.conesalab.org/ \
Mannual: http://qualimap.conesalab.org/doc_html/index.html \
Command:\
***./qualimap bamqc -bam bam_file.bam -gff gene_annotation.bed -outdir qualimap_results -outformat pdf*** \




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






