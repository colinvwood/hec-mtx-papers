# Metatranscriptomics for the Human Microbiome and Microbial Community Functional Profiling

## Summary

## Notes

### Metatranscriptomics requires deeper sequencing than metagenomics, p. 286, para. 1

The authors argue that 10,000 fold deeper sequencing is required if both organsims and transcripts exist each in an abundance range of 100-fold differences. For this reason many metatranscriptomics protocols are biased towards the most abundanct transcripts. The authors suggeset that rule of thumb is that a metatranscriptomics analysis should get 10x the sequencing depth of the accompanying metagenomics analysis.

### Quality control is similar to metagenomics, p. 286, para. 2

Quality trimming and filtering, adapter trimming, and host read removal can be performed in much the same way as it is in metagenomics pipelines. Two tools for computationally removing rRNA are "SortMeRNA" and "barrnap". The "KneadData" tool is a pipeline that can perform various quality control steps for metatranscriptomic data.

### Read mapping tools, p.287, para. 3

Tools for quantifying features (transcripts, gene families, etc.) from sequences include "MetaCLADE", "SAMSA2", and "HUMAnN". 

### Assembly strategies, p. 287, para. 4

When paired metagenomic sequencing is available, the DNA sequences can be assembled and then the metatranscriptomic reads can be mapped to them. Or, the metatranscriptomic reads can be assembled directly. However, there are few tools that have been designed and validated specifically for this task. One should expect a large proportion of the metatranscriptomic reads (~50%) to go unused in the assembly process and only the most abundant transcripts to be fully assemble-able. 

### Control for metagenomic abundance during differential analysis, p. 288, para. 3

Because the number of genes encoding a transcript can vary between samples it is important to control for metagenomic abundance differences between samples (if paired metagenomic sequencing is performed) before concluding differential expression.

### Normalization strategies, p. 288, para. 4

Because functional activity depends so strongly on genomic gene abundance it is crucial to estimate relative expression of a function ("the degree to which it is over- or under expressed in a metatranscriptome relative to the abundance of community genes encoding the function"). One approach is to normalize transcripts within the species that they come from, if this is known. Another strategy, when paired metagenomic sequencing data is available, is to directly normalize each gene's or gene family's abundance by its corresponding DNA abundance. This approach has the advantage that it works even when the taxonomy of the gene is unknown.
