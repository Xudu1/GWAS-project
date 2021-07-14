# GWAS-project

##Individual project

##General Methods

## SNP filtering

SNPs in the VCF file were filtered using vcftools (version 1.9). SNPs with a minor allele frequency (MAF) of less than 5% and samples with a genotyping rate of less than 90% were excluded. Ultimately, only 94 isolates meeting the filtering criteria were retained from over 420 individual isolates. 

## Phenotype data processing

Manual exclusion of samples with missing values was followed by normalisation of the phenotype data Nec, Pyc, and STB in R. Using two methods normalization and standardization to rescale the phenotype data.

## Population stratification analysis

In plink, the VCF files containing the filtered SNPs were transformed to Map and Ped files (version 1.9). These two files were used to generate the bed, fam, and bim files in plink. The piplines of admixture were used to stratify the population structure of the bed files. 

## GWAS analysis

Using pipelines from Tassel to conduct association analysis between fungal SNPs and phenotypic data for 20 cultivars.
