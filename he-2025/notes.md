# metaTP: a meta-transcriptome data analysis pipeline with integrated automated workflows

## Summary

Describes a metatranscriptomic analysis pipeline that combines various popular analysis tools using "Snakemake".

## Notes

### Pipeline overview, p. 3, fig. 1

First, raw reads are quality trimmed with trimmomatic and rRNA reads are removed using "bowtie2". Then, assembly is performed with "megahit" and ORFs are predicted with "TransDecoder". Next, assembled transcripts are quantified with "salmon". Next differentially expressed transcripts are detected and functionally annotated using "eggNOG-mapper".
