# Phylogeny

<hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr>

:::{index} phylogeny
:::

Animal behaviorists use **phylogenies** to investigate the development of behavior across generations (evolutionary timescales).
Critically, a **phylogeny** is a hypothesis. Phylogenies can be tested and falsified, and can change given new evidence or analytic techniques.
Phylogenies can be based on any animal trait. Commonly, in studying animal behavior, you will encounter phylogenies based on genetics.

## Genetic Sequences

[GenBank](https://www.ncbi.nlm.nih.gov/pubmed/23193287) is the NIH genetic sequence database, an annotated collection of all publicly available DNA sequences. The [nucleotide search](https://www.ncbi.nlm.nih.gov/nucleotide/) lets you search for species names and genes. If you want to use this resource directly, you can refer to the [FAQ](https://www.ncbi.nlm.nih.gov/books/NBK44863/) to get you started. In this document, I will provide you with some example sequences from the GenBank.

***Q: What is the relationship between DNA and nucleotides?*** 

<a id='fasta-files'></a>
Below are the contents of two sequence files downloaded from GenBank. "FASTA" is a common file format used to store sequence data. The files are very simple; they contain a *header* followed by the sequence. Click on the "FASTA" file headers to see the full sequence from the file. 

:::{dropdown} HQ377551.1 Chelonia mydas isolate Satang_4 16S ribosomal RNA gene, partial sequence; mitochondrial
GGCCGCGGTATCCTAACCGTGCAAAGGTAGCGTAATCACTTGTCTTTTAAATAAAGACTAGAATGAATGG
CCAAACGAGGTTCTACCTGTCTCTTACAAACAATCAGTGAAATTGATCTCCCCGTGCAAAAGCGGGGATA
ACACTATAAGACGAGAAGACCCTGTGGAACTTTAAATACAGATCAACTATCATACCCACTCACTCTAAGG
ACCTATAACTAATTAGTACTTGACCTATATTTTTGGTTGGGGCGACCTCGGAGTAAAACAAAACCTCCGA
AAAAAGAATACACTTCTTAACCTAGACCCACAATTCAAAGTGCCAACGGCAAAATGATCCAATATATTTG
ATCAACGAACCAAGCTACCCCAGGGATAACAGCGCAATCCCATCCTAGAGTTCCTATCGACGATGGGGTT
TACGACCTCGATGTTGGATCAGGACATCCTGATGGTGCAACCGCTATCAAGGGTTCGTTTGTTCAACGAT
TAACAGTCCTACGTGATCTG
:::

:::{dropdown} FJ039971.1 Eretmochelys imbricata isolate EI_Atlantic 16S ribosomal RNA gene, partial sequence; mitochondrial
GCCTCTAGCAACAACAAGTATTAGAGGTAATGCCTGCCCAGTGACACTGTTAAACGGCCGCGGTATCCTA
ACCGTGCAAAGGTAGCGTAATCACTTGTCTTTTAAATAAAGACTAGAATGAATGGCCAAACGAGGTTCCA
CCTGTCTCTTACAAACAATCAGTGAAATTGGTCTCCCCGTGCAAAAGCGAGGATAGCACTATAAGACGAG
AAGACCCTGTGGAACTTTAAATATAAATCAACTATTTAACTTACCACTCTAAAGACTTATAATTTACTAG
TTCTGATCCATATTTTTGGTTGGGGTGACCTCGGAGAAAAACAAAACCTCCGAAAAAAGAACATATCTTC
TTAACCTAGACCCACAACTCAAAGTGCCAACGGAAAAATGATCCAATATATTTGATCAACGAACCAAGCT
ACCCCAGGGATAACAGCGCAATCCCATCTTAGAGTCCATATCGACGATGGGGTTTACGACCTCGATGTTG
GATCAGGACATCCTGATGGTGCAACCGCTATCAAGGGTTCGTTTGTTCAACGATTAACAGTCCCACGTGA
T
:::

***Q: What information is contained in the header of the FASTA file?***

***Q: What gene specifically was sequenced for these two species?***  

The introduction of Yang et al (2014)[^Yang2014] gives succinct overview of mitochondrial DNA (mtDNA). 
[^Yang2014]: Yang, L., Tan, Z., Wang, D. et al. [Species identification through mitochondrial rRNA genetic analysis](https://doi.org/10.1038/srep04089). Sci Rep 4, 4089 (2014). 

:::{epigraph} 
With few exceptions, the cells of all eukaryotic species contain mitochondria. The mitochondrial genome comprises a double-stranded DNA molecule of approximately 16 kb in length and accounts for 1% to 2% of the total DNA in mammalian cells. The mitochondrial genome encodes the following 13 essential oxidative phosphorylation subunit proteins/polypeptides: seven subunits of Complex I (ND1-6 and ND4L), one subunit of Complex III (Cytb), three subunits of Complex IV (COI-III) and two subunits of Complex V (ATPase 6 and 8). It also encodes two rRNAs (12S rRNA and 16S rRNA) and 22 tRNAs that are required for mitochondrial protein synthesis [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). Mitochondria possess their own organelle-specific DNA replication, transcription and translation systems [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). 

Typical animal mtDNA has a high mutation rate and an exceptional organizational economy, with rare non-coding segments. The accelerated evolutionary rate of animal mtDNA implies that significant amounts of sequence variation could be observed in closely related species—a useful feature for species identification procedures. 
:::

If significant sequence variation between closely related species is useful for species identification, then it is also useful for creating a phylogeny.

***Q: Based on all of the information provided so far, what do you think you need to do to create a phylogeny?*** 

***Q: Given the sequences shown from [the two FASTA files](#fasta-files), why would it be difficult to determine genetic differences between species?*** 


## Sequence Alignment

The online webtool [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/) was developed to align genomic sequences across species. The output of the alignment procedure looks like the following:

<a id='alignment'></a>
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

***Q: Compute a metric of "relatedness" between Hawksbill and Loggerhead turtles***

***Q: Use the same method ot compute the "relatedness" between Hawksbill and Green turtles***


## From Relatedness to Trees

In a phylogenetic tree, the tips of branches represent *extant* (versus *extinct*) species. The tree is *rooted* with the *last common ancestor* (LCA) of all extant species on the tree. Each branch point from the root is a point of evolutionary *divergence*. 

:::{figure-md} sample-tree
:class: figure

<img src="/data/phylogeny/Sample-Tree.png" alt="fishy" class="bg-primary mb-1" width="400px">

An example phylogenetic tree.
:::

***Q: How many extant species are there in the tree (and what are their labels)?***

***Q: How many points of divergence are there?***

***Q: If you used this tree as a phylogeny for the three turtle species for which you calculated relatedness (Hawksbill, Loggerhead, and Green), wshich letter (A, B, or C) would correspond to each turtle species?***


***Q: Why is a phylogeny a hypothesis? What information could you gather that might change the tree that you constructed?***

Based on the [MUSCLE alignment of the 7 turtle species](#alignment), we can use a computer algorithm to calculate relatedness and generate a drawing of the most likely phylogeny. In this example (Fig. 2), I used [BioPython](https://biopython.org/) to calculate relatedness and estimate a tree. 


:::{figure-md} turtle-tree
:class: figure

<img src="/data/turtles/turtle-tree.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of 7 turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence.
:::


## From Trees to Behavioral Evolutionary History

If you search the [Animal Diversity Web](https://animaldiversity.org/) (for example), you will find that, of the 7 turtle species you have just examined, all but one are classified as *solitary*. The green turtle (*Chelonia mydas*) is classified as "colonial"[^colonial].

[^colonial]: "Used loosely to describe any group of organisms living together or in close proximity to each other - for example nesting shorebirds that live in large colonies. More specifically refers to a group of organisms in which members act as specialized subunits (a continuous, modular society) - as in clonal organisms." - [ADW](https://animaldiversity.org/accounts/Chelonia_mydas/#behavior)"

From a phylogenetic perspective, why is the green turtle colonial? If the LCA at the root of divergence for the green turtle was colonial, then it is an evolutionarily inherited behavior. If the LCA at the root of divergence for the green turtle was solitary, then it is an evolutionarily derived behavior. To understand whether a behavior is evolutionarilty derived or inherited at each node of a phylogenetic tree, we must determine the ancestral trait at each node. 

One basic way to do this is to use the principle of parsimony after counting evolutionary changes under each alternate LCA hypothesis.

***Q: Which requires more events/steps? Evolutionary change or evolutionary stasis?***

***Q: If the LCA of the turtles in Figure 2 was solitary, what is the least number of evolutionary changes that would need to occur to result in the correct behavioral traits of all 7 extant species?***

***Q: If the LCA of the turtles in Figure 2 was colonial, what is the least number of evolutionary changes that would need to occur to result in the correct behavioral traits of all 7 extant species?***

***Q: Which alternate hypothesis would require more evolutionary changes?***

***Q: All else being equal, which hypothesis results in a less likely series of events: "LCA was solitary" or "LCA was colonial"?***

***Q: If the method of parsimony is used to reject the less likely hypothesis, then what would be the result of your analysis? In other words, how would you interpret your results in terms of determining the behavioral trait exhibited by the LCA of these 7 turtles?***

***Q: If there are species of turtles missing from this phylogeny, how could that change the results of your ancestral state reconstruction analysis?***

***Q: If no one had yet characterized the behavior of some extant species within your phylogeny, how would that add uncertainty to your analysis and interpretation of the results?***

Many published phylogenetic trees exist that you can explore without needing to analyze any genetics. For example, [here is the entry on OpenTree that includes all 7 turtle species you have just examined](https://tree.opentreeoflife.org/opentree/opentree13.4@ott66469/Cheloniidae). This tree is rooted at *Cheloniidae* (the sea turtles), which is a *monophyletic group*. In this web interface, branches of the tree are sometimes collapsed for visual clarity. Clicking on each branch line in the tree reveals how many extant species derive from that branch. Clicking on each node in the tree roots the visualization at that node (often expanding/collapsing sets of branches as the view changes). Practice navigating around the tree. 

***Q: How many other species of turtles should have been included in Figure 2 to generate a complete phylogeny of sea turtles?***



There are, broadly, several categories of social behavior: solitary, social, and eusocial

:::{glossary}
solitary
	Individuals live and behave alone (except during mating usually)

social
	Individuals group together for some activities, but each maintain reproductive independence. 
	
eusocial
	Some individuals among the social group give up their own reproductive opportunities to help others reproduce. 
:::

Check out the [phylogeny of Bathyergidae on OpenTree](https://tree.opentreeoflife.org/opentree/opentree13.4@mrcaott45520ott692678/Bathyergidae--Petromuridae). 

Bathyergidae is comprised of 6 Genera: *Heterocephalus, Bathyergus, Fukomys, Cryptomys, Georychus,* and *Heliophobius*. There are only two species among the Bathyergidae family that are eusocial: *Fukomys demarensis* and *Heterocephalus glaber*. 

***Q: How many extant species are within the Bathyergidae family?***

If all extent species from the heliophobius genus are not eusocial, then it is more likely that the LCA of all heliophobius was not eusocial. The same logic applies to Bathyergus, Cryptomys, and Georychus. Likewise, the LCA of all Fukomys was likely not eusocial. To construct the behavior of the LCA for all Bathyergidae, We can consider a 'reduced' tree of all genera within this family. 

:::{figure-md} rootnonsocial
:class: figure

<img src="/data/phylogeny/Bathyergidae-genus-tree-eusocial-color-rootnonsocial.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of Bathyergidae genera with character mapping of eusocial (green) and not eusocial (orange) character mapping of LCA for each genera. Ancestral state reconstruction shown for the hypothesis that the LCA of Bathyergidae was *not* eusocial.
:::

:::{figure-md} rootsocial
:class: figure

<img src="/data/phylogeny/Bathyergidae-genus-tree-eusocial-color-rootsocial.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of Bathyergidae genera with character mapping of eusocial (green) and not eusocial (orange) character mapping of LCA for each genera. Ancestral state reconstruction shown for the hypothesis that the LCA of Bathyergidae was eusocial.
:::
 
***Q: Why is the Heterocephalus genus LCA eusocial?***

***Q: Which hypothesis would you reject based on parsimony?***

*Outgroups* can help resolve ambiguity in ancestral state reconstruction. 

:::{figure-md} with-outgroup
:class: figure

<img src="/data/phylogeny/Bathyergidae-genus-tree-with-outgroup.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of Bathyergidae genera and the *outgroups* *Petromuridae* and *Thryonomyidae*.
:::

***Q: Both Petromuridae and Thryonomyidae were* not *eusocial, what would you conclude about the behavior of the LCA for Bathyergidae?***

***Q: What was the most likely behavior of the LCA for all Bathyergidae species - based on counts of evolutionary change under each alternate hypothesis and a model of parsimony?***

***Q: Why is it important to include outgroups in an ancestral state reconstruction?***

## Conclusions

***Q: Include any questions or comments that you have about phylogeny***


Data for the turtle phylogeny was collected by Lindsay Taylor as part of their [example jupyter notebooks implementation of BioPython](https://taylor-lindsay.github.io/phylogenetics/)
