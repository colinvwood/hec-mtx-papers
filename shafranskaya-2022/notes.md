# MetaGT: A pipeline for de novo assembly of metatranscriptomes with the aid of metagenomic data

## Summary

Describes a novel pipeline that leverages paired metagenomic and metatranscriptomic sequenced samples to improve the de novo assembly of transcripts.

## Notes

### Pipeline overview, p. 2, para. 5

The MetaGT pipeline first assembles metagenomic reads and metatranscriptomic reads separately, using metaSPAdes and rnaSPAdes respectively. Then, the metatranscriptomic contigs are mapped to the metagenomic contigs using "minimap2" to extend and correct the metatranscriptomic contigs into longer length transcripts. Metagenomic contigs are annotated with "Prokka" and unannotated metatranscriptomic contigs are annotated with "TransDecoder". All contigs are then clustered with "MMseqs2" and quantified with "Kallisto". 

### Transcript correction process, p. 2, para. 7

Metatranscriptomic contigs are aligned to predicted metagenomic coding regions. Such predicted genes that are covered by incompletely assembled or fragmented metatranscriptomic contigs are corrected by concatenating fragmented transcripts and filling in missing subsequences. Only metagenomic coding regions with at minimum certain percentage coverage of metatranscriptomic contigs are processed in this way (50% coverage by default). Transcripts that map beyond the edges of predicted coding regions are truncated. 

### Effectiveness, p. 5, table 2 

MetaGT showed on average ~10% fewer assembled contigs, ~15% fewer unaligned contigs (when mapping assembled metatranscriptomic contigs to the reference genomes), and a ~15% increase in the number of captured reference transcripts.
