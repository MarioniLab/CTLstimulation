# MassSpecCTLstimulationActD

This directory contains an Rmarkdown file to analyze proteomics data from in vitro-differentiated murine cytotoxic T lymphocytes (CTLs) at rest and stimulated 4 hours with anti-CD3 in the presence of actinomycin D to block transcription or DMSO vehicle control.

## Preparing data and directories

The script uses as input the files JM-DIA_v14_report.csv and experimental_design.xlsx that should be downloaded from the PRIDE repository, project number PXD034920, and placed in the top level directory.

To run the script, also create a directory called "plots_and_tables" within the repository.

## Scripts

Run the script CTLActD_proteomics_analyses.Rmd to generate all analyses and figures for this dataset.

Note that this script performs a comparison with results of RNAseq analysis also in this repository, and so these should be run first to enable generation of this figure.

Of note, enrichment analysis was performed using the Panther classification tool outside of R as described in the Rmarkdown file.