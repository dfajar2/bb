bb
==

Bioinformatics utilities by Douglas Senalik

bb stands for black box

See also http://www.vcru.wisc.edu/simonlab/sdata/software/index.html

bb
--

The program bb is a program to list the other programs in the project with a short
one or two line summary of the program.

Type bb for a list of all programs, or bb followed by some text for a grep-like limit
to the list of programs returned.
Due to poor programming on my part, bb assumes that programs are
installed in /usr/local/bin or /usr/local/bb

bb.454contiginfo
----------------

This is a Perl program that will take an assembly of Roche 454 sequences generated by the
Roche newbler/gsAssembler, and displays all information for one or more specified contigs,
in particular, the connection and read flowthrough information.

For more details see http://www.vcru.wisc.edu/simonlab/sdata/software/index.html#contiginfo

bb.454contignet
---------------

This is a Perl program that will take an assembly of Roche 454 sequences generated by the
Roche newbler/gsAssembler, and use the connection information to link generated contigs
into a graphical map.

For more details see http://www.vcru.wisc.edu/simonlab/sdata/software/index.html#contignet

Reference. If you use this software, you may cite using this reference:

Massimo Iorizzo, Douglas Senalik, Marek Szklarczyk, Dariusz Grzebelus, David Spooner and Philipp Simon
De novo assembly of the carrot mitochondrial genome using next generation sequencing of whole genomic
DNA provides first evidence of DNA transfer into an angiosperm plastid genome
[BMC Plant Biology 2012, 12:61](http://www.biomedcentral.com/1471-2229/12/61)

Other citations:

1. Tongwu Zhang, Xiaowei Zhang, Songnian Hu and Jun Yu
An efficient procedure for plant organellar genome assembly, based on whole genome data
from the 454 GS FLX sequencing platform
[Plant Methods 2011, 7:38](http://www.plantmethods.com/content/7/1/38) doi:10.1186/1746-4811-7-38
[Additional file 1](http://www.plantmethods.com/content/supplementary/1746-4811-7-38-s1.doc)

2. Fajardo _et al._ Complete plastid genome sequence of _Vaccinium macrocarpon_: structure,
gene content, and rearrangements revealed by next generation sequencing
[Tree Genetics & Genomes April 2013, Volume 9, Issue 2, pp 489-498](http://link.springer.com/article/10.1007%2Fs11295-012-0573-9)

3. Chang S, Wang Y, Lu J, Gai J, Li J, et al. (2013)
The Mitochondrial Genome of Soybean Reveals Complex Genome Structures and Gene Evolution
at Intercellular and Phylogenetic Levels. [PLoS ONE 8(2): e56502.](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0056502)
doi:10.1371/journal.pone.0056502

4. Shearman _et al._ Assembly and analysis of a male sterile rubber tree mitochondrial
genome reveals DNA rearrangement events and a novel transcript
[BMC Plant Biology 2014, 14:45](http://www.biomedcentral.com/1471-2229/14/45)
doi:10.1186/1471-2229-14-45

bb.coverage
-----------

This program generates coverage plots from various types of input.
Fasta, fastq, sff, bam, or bed file input can be used.

bb.elsdlt
---------

This program collects and parses output from a Shimadzu ELSD-LT, which is
an Evaporative Light-scattering Detector, Low Temperature,
(original version circa 2002+) as collected from its RS232 serial port

bb.fastaconsensus
------------

This program takes an aligned multi-FASTA file as input, and generates
a consensus sequence based on the most abundant nucleotide.

bb.fastagrep
------------

Search and return sequences from FASTA or FASTQ files based on matches
to one or more queries to text in the header line. Also can do search
and replace on headers.

bb.fastareorder
---------------

This program will allow changing the order or orientation of multiple sequences
in FASTA format, or extraction of a subset of sequences. The resulting sequences
can optionally be concatenated into a single sequence.

For more details see http://www.vcru.wisc.edu/simonlab/sdata/software/index.html#fastareorder

This was cited by

Tongwu Zhang, Xiaowei Zhang, Songnian Hu and Jun Yu
An efficient procedure for plant organellar genome assembly, based on whole genome data
from the 454 GS FLX sequencing platform
[Plant Methods 2011, 7:38](http://www.plantmethods.com/content/7/1/38) doi:10.1186/1746-4811-7-38
[Additional file 1](http://www.plantmethods.com/content/supplementary/1746-4811-7-38-s1.doc)

bb.gapcoder
-----------

Implements gap coding of an aligned multi-fasta file as described in
BMC Bioinformatics 2003 4:6 "GapCoder automates the use of indel
characters in phylogenetic analysis"
http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-4-6
This program generates a tab-delimited matrix output format

bb.gffsort
---------------

Sort a gff3 file maintaining child features with the parent feature.
Sort alphabetically by sequence name, then numerically by start and
then by end coordinate.

bb.motif
--------

This program was used to generate a supplemental file for the publication:

Marina Iovene, Pablo F. Cavagnaro, Douglas Senalik, C. Robin Buell, Jiming Jiang and Philipp W. Simon
Comparative FISH mapping of Daucus species (Apiaceae family)

[Chromosome Research Volume 19, Number 4, 493-506](http://www.springerlink.com/content/y73j6m3133n16773/)
DOI: 10.1007/s10577-011-9202-y

For more details see http://www.vcru.wisc.edu/simonlab/sdata/software/index.html#motif

bb.orffinder
------------

This is a Perl program that will computationally detect open reading frames in DNA or RNA sequences in FASTA format.
This is computationally similar to the NCBI program at http://www.ncbi.nlm.nih.gov/gorf/orfig.cgi,
but allows command-line automation of the process, as well as a few additional features.

For more details see http://www.vcru.wisc.edu/simonlab/sdata/software/index.html#orffinder

bb.revcomp
----------

A very simple pipe to reverse complement a raw sequence stream
e.g. echo "ACTG" | bb.revcomp
outputs "CAGT"

bb.scaftigs
-----------

This program will return all portions of a final assembly consisting of
contiguous sequence, with sequences split at every occurrence of gaps of
unknown bases (Ns)

bb.tassel
---------

This program will preprocess paired-end Illumina reads from
GBS (Genotyping By Sequencing) experiments to make them
compatible with TASSEL. This involves copying the barcode
from the forward reads to the beginning of the reverse reads,
since TASSEL cannot otherwise identify the reverse reads which
do not have a barcode.

bb.timestamper
--------------

This program acts as a pipe, and will insert time stamps in the stream,
useful for monitoring long-running programs that do not themselves
output timestamps

bb.topoview
--------------

A wrapper around code originally from a script from
http://flybase.org/static_pages/docs/software/topoview.html
2009-2010 Victor Strelets, FlyBase.org

This program creates TopoView tracks for GBrowse from .wig or .bed files

To install prerequisites:
sudo apt-get install libdb-dev
sudo cpan BerkeleyDB
