# Agarwal et al., Scientific Data 2022

This repository contains code used for quality control and data analysis presented in: 

> Agarwal, D.; Kuhns, R.; Dimitriou, C.N.; Barlow, E.; Wahlin, K.J.; Enke, R.A. Bulk RNA Sequencing Analysis of Developing Human Induced Pluripotent Cell-Derived Retinal Organoids. *Sci Data **2022**, 9*, 759, https://doi.org/10.1038/s41597-022-01853-x.

----

## Data availability

Data is available in NCBI Sequence Read Archive (SRA) under the BioProject accession # PRJNA754196 (https://www.ncbi.nlm.nih.gov/bioproject/PRJNA754196).

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

1. [Quality assessment with FastQC](https://github.com/WahlinLab/Organoid_RNAseq_SciData22/tree/main/Walkthroughs)
3. [Quality analysis summary with MultiQC](https://github.com/WahlinLab/Organoid_RNAseq_SciData22/tree/main/Walkthroughs)
3. [Reference genome alignment with HISAT2](https://github.com/WahlinLab/Organoid_RNAseq_SciData22/tree/main/Walkthroughs)
4. [Assign sequence reads to features with featureCounts](https://github.com/WahlinLab/Organoid_RNAseq_SciData22/tree/main/Walkthroughs)
5. [Quantify differentially expressed transcripts with DESeq2](https://github.com/WahlinLab/Organoid_RNAseq_SciData22/tree/main/Walkthroughs)
