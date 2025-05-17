# Metagenomics Pipeline

This project is a Snakemake-based pipeline for taxonomic classification of raw DNA sequencing data using tools like FastQC, Fastp, and Kraken2.

## Features

- Automates quality control, trimming, and classification steps
- Uses MiniKraken database for lightweight taxonomic analysis
- Tracks workflow dependencies with Conda
- Simple configuration and modular structure

## Tools

- [Snakemake](https://snakemake.readthedocs.io)
- Conda (for environment management)
- SRA Toolkit (`prefetch`, `fasterq-dump`)
- Tools: `fastqc`, `fastp`, `kraken2`

## Usage

```bash
snakemake --cores 2 --snakefile workflow/Snakefile
