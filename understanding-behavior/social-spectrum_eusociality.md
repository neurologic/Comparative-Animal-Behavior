# Eusociality

[Responses template if you need it](https://docs.google.com/document/d/1PV03kG71qufTCPp2DHmdE5MDzO0zHsohVdp4dv91XEI/edit?usp=sharing)

:::{image} /images/eusocial-montage.png
:width: 700
:align: center
:::

:::{admonition} Defining Features
- Reproductive altruism
- Cooperative parental care
- Multi-generational
- Living in groups
:::


## Ultimate Explanations

**Reproductive altruism** is the key feature making eusociality difficult to understand from an evolutionary perspective.

:::{margin} Snowdrift Model
| |Altruist |Selfish|
|:--: |:--:|:--:
|**Altruist**| b - c/2 | b - c |
|**Selfish**| b | 0 |
:::

Some evolutionary models can explain cooperative altruism when the cost to the social donor is low enough (for example, the snowdrift model). However, the loss of reproduction seems effectively like an infinitely high cost. If evolutionary fitness is defined by how much you pass your genes to the next generation, not producing any offspring would result in zero fitness, no matter what factors you were able to increase your individual ("lifetime") fitness.

There are lots of alternate models that aim to make sense of eusociality and reproductive altruism.

### Group Level selection

"*The process known as group selection was once accepted unthinkingly, then was widely discredited*." - Edward Wilson and David Wilson[^for-good-of-group-oped]. The underlying question-"Can biological traits evolve for the good of the group?"-is a heavily debated concept. 

Wilson and Wilson are trying to pave the way for reconsidering group selection as a predictive force in understanding the evolution of behavior.

[^for-good-of-group-oped]: [Evolution "for the Good of the Group" BY EDWARD O. WILSON, DAVID SLOAN WILSON. American Scientist (2008)](https://www.americanscientist.org/article/evolution-for-the-good-of-the-group)



To think clearly about group selection, it is important to compare the survival and reproduction of individuals in the right way. Selection between individuals within groups favors cheating behaviors, even at the expense of the group as a whole (as seen in the game theory models). Selection between groups within the total population favors behaviors that increase the relative fitness of the whole group—although these behaviors, too, can have negative effects at a still-larger scale.

:::{image} /images/group-selection.png
:width: 600
:align: center
:::

The balance between levels of selection can tilt in either direction. Wilson and Wilson make the point that there is no single formula; answers must be worked out on a case-by-case basis[^for-good-of-group-oped]. 

:::{margin} Quantitative Genetics
“Quantitative Genetics” methods model changes in allele frequency from one generation to the next. In a general form, consider the **change in allele frequency = covariance(fitness, trait) / mean population fitness**. These models aim to understand how traits evolve due to natural selection.[^quant-vs-game]
:::

[^quant-vs-game]: [Joel W McGlothlin, Erol Akçay, Edmund D Brodie, III, Allen J Moore, Jeremy Van Cleve, A Synthesis of Game Theory and Quantitative Genetic Models of Social Evolution, Journal of Heredity, Volume 113, Issue 1, January 2022, Pages 109–119](https://doi.org/10.1093/jhered/esab064)

### Kin Selection

In the form of a ***quantitative genetics model*** (see margin), the frequency of an altruistic allele will increase if:

$$ 
r * b > c
$$

where **c** is the factor(s) that decreases the fitness of the donor for an altruistic act, **b** is the factor(s) that increases the fitness of the recipient for an altruistic act, and **r** is the relatedness between the donor and recipient of the altruistic act. The first derivation of this model (based on "*Price's equation*) was done by Hamilton[^hamilton-derivation-explanation]. 

Basically, this "*Hamilton's rule*" states that, if you help someone that shares a lot of your genotype (is very related to you), then your genotype will effectively be passed on *through* them if you help them reproduce.  

[^hamilton-derivation-explanation]: [Jonathan Birch (2017) Hamilton’s Rule as an Organizing Framework](https://doi.org/10.1093/oso/9780198733058.003.0002)

While it has been cited a lot and pushed heavily in classic textbooks, the examples providing evidence for this model are debated, and some debate its function as a predictive model at all[^Nowack].

[^Nowak]: [The general form of Hamilton’s rule makes no predictions and cannot be tested empirically](https://doi.org/10.1073/pnas.1701805114)

### Reproductive Potential

The ‘canonical Hamilton’s rule’ lacks demographic structure. Akcay and Van Cleve (2015)[^A-C-2015] explain a different model that re-evaluates the importance of reproductive potential on the impact of relatedness in ***heterogeneous populations***. From this model, we can infer a role for *polyphenisms* versus *polymorphisms* in the inheritance of altruism and selfishness. 

[^A-C-2015]: [Akcay and Van Cleve (2016) There is no fitness by fitness, and the lineage is its bearer](https://doi.org/10.1098%2Frstb.2015.0085)

:::{figure} /images/honeybee-castes.png
:width: 500

**Example of a heterogeneous pupulation**. Members of the three honeybee castes are morphologically and behaviorally distinct. Only the queen reproduces
:::

Population heterogeneity does not have to be so dramatic. In lots of populations, there are simply ***dominant*** and ***submissive*** individuals. Often, the submissive individuals are "altruistic" to the dominant individuals but receive no reciprocation. 

For example, male wild turkeys pair up during the mating season to compete for females. The ***lek*** is the mating battleground where males strut to attract females. To strut, a male holds their tail upright while fanning out their feathers, drops their wings so their primary feathers are touching the ground, makes their feathers erect to appear as large as possible, and pulls their neck inward. The role of the submissive male of each pair is to fend off other competing male pairs. If the pair succeeds in attracting a female, ***only the dominant turkey actually mates***.

<iframe width="560" height="315" src="https://www.youtube.com/embed/xDGCEvdj5GU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

So why doesn't the submissive phenotype get eliminated by natural selection? How can a male in a lek who never succeeds in mating with a female nevertheless “benefit” by their participation? Both of these questions assume potentially incorrect thinking about the proximate and ultimate mechanisms of behavior -- instead, the submissive male might not need to ever "benefit", and selfish and altruist phenotypes may be linked rather than mutually exclusive. 

In Akcay and Van Cleve's model, fitness is averaged across the social environments and demographic states in which members of a lineage find themselves. In other words, fitness belongs to the gene lineage, not to the individual.

The frequency of an altruistic gene will increase if[^repro-pot-derivation]:

$$
(1 - \sigma) * [-c_d + r * b_d] > s * \sigma * [-c_s + r * b_s]
$$

where $\sigma$ is the fraction of submissives in the population, $c_d$ is the cost to a dominant individual for helping a subordinate (and vice-versa for $c_s$), $b_d$ is the benefit to the dominant when it is helped by a subordinate (and vice-versa for $b_s$), and $r$ is the relatedness between dominant and subordinate individuals.

This model seems to require that altruism and selfishness are polyphenisms. 

[^repro-pot-derivation]: The derivation of this equation comes from [Taylor and Frank (1996) How to make a kin selection model](https://doi.org/10.1006/jtbi.1996.0075) and is explained in this format in [Akcay and Van Cleve (2016) There is no fitness by fitness, and the lineage is its bearer](https://doi.org/10.1098%2Frstb.2015.0085). 

---
> ⏳ 3 min 

***Q1 : If dominants never help subordinates, what is the value of $c_d$ and $b_s$?***

***Q2 : Assume the population has an equal number of dominants and subordinates so that $\sigma = 1 - \sigma$ (ie. turkey lekking pairs). Simplify the model equation given this assumption and the assumption that dominants never help subordinates.***

⏸️ PAUSE here for class-wide discussion

---

### Ecological Factors

***Ecological origins*** mechanisms for (eu)sociality predict different worker sex ratios than ***relatedness*** mechanisms.[^Ross-2013] 

[^Ross-2013]: [Ross, L., Gardner, A., Hardy, N., & West, S. A. (2013). Ecology, not the genetics of sex determination, determines who helps in eusocial populations. Current biology : CB, 23(23), 2383–2387.](https://doi.org/10.1016/j.cub.2013.10.013)

:::{figure} /images/eusociality-ecology-hypoth.png
:width: 500

Predictions of relatedness and ecological hypotheses on the sex ratio of the worker caste.[^Ross-2013]
:::

::::{margin} haplodiploidy: males develop from unfertilized eggs and are haploid, and females develop from fertilized eggs and are diploid
:::{image} ../images/Haplodiploid_Sex_Determination_in_Honey_Bees.svg.png
:::
::::

The ***relatedness hypothesis*** suggests that, in haplodiploid species, a higher relatedness between sisters (75% f:f vs 25% f:m or 50% m:m) favors female workers. In contrast, in diploid species, there is no relatedness asymmetry among siblings, and both sexes are equally favored to be workers. This hypothesis focuses on the possible importance of variation in the relatedness \(r\) term in Hamilton’s rule.

The ***ecology hypothesis*** suggests that the sex of the *worker* caste depends upon the ecological (economic) benefit of cooperation and eusociality. For example, either the cooperative rearing of brood when it is likely that either the offspring or the parent will die before parental care is completed (life insurance) or colony defense when the living environment requires social defense (fortress defense). 
- If workers rear brood, then we would expect the workers to be drawn from the sex or sexes that provided parental care in the ancestral solitary species, which is usually females. 
- If workers defend the colony, and neither sex is preadapted to be a soldier, then we would expect the workers to be drawn from both sexes. 

This ecological origins hypothesis focuses on the possible importance of variation in the benefit (b) and cost \(c\) terms in Hamilton’s rule. It is not mutually exclusive to the theory of kin selection more generally. 

Ross et al (2013)[^Ross-2013] performed a meta-analysis to test these hypotheses (Figure 133 and 134). 

:::{figure} /images/eusociality-ecology-phylogeny.png
:width: 500

Open circles and filled squares represent diploid versus haplodiploid taxa, respectively, while the number within each square/circle shows the number of independent origins of eusociality (according to Wilson’s definition of eusociality) within each clade. The color of the icon represents the sex ratio of workers—half blue, half pink for unbiased and pink for female only.[^Ross-2013]
:::

:::{figure} /images/eusocial-ecological-results.png
:width: 400

The probability of having female only helpers, as opposed to an unbiased mixture of males and females (where 0 represents an unbiased helper sex ratio), for haploidiploid and diploid taxa in the different ecological scenarios.[^Ross-2013] 
:::

---
> ⏳ 3 min 

***Q3: Which of the following would you infer given these results, and why?***  
***A) the evolution of eusociality was influenced more by ecological selective pressures on altruism than by relatedness among individuals of a population***  
***B) the evolution of eusociality was influenced more by relatedness among individuals of a population than by ecological selective pressures on altruism***

⏸️ PAUSE here for class-wide discussion

---

#### Origins of cooperative parental care

*Ammophila* (digger wasps) are non-social. However, their behavior provides clues to a potential evolutionary mechanism for cooperative parental care[^Field-Brace-2004]. All ammophila lay single eggs in nests stocked with food provisions. 

[^Field-Brace-2004]: [Field, J., Brace, S. Pre-social benefits of extended parental care. Nature 428, 650–652 (2004).](https://doi.org/10.1038/nature02427)

:::{figure} /images/ammophila-nest.png
:width: 300

Diagram of an ammophila nest.
:::

<iframe src="https://drive.google.com/file/d/1MxIAFYikTgWR5zLtthHtTcDn1rzpKrOE/preview" width="640" height="480" allow="autoplay"></iframe>

However, some species ***mass provision*** each nest, while other species ***progressively provision*** their nests. 

- Mass provisioners work on one nest at a time, fully provisioning each in one shot and sealing the nest. 
- Progressive provisioners simultaneously work on 2-5 nests at a time, initiating all of the nests on the same day and then coming back each day to re-provision. 

Progressive provisioning enables the opportunity to intervene or terminate investment early if offspring show signs of failing. If an offspring does not look like it will make it, the wasp can save otherwise wasted energy investment in it. However, progressively provisioned offspring are more at risk of parasitism because the nest keeps getting reopened to reprovision and is unattended while the parent is foraging for provisions. More offspring would survive if the parental wasp had help guarding the nest from parasites while it was tending to other nests. 

### Other Selective Pressures?

#### Case Study: Mole rats

:::{figure} /images/mole-rat-phylogeny.png
:width: 600

Simplified phylogeny for the African mole-rats indicating main clades/genera. Numbers in parentheses indicate current estimates of species numbers in each genus. From [Faulkes and Bennett (2021)](https://doi.org/10.1007/978-3-030-65943-1_1)
:::

Note that the eusocial naked mole-rat at the base of the tree and the eusocial Damaraland mole-rat at the top of the tree are separated by a number of common ancestors that vary in degrees of sociality. From the eusocial naked mole-rat at the base of the tree, sociality was lost, and then evolved again. Eusociality has evolved independently twice within the same family. 

::::{margin} Arid versus Mesic environments
:::{image} /images/mole-rat-eusocial-ecological-factors.png
:::
::::


By comparing the character mapping of social behavior among this phylogeny with the mapping of ecological factors, we find that eusociality is associated with **arid** versus **mesic** habitats. 

:::{figure} /images/mole-rat-phylogeographical-pattern.png
:width: 600

Phylogeographical patterns of genetic divergence and speciation in African mole-rats (Family: Bathyergidae) in the context of rift valley formation in Africa (indicated by brown lines). African mole-rats are distributed in a range of habitats across sub-Saharan Africa, and display a range of social and reproductive strategies. From [Faulkes et al (2004)](https://doi.org/10.1046/j.1365-294x.2004.02099.x)
:::


<!-- #### Case Study: Vespid wasps

:::{figure} /images/vespid-social-phylogeny.png
:width: 300

Character mapping of eusociality (gray) and solitary (white) behavior among *Vespidae*. Two alternative phylogenetic hypotheses are presented. A) the conventional hypothesis based on morphological and behavioral characters. B) An alternative based on molecular data.[^Hines-2006]
:::

***Q4: Under each phylogenetic hypothesis, was the LCA of Vespidae solitary or eusocial?***

***Q5: Under each phylogenetic hypothesis, how many times did eusociality independently evolve?***

***Q6: Why would the alternate phylogenetic hypothesis based on molecular data be more useful for understanding the selective pressures favoring eusociality in Vespidae?***  

[^Hines-2006]: [Multigene phylogeny reveals eusociality evolved twice in vespid wasps](https://www.pnas.org/doi/10.1073/pnas.0610140104) -->

## Proximate Mechanisms

### Neural

> ⏳ 5 min 

***Q4: What behaviors and/or might be modified to support eusocial versus solitary or group lifestyles? And how, at a proximate level, could these modifications be achieved?***


⏸️ PAUSE here for class-wide discussion

---

***Social neuroscience*** is a rapidly expanding and integrative field of study. Research that focuses on the neurobiology of eusociality per se is lacking. 

What we do know so far is that social processes cannot be localized to one brain region-they are highly distributed systems.

There is more known about the neurobiology of related behaviors, for example **pair bonding** in monogamous species. Research has found that, in ***voles***, oxytocin and vasopressin hormonal systems play a large role. Pair bonding is not a component of eusociality per se, but at least in mammals, we find that ***cooperative breeding (a precondition for eusociality) is restricted to monogamous species***. Comparative studies of oxytocin and vasopressin receptor distribution among African mole-rats have revealed both similarities and differences with reference to voles.  

The only other neural substrate that has been investigated in African mole-rats in a detailed comparative context is the corticotrophin-releasing factor (CRF) family of hormone peptides and receptors[^Coen-2021]. This study found clear species differences in the anatomical pattern of receptor/ligand binding between naked mole-rats and Cape mole-rats (a solitary species) which are suggested to reflect differences in affiliative behavior.

[^Coen-2021]: [Coen, C. W., Bennett, N. C., Holmes, M. M., & Faulkes, C. G. (2021). Neuropeptidergic and Neuroendocrine Systems Underlying Eusociality and the Concomitant Social Regulation of Reproduction in Naked Mole-Rats: A Comparative Approach. Advances in experimental medicine and biology, 1319, 59–103.](https://doi.org/10.1007/978-3-030-65943-1_3)


### Genetic and Development

In the following examples, environmental signals are used to modulate behavioral phenotype.
 
- [Suryanarayanan, S., Hermanson, J. C., & Jeanne, R. L. (2011). A mechanical signal biases caste development in a social wasp. Current biology : CB, 21(3), 231–235](https://doi.org/10.1016/j.cub.2011.01.003)
- [The effect of Royal Jelly and DNMT3 on the development of workers versus queens](../levels-of-analysis/development.md)

---
> ⏳ 5 min 

***Q5: What do these studies imply about the inheritance of altruist and selfish genes/alleles? Are altruist and selfish likely different alleles of the same gene(s) or controlled by different (sets of) genes?*** 

⏸️ PAUSE here for class-wide discussion

---

## Additional Resources

- [army ants podcast](https://www.listennotes.com/podcasts/discovery/tooth-and-claw-army-ant-pDlqVjaXSz8/)
	<iframe src="https://www.listennotes.com/podcasts/discovery/tooth-and-claw-army-ant-pDlqVjaXSz8/embed/" height="180px" width="100%" style="width: 1px; min-width: 100%;" frameborder="0" scrolling="no" loading="lazy"></iframe>
- [Faulkes, C., & Bennett, N. (2016). Damaraland and naked mole-rats: Convergence of social evolution. In W. Koenig & J. Dickinson (Eds.), Cooperative Breeding in Vertebrates: Studies of Ecology, Evolution, and Behavior (pp. 338-352). Cambridge: Cambridge University Press.](http://dx.doi.org/10.1017/CBO9781107338357.020) (or access [via share link](https://drive.google.com/file/d/1r5ghtynPVhl3jEaLCCwpuwS55AkdelNr/view?usp=sharing)
- [Jonathan Birch (2017) Hamilton’s Rule as an Organizing Framework](https://doi.org/10.1093/oso/9780198733058.003.0002)
- [McGlothlin et al (2022) A Synthesis of Game Theory and Quantitative Genetic Models of Social Evolution](https://doi.org/10.1093/jhered/esab064)
- [Field, J., Brace, S. Pre-social benefits of extended parental care. Nature 428, 650–652 (2004).](https://doi.org/10.1038/nature02427)
- [Faulkes, C.G., Bennett, N.C. (2021). Social Evolution in African Mole-Rats – A Comparative Overview. In: Buffenstein, R., Park, T.J., Holmes, M.M. (eds) The Extraordinary Biology of the Naked Mole-Rat. Advances in Experimental Medicine and Biology, vol 1319.](https://doi.org/10.1007/978-3-030-65943-1_1)
- [Faulkes, C. G., Verheyen, E., Verheyen, W., Jarvis, J. U., & Bennett, N. C. (2004). Phylogeographical patterns of genetic divergence and speciation in African mole-rats (Family: Bathyergidae). Molecular ecology, 13(3), 613–629.](https://doi.org/10.1046/j.1365-294x.2004.02099.x)
- [Opachaloemphan, C., Yan, H., Leibholz, A., Desplan, C., & Reinberg, D. (2018). Recent Advances in Behavioral (Epi)Genetics in Eusocial Insects. Annual review of genetics, 52, 489–510.](https://doi.org/10.1146/annurev-genet-120116-024456)