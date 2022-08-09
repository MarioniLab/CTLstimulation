# RNAseqCTLstimulation

This directory contains an Rmarkdown file to analyze RNAseq data of in vitro-differentiated murine cytotoxic T lymphocytes (CTLs) at rest and stimulated for 10, 20, 40 and 60 minutes with anti-CD3.

## Preparing data and directories

The script uses as input a counts table "counts_ArrayExpress.csv" and sample information table "sdrf.txt" that should be downloaded from ArrayExpress (accession number E-MTAB-12083) and placed in the top level directory.

Obtain the necessary annotation files and put in the annotation_resources directory:
UCSC tables: ensGene and ensemblToGeneName tables for mm10 genome (I downloaded on 18/3/16); name them as follows: "ucsc_mm10_ensGene" and "ucsc_mm10_ensemblToGeneName"
Note: Because these files are no longer available via UCSC, an alternative annotation method is provided in the script.

To run the script, also create a directory called "plots_and_tables" within the repository.

## Scripts

Run the script CTLstimulation_RNAseq_analyses.Rmd to generate all analyses and figures for this dataset.

Of note, enrichment analysis was performed using the Panther classification tool outside of R as described in the script.