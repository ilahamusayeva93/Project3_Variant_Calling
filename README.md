## Project 3: Variant Calling

Course: BIOL 4150 / BIOL 6150

Overview

This project focuses on variant calling using high-throughput sequencing data. Starting from aligned sequencing reads, the workflow includes quality assessment, pileup generation, variant calling, and filtering. The project builds on prior work in Project 2 (Read Mapping) to analyze genomic variants, such as SNPs and indels, and assess their quality and depth.

Details

Estimated Time: ~1.5 hours
Environment Configuration
Processor: Intel(R) Xeon(R) Gold 6226 CPU @ 2.70GHz
Cores: 24 (12 cores per socket, 2 sockets)
Memory: 754 GB
Storage: 50 TB (network-mounted) and 1.4 TB (local)
Repository Contents

Starter Notebook: Project3-VariantCalling.ipynb
Includes all required tasks, questions, and placeholders for commands. Do not delete any comments or information boxes.
Input Files:
SRR081224_sorted.sam: Sorted SAM file from Project 2.
SRR081224.bam: Converted BAM file for efficient processing.
hg38.fa: GRCh38 human reference genome.
Output Files:
Pileup File: SRR081224.pileup
SNP VCF File: snps.vcf
Indel VCF File: indels.vcf
Filtered SNP and Indel Files:
snps_depth_gt_50.vcf
indels_depth_gt_50.vcf
Objectives

Quality Assessment
Ensure proper sorting and quality of SAM/BAM files.
Generate basic statistics using SAMtools Flagstat.
Pileup Generation
Convert aligned reads to pileup format.
Understand pileup format fields and their significance for variant calling.
Variant Calling
Use VarScan for identifying SNPs and short indels.
Interpret VCF files and assess variants by depth and quality.
Filtering and Visualization
Apply thresholds to select high-confidence variants.
Visualize read count distributions across genomic regions.
Instructions

Clone the Repository
git clone https://github.com/ilahamusayeva93/Project-3-Variant-Calling
cd Project-3-Variant-Calling
Prepare the Environment
Ensure SAMtools and VarScan are installed.
Confirm the presence of required input files (SRR081224_sorted.sam, hg38.fa).
Follow the Starter Notebook
Complete each task step-by-step as outlined in Project3-VariantCalling.ipynb.
Do not delete any comments or placeholders in the notebook.
Generate Outputs
Pileup File: Convert SAM/BAM files to pileup format.
Variant Calling: Call SNPs and indels.
Filtering: Extract high-confidence variants based on depth and quality.
Visualization
Plot read count distributions for specific chromosomes.
Expected Outputs

Intermediate Files:
Pileup File: SRR081224.pileup
SNP VCF: snps.vcf
Indel VCF: indels.vcf
Filtered Variants:
SNPs with Depth > 50: snps_depth_gt_50.vcf
Indels with Depth > 50: indels_depth_gt_50.vcf
Visualizations:
Read count distribution plot for Chromosome 20.
