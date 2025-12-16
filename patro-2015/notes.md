# Salmon: Accurate, Versatile and Ultrafast Quantification from RNA-seq Data using Lightweight-Alignment

## Summary

## Notes

### Possible inputs

Salmon can analyze pre-aligned data (e.g. in the form of bam/sam files), or can perform the alignment itself after creating a salmon transcriptome index.

One approach is to use contigs assembled from the metatranscriptome itself as the index database, and to use the Salmon algorithm to then quantify each of the transcripts (contigs).

### Transcript quantification doesn't need optimal alignments, p. 7, para. 2

Transcript quantification only requires knowing which transcripts and positions within each transcript match a read reasonably well. 

Salmon performs a "lightweight assembly" that involved finding chains of super-maximal exact matches between reads and transcripts in the index.
