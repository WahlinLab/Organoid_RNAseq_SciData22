# Agarwal et al., Scientific Data 2022

This repository contains code used for quality control and data analysis presented in: 

> **Agarwal D, Kuhns R, Dimitriou CN, Barlow E, Wahlin KJ, Enke RA. Bulk RNA sequencing analysis of developing human induced pluripotent cell-derived retinal organoids. Scientific Data 2022 (in prep).**

----

## Data availability

Data is available in NCBI SRA under the accession number (https:).

## Software used

| Software | Version | URL | 
| --- | --- | --- |
| FastQC | 0.11.5 | http://www.bioinformatics.babraham.ac.uk/projects/fastqc/ |
| MultiQC | 1.11 | https://multiqc.info|
| HISAT2-index-align | 2.2.1 | http://daehwankimlab.github.io/hisat2/ |
| featureCounts | 2.0.3 | http://subread.sourceforge.net/ |
| DESeq2 | 1.36 | http://www.bioconductor.org/packages/release/bioc/html/DESeq2.html |

## Data analysis walkthroughs & code

Walkthroughs and code used for all of the quality assessment and data analysis steps are available in each of the below links.

1. [Quality assessment with FastQC](https://github.com/ScottSchumacker/Schumacker2019_Sci_Data/blob/master/Walkthroughs/FastQC-Instructions)
2. [Sequence trimming with Trimmomatic](https://github.com/ScottSchumacker/Schumacker2019_Sci_Data/blob/master/Walkthroughs/Trimmomatic-Instructions)
3. [Quality Analysis summary with MultiQC](https://github.com/ScottSchumacker/Schumacker2019_Sci_Data/blob/master/Walkthroughs/MultiQC-Instructions)
3. [Quantitation with kallisto](https://github.com/ScottSchumacker/Schumacker2019_Sci_Data/blob/master/Walkthroughs/Kallisto-Instructions)
4. [Normalization, visualization, and differential expression analysis with sleuth](https://github.com/ScottSchumacker/Schumacker2019_Sci_Data/tree/master/R)
