# rnaSPAdes: a de novo transcriptome assembler and its application to RNA-seq data

## Summary

Describes changes made to the SPAdes algorithms that result in a new assembler (rnaSPAdes) adapted to single-cell transcriptome assembly.

## Notes

### Benchmarking datasets, p. 2, para. 6

The datasets used to assess the performance of rnaSPAdes are all single organism datasets. The variables among the datasets include organism, read length, sequencing depth, and insert size--but not phylogenetic diversity. Thus rnaSPAdes was clearly developed for single organism transcriptome assembly.  

### Tip trimming changes, p. 7, para. 4

In genomic assembly tips in the de Bruijn graph most commonly represent sequencing error and true reasons for tips (end of chromosome or coverage gap) are rare, so tip trimming is aggressive. In transcriptome assembly tips are expected to be more commonly correct because of the many distinct (non-contiguous) transcripts. Thus lower coverage and length thresholds are used in rnaSPAdes compared to SPAdes.

### Bulge collapsing changes, p. 7, para. 8

The rnaSPAdes algorithm only collapses bulges with small differences in edge length (<10%) because it assumed these are possibly due to sequencing error, while bulges that show a greater difference between edge lengths could be due to alternative spliced isoforms.

In the context of metatranscriptome assembly bulges could exist for the additional reason of separate but homologous transcripts. Where these transcripts also differ in coverage due to differential expression it will be difficult to differentiate the cause from sequencing error.
