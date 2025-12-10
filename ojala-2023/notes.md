# Current concepts, advances, and challeneges in deciphering the human microbiota with metatranscriptomics

## Summary
This paper provides an overview of metatransciptomics as it is applied to human-associated microbial communities. 

## Notes

### Overview of wet-lab process, p. 687, fig. 1A

The metatranscriptomic wet-lab process can be outlined as follows. First is sample collection. Next is sample preservation, where an RNA-stabilizing solution which inactivates DNases, RNases, and proteases, and stabilizes RNA is added to the sample. Next is sample disruption, which releases RNA trapped in cells into an exogenous solution; options include mechanical (e.g. bead beating), chemical, end enzymatic (e.g. lysis enzymes) approaches. Next is total RNA extraction, where RNA molecules are purified from the other biological moclecules, many different approaches are possible. Next is rRNA depletion, where ribosomal RNA is removed to allow relative enrichment of mRNA, different techniques are possible. Next is host RNA depletion where RNAs from a host organism, if present, are removed, different techniques are possible. Next is library preparation, where the RNAs of interest are prepare to be sequenced; the details of this step depend heavily on the sequencing technology that will be used. The final step is sequencing; the major categories are next-generation and third-generation sequencing.

### Overview of data analysis process, p. 687, fig. 1B

The metatranscriptomic data analysis process can be outlined as follows.
First is preprocessing and quality control, where synthetic sequences are removed, quality-score filtering is performed, and contaminants are identified and removed. Next is unwanted read removal, where specific types of RNAs that are not of interest are filtered, e.g. host RNAs, rRNA, or tRNA. Next is de novo assembly where reads are combined into longer transcript contigs. An alternative step is read mapping, where reads are aligned directly to known genomes to identify and quantify active genes. Next is gene prediction where assembled contigs have their coding regions predicted. Next is taxonomic and functional assignment, where reads/contigs are taxonomically and functionally classified, which can then allow taxa and functions to be quantified. The final steps are study-specific and can include a wide variety of bioinformatic and statistical tools.

### Contamination control, p. 691, box 2

The most effective way to detect contamination is to use negative controls. Negative controls should be used at multiple steps in the wet-lab process, including extraction and sequencing. Positive controls can be used to assess loss of non-contaminant nucleic acids. Negative and positive controls should be created to mimic the charactersitics of the true samples.

### Sequencing depth, p.692, para. 3

Metatransciptomics requires greater sequencing depth than metagenomics.
One rule of thumb is that 10 times the depth of metagenomic sequencing for the same samples. The reason that the depth requirement is greater is that metatranscriptomics must accomodate two abundance continuums: the relative abundances of species (groups of cells) and the relative abundances of transcripts within each cell--metagenomics only has to accomodate the former. Two cited studies have per-sample depths of 1 million and 250 million reads.
