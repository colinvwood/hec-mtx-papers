# SortMeRNA: fast and accurate filtering of ribosomal RNAs in metatranscriptomic data

## Summary

This paper describes an rRNA read filtering algorithm based on a burst trie.

## Notes

### Databases used, p. 3215, para. 3

Eight different databases are used by the software, including 16S & 18S, 23S and 28S and 5S & 5.8S subunits. The sequences come from the SILVA and RFAM databases. Or, user-provided databases can be used.

### Effectiveness, p. 3216, para. 1

On simulated Illumina reads the software was ~99.86% sensitive and ~99.99% selective, using an 85% identity 16S rRNA database with ~7.5k sequences.
