# Phylogeny
<!-- 
<hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr> -->

[Day 1](phylogeny_day1); [Responses template for use on computer if desired](https://docs.google.com/document/d/1Zny7rFlzbYkPHoAMDLy6aPTXH-bod1ODxdhiLQz9AIg/edit?usp=sharing)  
[Day 2](phylogeny_day2); [Responses template for use on computer if desired]

:::{index} phylogeny
:::


:::{admonition} Why?
Animal behaviorists use **phylogenies** to investigate the development of behavior across generations (evolutionary timescales).
Critically, a **phylogeny** is a hypothesis. Phylogenies can be tested and falsified, and can change given new evidence or analytic techniques.
Phylogenies can be based on any animal trait. Commonly, in studying animal behavior, you will encounter phylogenies based on *genetic sequence data*.
:::

Today and tomorrow, you will be working on understanding what phylogenies are and phylogenetic analyses that are used to study animal behavior. All of the information that you need for today is contained on this page. However, this page also links you to tools that you can use in the future to study the phylogenetic basis of behavior. 

(phylogeny_day1)=
## Genetic Sequences

All animals have genes (generally, sequences of *nucleutides*, usually abbreviated *A*, *T*, *G*, and *C*). [GenBank](https://www.ncbi.nlm.nih.gov/pubmed/23193287) is the NIH genetic sequence database, an annotated collection of all publicly available DNA sequences. The [nucleotide search](https://www.ncbi.nlm.nih.gov/nucleotide/) lets you search for species names and genes. Here, I have provided you with example sequences from the GenBank to refer to.[^genbank]

[^genbank]: If you want to use this resource directly, you can refer to the [FAQ](https://www.ncbi.nlm.nih.gov/books/NBK44863/) to get you started. 

---
> ⏳ 5 min 

<a id='fasta-files'></a>
Below are two *FASTA* files downloaded from GenBank. "FASTA" is a common file format used to store genetic sequence data. The files are very simple; they contain a *header* (with *metadata* about the file) followed by a sequence of nucleotide codes. Click on the file headers to see its contents. 

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

***Q1: Given the information in the header file, what gene was sequenced?*** 

***Q2: How long is the sequenced gene for each species?*** 


⏸️ PAUSE here for class-wide discussion

---

From [Yang et al (2014)](https://doi.org/10.1038/srep04089): "With few exceptions, the cells of all eukaryotic species contain mitochondria. The mitochondrial genome comprises a double-stranded DNA molecule that accounts for 1% to 2% of the total DNA in mammalian cells. Typical animal mitochondrial DNA (***mtDNA***) has a high mutation rate. The accelerated evolutionary rate of animal mtDNA implies that significant amounts of sequence variation could be observed in closely related species—a useful feature for species identification procedures."[^yang-2014]

[^yang-2014]: Yang, L., Tan, Z., Wang, D. et al. [Species identification through mitochondrial rRNA genetic analysis](https://doi.org/10.1038/srep04089). Sci Rep 4, 4089 (2014).  

## From Relatedness to Trees

In a tree representation of a **phylogeny** (Figure 9), the tips of branches represent *extant* (versus *extinct*) species. The tree is *rooted* with the *last common ancestor* (LCA) of all extant species on the tree (the evolutionarily oldest species of the tree). Each branch point from the root is a point of evolutionary *divergence*. We talk about species being closer to each other on a phylogenetic tree as being more *related* (having a higher *relatedness*).

---
> ⏳ 10 min 

:::{figure-md} sample-tree
:class: figure

<img src="/data/phylogeny/Sample-Tree.png" alt="fishy" class="bg-primary mb-1" width="400px">

An example phylogenetic tree.
:::

The following table reports the number of mtDNA sequence differences between species in the example phylogeny (Figure 9).

|  | B | C |
| :---: | :---: | :---: |
| **A** | 5 | 23 |
| **B** | - | 23 |

***Q3: How many extant species are there in the tree?***

***Q4: How many points of divergence are there?***

***Q5: If there are fewer branch points between two species, do they have more or fewer differences in their mtDNA sequence?***

***Q6: Given the sequences shown in [the two FASTA files](#fasta-files) that you already examined, why would it be difficult to determine differences in the genetic sequence between species?*** 


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10 min 


## Sequence Alignment

The online webtool [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/) was developed to align genomic sequences across species. The following is the output of the MUSCLE alignment procedure for a genetic sequence (16S ribosomal RNA partial gene sequence) from 7 species of turtles:

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


***Q7: What does the star mean for a column of letters (molecules in the gene sequence)?*** 

***Q8: Compute a metric of genetic similarity ("relatedness") between Hawksbill and Loggerhead turtles based on sequence (dis)similarity.***

***Q9: Use the same method to compute the relatedness between Hawksbill and Green turtles.***

***Q10: If you used the example phylogeny (Figure 9) for these three turtle species (Hawksbill, Loggerhead, and Green), which letter (A, B, or C) would most likely correspond to each turtle species?***


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 5 min 

***Q11: Based on all of the information provided so far, how would you define 'phylogeny'?*** 

***Q12: Remember that a phylogeny is a hypothesis. What would an 'alternative hypothesis' be for the example phylogeny (Figure 9)?***

⏸️ PAUSE here for class-wide discussion

---

Readily available computer algorithms can calculate relatedness from *aligned* genetic sequence data and generate a drawing of the most likely phylogeny. 

:::{figure} /images/turtles_cladogram_black.png
:width: 600

A phylogenetic tree of 7 turtle species. Relatedness and branch lengths were calculated from the MUSCLE alignement data of the 16S ribosomal RNA partial gene sequence using [BioPython](https://biopython.org/).
:::

Many published phylogenetic trees exist that you can explore without needing to obtain or analyze any genetics yourself. For example, [here is the entry on OpenTree that includes all 7 turtle species you have just examined](https://tree.opentreeoflife.org/opentree/opentree13.4@ott66469/Cheloniidae). This tree is rooted at *Cheloniidae* (the sea turtles), which is a *monophyletic group*. In this web interface, branches of the tree are sometimes collapsed for visual clarity. Clicking on each branch line in the tree reveals how many extant species derive from that branch. Clicking on each node in the tree roots the visualization at that node (often expanding/collapsing sets of branches as the view changes). Practice navigating around the tree. 

Clicking on the ```i``` icon next to a node brings up a menu with a ```Search EOL for 'node name'``` link. ***EOL*** is the "Encyclopedia of Life". This non-profit is a great resource for biodiversity information. 


⏹️ STOP here for today

---

(phylogeny_day2)=
## From Trees to Behavioral Evolutionary History

If you search the [Animal Diversity Web](https://animaldiversity.org/) (for example), you will find that, of the 7 turtle species you have just examined, all but one are classified as *solitary*. The green turtle (*Chelonia mydas*) is classified as *colonial*[^colonial]. 

From a phylogenetic perspective, why is the green turtle colonial? Either colonialism is an *inherited* behavior or colonialism is a *derived* behavior. In order to determine whether colonialism is derived or inherited, we need to test all alternative hypotheses for the ancestral state reconstruction. 

[^colonial]: "Used loosely to describe any group of organisms living together or in close proximity to each other - for example nesting shorebirds that live in large colonies. More specifically refers to a group of organisms in which members act as specialized subunits (a continuous, modular society) - as in clonal organisms." - [ADW](https://animaldiversity.org/accounts/Chelonia_mydas/#behavior)"

---
> ⏳ 10 min 

:::{figure} /images/turtles-charmap-lca.png
:width: 800

Graphical representations of character mapping and ancestral state reconstruction. **A)** Character mapping of social behavior on the turtle phylogeny. Green = colonial. Orange = solitary. **B)** Ancestral state reconstruction under Hypothesis \#1 on the turtle phylogeny. **C)** Ancestral state reconstruction under Hypothesis \#2 on the turtle phylogeny. To construct the turtle phylogeny, relatedness and branch lengths were calculated from the *MUSCLE* alignement data of the 16S ribosomal RNA partial gene sequence using *BioPython*.
:::

***Q1: Based on the information given, what do you think 'character mapping' is?***

***Q2: Under Hypothesis \#1, the LCA of this turtle phylogeny exhibited ______________ behavior (fill in the blank).*** 

***Q3: Under Hypothesis \#2, the LCA of this turtle phylogeny exhibited ______________ behavior (fill in the blank).*** 

***Q4: How is a character mapping different than an ancestral state reconstruction?***

***Q5: Under which ancestral state reconstruction hypothesis (1 or 2) would colonialism be an inherited (versus derived) trait in green turtles?***


⏸️ PAUSE here for class-wide discussion

---
> ⏳ 15 min 

One common way to assess alternative hypotheses for the LCA behavioral trait is to use an *argument of* ***parsimony***. Answer the following questions to understand the logic of making an argument about LCA behavior based on ***parsimony***.

***Q6: If the LCA of the turtles in Figure 11 was solitary, what is the least number of total evolutionary changes that would need to occur (across the tree) to result in the correct behavioral traits of all 7 extant species?***

***Q7: If the LCA of the turtles in Figure 11 was colonial, what is the least number of total evolutionary changes that would need to occur to result in the correct behavioral traits of all 7 extant species?***

***Q8: Which alternative hypothesis would require more evolutionary changes?***

By an argument of parsimony, we would conclude that it is less likely that the LCA was colonial. 

***Q9: From that conclusion, which would you infer is more likely: evolutionary change or evolutionary stasis?***

***Q10: Create your definition for the "argument of parsimony".***

***Q11: If no one had yet characterized the behavior of Flatback and Leatherback turtles, would it change the results of your analysis? How would you handle this unknown data in your analysis?***

⏸️ PAUSE here for class-wide discussion

---

### Case Study: Vocal Learning

:::{figure} /images/phylogeny-vocal-learning-comparison.png
:width: 900

Phylogeny of *Neoaves* (By clicking on the image you can zoom in).  
**A)** From the *Animal Behavior, 9th edition* textbook by Rubenstein and Alcock (2009). Phylogeny data generated using DNA-DNA hybridization[^dna-hybridization] and published by Eliot A. Brenowitz in *Evolution of the vocal control system in the avian brain*[^brenowitz-1991]. Character mapping of vocal learnering highlighted in green, blue, and red.  
**B)** From Suh et al (2011)[^suh-2011]. Phylogeny data generated using Mesozoic retroposons[^retroposons] and analysis utilizing ***maximum parsimony***. New taxa *Eufalconimorphae* (falcons+parrots+passerines) and *Psittacopasserae* (parrots+passerines) are highlighted.
:::

[^brenowitz-1991]: [Eliot A. Brenowitz (1991) *Evolution of the vocal control system in the avian brain*. Seminars in Neuroscience; 3(5).](https://doi.org/10.1016/1044-5765%2891%2990030-R)

[^dna-hybridization]: (from [wiki](https://en.wikipedia.org/wiki/DNA%E2%80%93DNA_hybridization)) The DNA of one organism is labelled, then mixed with the unlabelled DNA to be compared against. The mixture is incubated to allow DNA strands to dissociate and then cooled to form renewed hybrid double-stranded DNA. Hybridized sequences with a high degree of similarity will bind more firmly, and require more energy to separate them: i.e. they separate when heated at a higher temperature than dissimilar sequences, a process known as "DNA melting". To assess the melting profile of the hybridized DNA, the double-stranded DNA is bound to a column and the mixture is heated in small steps. At each step, the column is washed; sequences that melt become single-stranded and wash off the column. The temperatures at which labelled DNA comes off the column reflects the amount of similarity between sequences (and the self-hybridization sample serves as a control). These results are combined to determine the degree of genetic similarity between organisms. One method was introduced for hybridizing large numbers of DNA samples against large numbers of DNA probes on a single membrane. These samples would have to be separated in their own lanes inside the membranes and then the membrane would have to be rotated to a different angle where it would result in simultaneous hybridization with many different DNA probes.


[^suh-2011]: [Suh, A., Paus, M., Kiefmann, M. et al. Mesozoic retroposons reveal parrots as the closest living relatives of passerine birds. Nat Commun 2, 443 (2011).](https://doi.org/10.1038/ncomms1448)

[^retroposons]: (from [Suh et al 2011](https://doi.org/10.1038/ncomms1448)) Retroposons, jumping genetic elements that copy via RNA intermediates and insert nearly randomly anywhere in the genome (although some biases of insertion and retention have been proposed15), provide (by inheritance) virtually homoplasy-free evidence of relatedness that is detectable for more than 100 million years. Because parallel insertions or exact excisions are highly unlikely, presence/absence patterns of retroposons at orthologous genomic loci are powerful, clear-cut phylogenetic markers capable of resolving long-standing uncertainties.

---
> ⏳ 15 min 

:::{figure} /images/phylogeny-vocal-learning-comparison-drawn.png
:width: 900

Character mapping of vocal learning behavior on the phylogeny of *Neoaves* from Brenowitz (1991)[^brenowitz-1991] in **A** and **B** and off of Suh et al (2011)[^suh-2011] in **C**.
:::

***Q12: Use the phylogeny in Figure 13A to analyze (using parsimony) the two alternative ancestral state reconstruction hypotheses for the LCA of all song learners (arrow).***   

***Q13: How would your analysis change using the same (but simplified) phylogeny in Figure 13B?*** 

***Q14: Use the phylogeny in Figure 13C to analyze (using parsimony) the two alternate ancestral state reconstruction hypotheses for the LCA of all song learners.***  

***Q15: How does your understanding of vocal learning behavior change based on the two phylogenetic hypotheses (Brenowitz versus Suh)?*** 


⏹️ STOP here for today

:::{admonition} Complete this section for homework and bring your responses to next class in a format that you can turn in (written on paper, printed, or emailed to me directly are all fine). They will be graded CR/U. 
:name: phylogeny-burrowing-assignment

1. Examine Figure 2 from [Weber and Hoekstra (2009). The evolution of burrowing behaviour in deer mice (genus Peromyscus)](https://doi.org/10.1016/j.anbehav.2008.10.031). Perform an ancestral state reconstruction for burrowing behavior among these species by examining alternate hypotheses for the LCA and analyzing the results using an argument of parsimony. Bring your analysis to class.[^Hu-Hoekstra-review]

[^Hu-Hoekstra-review]: Figure 1 from [Hu and Hoekstra (2017) Peromyscus burrowing: A model system for behavioral evolution. Journal of Cell and Developmental Biology, 61](https://doi.org/10.1016/j.semcdb.2016.08.001) shows a mapping of both burrowing behavior and habitat on the phylogeny of Peromyscus. You can also start prepping for the next section of the course by thinking about... What correlations do you notice? What do you wonder about the function of burrowing behavior and how that relates to its phylogenetic history?

2. Using the concepts and tools you learned today, research the phylogeny of a species/behavior you are interested in. What are the alternatives to the behavior? How much the the phylogeny do you need to examine interesting convergence and/or divergence for the behavior? Bring your analyis to class.
:::


## Additional Resources

- [Common Descent Podcast, Episode 10: The Tree of Life](https://www.youtube.com/watch?v=ULzJgG5IBAo&list=PLfdiT8Klm_YPa0lNVa9ygwAjy_1Lpz9_S&index=11)
- Data for the turtle phylogeny was collected by Lindsay Taylor as part of their [example jupyter notebooks implementation of BioPython](https://taylor-lindsay.github.io/phylogenetics/)

