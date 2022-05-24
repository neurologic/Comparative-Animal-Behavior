# Phylogeny

> {sub-ref}`today` | {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read


A phylogeny is a hypothesis.
Animal behaviorists use phylogenies to investigate the development of behavior across generations (evolutionary timescales).


## Sequences

[GenBank](https://www.ncbi.nlm.nih.gov/pubmed/23193287) is the NIH genetic sequence database, an annotated collection of all publicly available DNA sequences. The [nucleotide search](https://www.ncbi.nlm.nih.gov/nucleotide/) lets you search for species names and genes. If you use this resource, you can refer to the [FAQ](https://www.ncbi.nlm.nih.gov/books/NBK44863/) to get you started. 

***Q: What is the relationship between DNA and nucleotides?*** 

Below are two sequences downloaded from GenBank. "FASTA" is a common file format used to store sequence data. The files are very simple; they contain a *header* followed by the sequence. Click on the "FASTA" file headers to see the full sequence. 

<details>
	<summary>HQ377551.1 Chelonia mydas isolate Satang_4 16S ribosomal RNA gene, partial sequence; mitochondrial</summary>
GGCCGCGGTATCCTAACCGTGCAAAGGTAGCGTAATCACTTGTCTTTTAAATAAAGACTAGAATGAATGG
CCAAACGAGGTTCTACCTGTCTCTTACAAACAATCAGTGAAATTGATCTCCCCGTGCAAAAGCGGGGATA
ACACTATAAGACGAGAAGACCCTGTGGAACTTTAAATACAGATCAACTATCATACCCACTCACTCTAAGG
ACCTATAACTAATTAGTACTTGACCTATATTTTTGGTTGGGGCGACCTCGGAGTAAAACAAAACCTCCGA
AAAAAGAATACACTTCTTAACCTAGACCCACAATTCAAAGTGCCAACGGCAAAATGATCCAATATATTTG
ATCAACGAACCAAGCTACCCCAGGGATAACAGCGCAATCCCATCCTAGAGTTCCTATCGACGATGGGGTT
TACGACCTCGATGTTGGATCAGGACATCCTGATGGTGCAACCGCTATCAAGGGTTCGTTTGTTCAACGAT
TAACAGTCCTACGTGATCTG
</details>

<details>
	<summary>FJ039971.1 Eretmochelys imbricata isolate EI_Atlantic 16S ribosomal RNA gene, partial sequence; mitochondrial</summary>
GCCTCTAGCAACAACAAGTATTAGAGGTAATGCCTGCCCAGTGACACTGTTAAACGGCCGCGGTATCCTA
ACCGTGCAAAGGTAGCGTAATCACTTGTCTTTTAAATAAAGACTAGAATGAATGGCCAAACGAGGTTCCA
CCTGTCTCTTACAAACAATCAGTGAAATTGGTCTCCCCGTGCAAAAGCGAGGATAGCACTATAAGACGAG
AAGACCCTGTGGAACTTTAAATATAAATCAACTATTTAACTTACCACTCTAAAGACTTATAATTTACTAG
TTCTGATCCATATTTTTGGTTGGGGTGACCTCGGAGAAAAACAAAACCTCCGAAAAAAGAACATATCTTC
TTAACCTAGACCCACAACTCAAAGTGCCAACGGAAAAATGATCCAATATATTTGATCAACGAACCAAGCT
ACCCCAGGGATAACAGCGCAATCCCATCTTAGAGTCCATATCGACGATGGGGTTTACGACCTCGATGTTG
GATCAGGACATCCTGATGGTGCAACCGCTATCAAGGGTTCGTTTGTTCAACGATTAACAGTCCCACGTGA
T
</details>  

***Q: What information is contained in the header of the FASTA file?***

***Q: What gene specifically was sequenced for these two species?***  

The introduction of Yang et al (2014)[^Yang2014] gives great overview of mitochondrial DNA (mtDNA). 
[^Yang2014]: Yang, L., Tan, Z., Wang, D. et al. [Species identification through mitochondrial rRNA genetic analysis](https://doi.org/10.1038/srep04089). Sci Rep 4, 4089 (2014). 

> With few exceptions, the cells of all eukaryotic species contain mitochondria. The mitochondrial genome comprises a double-stranded DNA molecule of approximately 16 kb in length and accounts for 1% to 2% of the total DNA in mammalian cells. The mitochondrial genome encodes the following 13 essential oxidative phosphorylation subunit proteins/polypeptides: seven subunits of Complex I (ND1-6 and ND4L), one subunit of Complex III (Cytb), three subunits of Complex IV (COI-III) and two subunits of Complex V (ATPase 6 and 8). It also encodes two rRNAs (12S rRNA and 16S rRNA) and 22 tRNAs that are required for mitochondrial protein synthesis [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). Mitochondria possess their own organelle-specific DNA replication, transcription and translation systems [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). 

> Typical animal mtDNA has a high mutation rate and an exceptional organizational economy, with rare non-coding segments. The accelerated evolutionary rate of animal mtDNA implies that significant amounts of sequence variation could be observed in closely related species—a useful feature for species identification procedures. 

If significant sequence variation between closely related species is useful for species identification, then it is also useful for creating a phylogeny.

***Q: Based on this information, what do you think you need to do to create a phylogeny?*** 


## Alignment

The online webtool [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/) was developed to align genomic sequences across species. The output of the alignment procedure looks like the following:

:::
Hawksbill        AACTAT-TTAACTTACC-ACTCTAAAGACTTATAATTTACTAGTTC-TGATCCATATTTT
Loggerhead       AACTAT-TATATTTACC-ACCCTAAAGACTTATAATTAACTAGTTC-TGATCCATATTTT
Olive            AACTAT-CACACTTACT-ACCCTAAAGACTTATAACTTACTAGTTC-TGATCCATATTTT
Kemp’s           AACTAT-TACACTTACT-ACCCTAAAGACTTATAACTTACTAGTTC-TGATCCATATTTT
Leatherback      AACTACACATCCACACCTAATCTAAGGACTTATAACCAACTAG-ACTTGATCCATATTTT
Flatback         AACTAT-CATACTCACCCACCCCAAGGACCTATAACTAACTAATACTTGACCTATATTTT
Green            AACTAT-CATACCCACTCACTCTAAGGACCTATAACTAATTAGTACTTGACCTATATTTT
                 *****         **  *  * ** *** *****   * **   * *** * *******
:::


***Q: What do the stars represent?*** 

***Q: Compute the "relatedness" between Hawksbill and Loggerhead turtles***

***Q: Compute the "relatedness" between Hawksbill and Green turtles***


## From Relatedness to Trees

In a phylogenetic tree, the tips of branches represent *extant* (versus *extinct*) species. The tree is *rooted* with the *last common ancestor* (LCA) of all extant species on the tree. Each branch point from the root is a point of evolutionary *divergence*. 

:::{figure-md} sample-tree
:class: figure

<img src="/data/phylogeny/Sample-Tree.png" alt="fishy" class="bg-primary mb-1" width="400px">

An example phylogenetic tree.
:::

***Q: How many extant species are there in the tree (and what are their labels)?***

***Q: How many points of divergence are there?***

***Q: Use this tree as a phylogeny for the three turtle species for which you calcualted relatedness (Hawksbill, Loggerhead, and Green). Which letter (A, B, or C) would correspond to each turtle species?***


***Q: Why is a phylogeny a hypothesis? What information could you gather that might change the tree that you constructed?***

Based on the MUSCLE alignment of the 5 turtle species shown, we can use a computer algorithm to generate a phylogeny. In this example, I used [BioPython](https://biopython.org/) to calculate relatedness and estimate a tree. 


:::{figure-md} sample-tree
:class: figure

<img src="/data/turtles/turtle-tree.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence.
:::


[Open Tree (Bathyergidae)](https://tree.opentreeoflife.org/opentree/opentree13.4@mrcaott45520ott692678/Bathyergidae--Petromuridae)

[Python phylogenetics example](https://taylor-lindsay.github.io/phylogenetics/)

Character mapping
