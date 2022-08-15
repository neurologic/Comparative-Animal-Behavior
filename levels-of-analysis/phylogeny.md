# Phylogeny

<hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr>

:::{index} phylogeny
:::

:::{admonition} Why?
Animal behaviorists use **phylogenies** to investigate the development of behavior across generations (evolutionary timescales).
Critically, a **phylogeny** is a hypothesis. Phylogenies can be tested and falsified, and can change given new evidence or analytic techniques.
Phylogenies can be based on any animal trait. Commonly, in studying animal behavior, you will encounter phylogenies based on genetics.
:::

## Genetic Sequences

[GenBank](https://www.ncbi.nlm.nih.gov/pubmed/23193287) is the NIH genetic sequence database, an annotated collection of all publicly available DNA sequences. The [nucleotide search](https://www.ncbi.nlm.nih.gov/nucleotide/) lets you search for species names and genes. If you want to use this resource directly, you can refer to the [FAQ](https://www.ncbi.nlm.nih.gov/books/NBK44863/) to get you started. In this document, I provide you with example sequences from the GenBank.

---
> ⏳ 5 min 

***Q: What is the relationship between DNA and genes?***

***Q: What is the relationship between DNA and nucleotides?*** 

***Q: What is the relationship between DNA and RNA?*** 

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 5 min 

<a id='fasta-files'></a>
Below are two *FASTA* files downloaded from GenBank. "FASTA" is a common file format used to store sequence data. The files are very simple; they contain a *header* followed by the sequence. Click on the file headers to see its contents. 

:::{dropdown} HQ377551.1 *Chelonia mydas* isolate Satang_4 16S ribosomal RNA gene, partial sequence; mitochondrial; length 510
GGCCGCGGTATCCTAACCGTGCAAAGGTAGCGTAATCACTTGTCTTTTAAATAAAGACTAGAATGAATGG  
CCAAACGAGGTTCTACCTGTCTCTTACAAACAATCAGTGAAATTGATCTCCCCGTGCAAAAGCGGGGATA 
ACACTATAAGACGAGAAGACCCTGTGGAACTTTAAATACAGATCAACTATCATACCCACTCACTCTAAGG  
ACCTATAACTAATTAGTACTTGACCTATATTTTTGGTTGGGGCGACCTCGGAGTAAAACAAAACCTCCGA  
AAAAAGAATACACTTCTTAACCTAGACCCACAATTCAAAGTGCCAACGGCAAAATGATCCAATATATTTG  
ATCAACGAACCAAGCTACCCCAGGGATAACAGCGCAATCCCATCCTAGAGTTCCTATCGACGATGGGGTT  
TACGACCTCGATGTTGGATCAGGACATCCTGATGGTGCAACCGCTATCAAGGGTTCGTTTGTTCAACGAT  
TAACAGTCCTACGTGATCTG
:::

:::{dropdown} FJ039971.1 *Eretmochelys imbricata* isolate EI_Atlantic 16S ribosomal RNA gene, partial sequence; mitochondrial; length 560
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

***Q: How much information contained in the header of the FASTA file can you decipher?***

***Q: What gene specifically was sequenced for these two species?***  


:::{epigraph} 
With few exceptions, the cells of all eukaryotic species contain mitochondria. The mitochondrial genome comprises a double-stranded DNA molecule that accounts for 1% to 2% of the total DNA in mammalian cells. The mitochondrial genome encodes 13 essential oxidative phosphorylation subunit proteins/polypeptides. It also encodes two rRNAs (12S rRNA and 16S rRNA) and 22 tRNAs that are required for mitochondrial protein synthesis [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). Mitochondria possess their own organelle-specific DNA replication, transcription and translation systems [13,14,15,16](https://www.nature.com/articles/srep04089#Bib1). 

Typical animal mtDNA has a high mutation rate and an exceptional organizational economy, with rare non-coding segments. The accelerated evolutionary rate of animal mtDNA implies that significant amounts of sequence variation could be observed in closely related species—a useful feature for species identification procedures. 

-- Yang et al (2014)[^Yang2014]
:::

[^Yang2014]: Yang, L., Tan, Z., Wang, D. et al. [Species identification through mitochondrial rRNA genetic analysis](https://doi.org/10.1038/srep04089). Sci Rep 4, 4089 (2014). 

***Q: Given the sequences shown from [the two FASTA files](#fasta-files), why would it be difficult to determine differences in the genetic sequence between species?*** 


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10 min 


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

***Q: Compute a metric of "relatedness" between Hawksbill and Loggerhead turtles based on sequence (dis)similarity.***

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

***Q: If you used this tree as a phylogeny for the three turtle species for which you calculated relatedness (Hawksbill, Loggerhead, and Green), which letter (A, B, or C) would correspond to each turtle species?***


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 5 min 

***Q: Based on all of the information provided so far, how would you define 'phylogeny'?*** 

***Q: Why is mitochondrial DNA particularly useful for assembling a phylogeny?***

***Q: Why is a phylogeny a hypothesis? What information could you gather that might change the tree that you constructed?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10 min 

Based on the [MUSCLE alignment of the 7 turtle species](#alignment), we can use a computer algorithm to calculate relatedness and generate a drawing of the most likely phylogeny. 

:::{figure-md} turtles_cladogram_black
:class: figure

<img src="/data/turtles/turtles_cladogram_black.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of 7 turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence using [BioPython](https://biopython.org/).
:::


## From Trees to Behavioral Evolutionary History

If you search the [Animal Diversity Web](https://animaldiversity.org/) (for example), you will find that, of the 7 turtle species you have just examined, all but one are classified as *solitary*. The green turtle (*Chelonia mydas*) is classified as "colonial"[^colonial].

[^colonial]: "Used loosely to describe any group of organisms living together or in close proximity to each other - for example nesting shorebirds that live in large colonies. More specifically refers to a group of organisms in which members act as specialized subunits (a continuous, modular society) - as in clonal organisms." - [ADW](https://animaldiversity.org/accounts/Chelonia_mydas/#behavior)"

:::{figure-md} turtles_cladogram_character-map
:class: figure

<img src="/data/turtles/turtles_cladogram_character-map.png" alt="fishy" class="bg-primary mb-1" width="600px">

A character mapping of social behavior on the phylogeny of 7 turtle species. Green = colonial. Orange = solitary.
:::

***Q: Based on the information given, define 'character mapping'.***

From a phylogenetic perspective, we can understand why the green turtle colonial. There are two alternative explanations: that colonialism is a phylogenetically *inherited* behavior or that colonialism is a phylogenetically *derived* behavior. 

Examine the following two *ancestral state reconstruction* hypotheses and their graphical representation. 

**Hypothesis \#1**: The LCA of this turtle phylogeny was colonial. A consequence of this hypothesis would be that colonialism is an evolutionarily inherited behavior in green turtles. 

:::{figure-md} turtles_cladogram_LCA1
:class: figure

<img src="/data/turtles/turtles_cladogram_LCA1.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of 7 turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence using BioPython.
:::

***Hypothesis \#2***: The LCA of this turtle phylogeny was solitary. A consequence of this hypothesis would be that colonialism is an evolutionarily derived behavior in green turtles. 

:::{figure-md} turtles_cladogram_LCA0
:class: figure

<img src="/data/turtles/turtles_cladogram_LCA0.png" alt="fishy" class="bg-primary mb-1" width="600px">

A phylogenetic tree of 7 turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence using BioPython.
:::

***Q: Under which ancestral state reconstruction hypothesis (1 or 2) would colonialism be an inherited trait in green turtles?***

***Q: What is the difference between an 'ancestral state reconstruction' and a 'character mapping'?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10 min 

We can provide evidence for/against each of these alternative hypotheses about the LCA behavioral trait by using an *argument of parsimony*. 

***Q: Which requires more events/steps? Evolutionary change or evolutionary stasis?***

***Q: If the LCA of the turtles in Figure ______ was solitary (hypothesis \#2), what is the least number of evolutionary changes that would need to occur to result in the correct behavioral traits of all 7 extant species?***

***Q: If the LCA of the turtles in Figure ______ was colonial (hypothesis \#1), what is the least number of evolutionary changes that would need to occur to result in the correct behavioral traits of all 7 extant species?***

***Q: Which alternate hypothesis would require more evolutionary changes?***

***Q: All else being equal, which hypothesis results in a less likely series of events: "LCA was solitary" or "LCA was colonial"?***

***Q: If the method of parsimony is used to reject the less likely hypothesis, then what would be the result of your analysis? In other words, how would you interpret your results in terms of determining the behavioral trait exhibited by the LCA of these 7 turtles?***


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10 min 


***Q: What is the minimum subset of this phylogenetic tree that you would need to provide evidence that colonialism is a derived trait in green turtles?***

***Q: If there are species of turtles missing from this phylogeny, how could that change the results of your ancestral state reconstruction analysis?***

***Q: If no one had yet characterized the behavior of some extant species within your phylogeny, how would that add uncertainty to your analysis and interpretation of the results?***

Many published phylogenetic trees exist that you can explore without needing to analyze any genetics. For example, [here is the entry on OpenTree that includes all 7 turtle species you have just examined](https://tree.opentreeoflife.org/opentree/opentree13.4@ott66469/Cheloniidae). This tree is rooted at *Cheloniidae* (the sea turtles), which is a *monophyletic group*. In this web interface, branches of the tree are sometimes collapsed for visual clarity. Clicking on each branch line in the tree reveals how many extant species derive from that branch. Clicking on each node in the tree roots the visualization at that node (often expanding/collapsing sets of branches as the view changes). Practice navigating around the tree. 

***Q: How many other species of turtles should have been included in Figure 2 to generate a complete phylogeny of sea turtles?***


⏹️ STOP here for today


## Additional Resources

[Common Descent Podcast, Episode 10: The Tree of Life](https://www.youtube.com/watch?v=ULzJgG5IBAo&list=PLfdiT8Klm_YPa0lNVa9ygwAjy_1Lpz9_S&index=11)
Data for the turtle phylogeny was collected by Lindsay Taylor as part of their [example jupyter notebooks implementation of BioPython](https://taylor-lindsay.github.io/phylogenetics/)
