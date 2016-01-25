# intropolis

`intropolis` is a list of exon-exon junctions found across 21,504 human RNA-seq samples on the [Sequence Read Archive](http://www.ncbi.nlm.nih.gov/sra) from spliced read alignments to `hg19` with [Rail-RNA](http://rail.bio). Two files are provided:

A. ftp://ftp.toinsert.com/intropolis.v1.hg19.tsv.gz : a gzipped TSV with fields
  1. chromosome
  2. intron start position (1-based; inclusive)
  3. intron end position (1-based; exclusive)
  4. strand (+ or -)
  5. donor dinucleotide (e.g., GT)
  6. acceptor dinucleotide (e.g., AG)
  7. comma-separated list of indexes of samples in which junction was found
  8. comma-separated list of corresponding numbers of reads mapping across junction in samples from field 7

B. ftp://ftp.toinsert.com/intropolis.idmap.v1.hg19.tsv : a TSV with fields
  1. sample index used in field 7 of `intropolis.v1.hg19.tsv.gz`
  2. SRA project accession number
  3. SRA sample accession number
  4. SRA experiment accession number
  5. SRA run accession number

If you use `intropolis`, cite [*Human splicing diversity across the Sequence Read Archive*](http://bioarxiv.org/), by

* [Abhi Nellore](http://nellore.github.io)
* [Jean-Philippe Fortin](http://jfortinbiostats.com/)
* [José Alquicira-Hernández](https://github.com/joseah)
* [Leonardo Collado-Torres](http://www.biostat.jhsph.edu/~lcollado/)
* Siruo Wang
* Robert A. Phillips III
* Nishika Karbhari
* [Kasper D. Hansen](http://www.hansenlab.org/)
* [Andrew E. Jaffe](http://www.aejaffe.com/)
* [Ben Langmead](http://www.langmead-lab.org/)
* [Jeffrey T. Leek](http://jtleek.com/)
