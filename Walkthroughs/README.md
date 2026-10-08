# FastQC Instructions

1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard) open applications and load FastQC.
2. Name the analysis and select the appropriate output folder.
3. Input .fastq files and run FastQC.

# MultiQC Instructions

1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard) open applications and load MultiQC.
2. Name the analysis and select the appropriate directory where FastQC results are stored.
3. Click Next, confirm the output directory for MultiQC results, and start MultiQC using the Launch Analysis button.

# HISAT2 Genome Alignment

1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard) open applications and load HISAT2-index-align-2.1.
2. Name the analysis and click Next to set run parameters.
3. Upload the .fasta genome file from a source such as NCBI (for example, the human genome assembly file can be found [here](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000001405.39/). Make sure to also download the corresponding genome annotation file (.gtf or .gff).
4. Select the paired end .fastq files that need to be aligned. Make sure to choose paired-end (PE) as the file type.
5. Click Next, confirm the output directory for HISAT2 results, and start HISAT2 using the Launch Analysis button.

# Transcript counting via featureCounts

1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard) open applications and load featureCounts.
2. Name the analysis and select the appropriate directory where featureCounts output will be stored.
3. Click Next, check the box for paired-end reads, and upload the genome annotation file corresponding to the genome downloaded above (.gtf or .gff).
4. Choose all the .bam files resulting from HISAT2 that need to be counted.
5. Click Next and start featureCounts using the Launch Analysis button.

# Differential Gene Expression Analysis using DESeq2

Before using DESeq, combine all the .tabular files from featureCounts:
1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard), open applications, search for "Join multiple tab-delimited files".
2. Select your .tabular files.
3. Specify the column number (key) that matches between both files; in this case, it is the gene name column.
4. Launch the tool to generate your merged file.

Now we proceed to DESeq2:
1. In [Cyverse Discovery Environment](https://de.cyverse.org/dashboard) open applications and load DESeq2.
2. Name the analysis and select the appropriate directory where DESeq2 output will be stored.
3. Select the combined .tabular file from featureCounts that needs to be analyzed. 
4. In the experiment design section, add a comma-separated list of sample names (factors) from the tabular file. If you want to include replicates in your analysis, enter the same name for each replicate. If you use different names, the factors will NOT be treated as replicates. Add a comma-separated list of library types for each of the factors listed above. For this analysis, use "paired-end" for each entry.
5. Click Next and start DESeq2 using the Launch Analysis button.
Note: All DESeq2 output, including pairwise comparisons and normalized counts for the samples from the paper, is available in this GitHub repository.

