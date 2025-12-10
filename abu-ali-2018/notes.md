# Metatranscriptome of human faecal microbial communities in a cohort of adult men

## Summary

## Notes

### HUMAnN2 can analyze DNA and RNA reads, p. 357, para. 1

The authors note that in 929 metagenomic samples ~1.5 million UniRef90 gene families are detected and in 372 metatranscriptomic samples ~600k gene families are detected. HUMAnN2 is a complex pipeline that involves taxonomic assignment using marker genes, pangenome alignments, protein translated searches for reads that don't hit a taxonomic assignment, and metabolic pathway mapping.

### A large proportion of assigned gene families lacked characterization, p.357, para. 1

About 58% of gene families assigned through metatranscriptomic pipeline had "functional characterization." Weighted by relative abundance ~85% of gene families did not have "biochemical characterization." Considering that this is in the well-studied gut, we can likely expect much worse numbers in the composting data. In the years between this study and now gene familiy characterization coverage may have improved however.

### Simple statistic for assessing variance, p. 358, para. 2

The authors use an average proportion of gene families found per sample as a measure of variance. This is useful to get a sense of variability but also to compare between metagenomic and metatranscriptomic paired samples. As the authors note, because the average metatranscriptomic proportions is ~5% and the average metagenomic proportion is >10%, this indicates "only a subset of fecal functional potential is active." Other ratios would give other interesting insights, but sequencing depth can be a confounder.

### Core and variable metatranscriptome determination, p. 358, para. 3

Defining a prevalence threshold sorts gene families into core and variable groups, e.g. if a gene family is present in 80% or more of samples, then it is considered core. The authors found a smaller core metatranscriptome than core metagenome.

### Quality control significantly reduced total sequencing information, p. 364, para. 4

Quality control, made up of quality trimming/filtering and host read filtering (using the KneadData v0.3 quality control pipeline), reduced the amount of sequencing data from an average of 3 Gnt to 1.3 Gnt.
