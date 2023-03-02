# Phylogeny and Evolution


:::{admonition} Deadline
Due by 11pm on Friday March 10.
:::

:::{admonition} Honor Code
This exam is open note/book/web, but must be done independently. Do not consult any other people (regardless of whether they are in or out of this course) or artificial intelligence (AI) in answering the questions. Handing in responses to the assignment for grading serves as your signature of the honor code.
:::

Answer all questions either electronically or by hand. Label each of your answers with the corresponding question number. Scan or convert your document to a good quality PDF. Upload to gradescope by the deadline -- make sure to tag all appropriate page(s) in your PDF for each question. 

**Please don’t hesitate to ask for clarifation on the wording of questions and/or expectations**. Key expectations are highlighted with font style. For any multiple choice question that asks for an explanation of your reasoning: provide a correct answer selection as well as your reasoning for selecting that answer - the reasoning should logically (and unabiguously) explain for your answer selection. Not all multiple choice questions require for reasoning.



## Section 1: Evolutionary history of feeding behavior

:::{image} /images/phylogeny-feeding-exam-example.png
:width: 800
:align: center
:::

**Figure 1:**  

***Q (2 points)*** Select the most complete sentence (among the choices) to add to the caption for Figure 1.   
**a)** *Phylogeny of finches with the character mapping of feeding behavior overlaid*   
**b)** *Phylogeny of 11 extant species of finches*  
**c)** *Phylogeny of finches with the character mapping and ancestral state reconstruction of feeding behavior overlaid*  

***Q (2 points)*** Select a correct sentence to add to the caption for Figure 1.   
**a)** *The nodes (labeled a, b, c, and d) mark potential points of phenotype divergence.*    
**b)** *The nodes (labeled a, b, c, and d) mark potential points of phenotype convergence.*  
**c)** *The nodes (labeled a, b, c, and d) mark the time of evolution of new phenotypes.*  

***Q (2 points)*** Which node (*a, b, c, or d*) represents the last common ancestor for the entire set of extant species shown?

***Q (5 points)*** Why is it least likely (*by parsimony*) that the last common ancestor of all extant species shown was a *folivore*?  
(***Answer this question in 1-3 concise sentences by drawing a conclusion in terms of the alternate hypotheses and quantitative results of your analysis under each hypothesis.***)  

***Q (4 points)*** Which node (*a, b, c,* or *d*) represents the last common ancestor for all Ground finches and Tree finches? What was the most likely behavioral trait of that LCA (*in your analysis, consider all information available in the Figure*)?  

***Q (2 points)*** Which node (*a, b, c,* or *d*) represents the last common ancestor for only the extant ground finch species?

***Q (2 points)*** Consider the scenario in which two species that exhibit the same behavioral phenotype and are incorrectly separated in a phylogenetic tree such that, by parsimony, their most recent common ancestor exhibited a different behavioral trait. In this situation, you would misinterpret their common phenotype as an example of [*CONVERGENCE* / *DIVERGENCE* / *SHARED ANCESTRY*] rather than correctly identifying it as an example of [*CONVERGENCE* / *DIVERGENCE* / *SHARED ANCESTRY*].  
(***Choose the appropriate term from each bracketed list to complete the sentence.***)

## Section 2: Evolutionary models for feeding behavior in offspring

:::{admonition} Phenotypes and factors affecting evolutionary fitness of feeding behavior

Let's consider two behavioral phenotypes associated with feeding behavior:   
1. *BEGGER* = begs for food by making loud vocalizations.  
2. *SILENT* = do nothing while waiting for food from the parent  

Parents will feed their offspring no matter what, but loud vocalizations grab their attention and cause them to preferentially feed *begging* offspring over *silent* offspring if they are present.   
We will assume that the amount of food a parent is able to gather is limited, and we will call this value **$f$** (for simplicity, *assume that the amount of food that the parent is able to gather does not depend on the behavior of its offspring*). Begging offspring get all of the food, *but* they also expend a lot of energy to produce vocalizations (a factor that we will call **$e$**) *AND* the vocalizations make them more noticable to predators and increase the likelihood that they will get attacked (a factor that we will call **$p$**). 

:::

### Optimality Theory

***Q (3 points)*** Given this setup, the most reasonable optimality theory model for the total net fitness of individual offspring (**$F$**) would be formulated as:  
(***Choose the one correct option from below and briefly explain your reasoning.***)  
**a**) $f = - e - p$  
**b**) $F = f - e - p$  
**c**) $F = -f + e + p$  
**d**) $F = f + e + p$  

***Q (2 points)*** According to the optimality theory model you chose, the average fitness of the *silent* phenotype could depend on:  
(***Choose the one correct option from below***)  
**a)** whether conspecifics were *beggers* or *silent*.  
**b)** the number of predators in the environment (and therefore the risk of predation).  
**c)** whether $e > p$ or $p < e$ for the *begging* phenotype.   

***Q (3 points)*** Given the optimality theory model you chose (and its assumptions explained in the setup), under which of the following conditions would you predict that the *silent* phenotype would be stable at evolutionary equilibrium?    
(***Choose the one correct option from below and explain your reasoning.***)  
**a**) When $f$ (the food gathered by the parent) is greater for *silent* offspring than for *begging* offspring (assuming all other factors are the same for both phenotypes)  
**b**) When $e$ is greater for *begging* offspring than for *silent* offspring (assuming all other factors are the same for both phenotypes)  
**c**) When $p$ is greater for *silent* offspring than for *begging* offspring (assuming all other factors are the same for both phenotypes)  


### Game Theory 

:::{image} /images/game-theory-chick-feeding-exam-example.png
:width: 300
:align: center
:::

**Figure 2:** *Game theory model of *begging* versus *silent* feeding behavior phenotypes in offspring (following the convension that: columns = phenotypes of conspecifics; rows = net fitness of each phenotype being assessed). The factors in the model are the same as in the optimality theory model: $f$ (the food gathered by the parent), $e$ (energy to produce vocalizations), $p$ (likelihood of being noticed/attacked by predators).* 

***Q (4 points)*** According to the game theory model, beggers would have a greater net fitness in a population of [*BEGGING* / *SILENT*] offspring than in a population of [*BEGGING* / *SILENT*] offspring.  
(***Choose the correct words to complete the sentence above.  
Then, select one option from below that provides the appropriate caveat based on the game theory.***)   
**a)** However, this scenario is not possible because the *silent* phenotype is not the evolutionarily stable phenotype.   
**b)** However, this scenario is not possible because the *silent* phenotype has a lower net fitness than the *begging* phenotype in a population of *begging* offspring.  
**c)** However, this scenario is not possible because *begging* is the only evolutionarily stable phenotype.  
**d)** However, this scenario would not be possible if the *silent* phenotype had a lower net fitness than the *begging* phenotype in a population of *begging* offspring.  

***Q (3 points)*** State the mathematical conditions for which *begging* would be the evolutionarily stable phenotype.  
(***Refer to the game theory model shown. Show your work to set up the necessary inequality(ies), and simplify so that all of the 'fitness increasing' factors are on one side and all of the 'fitness decreasing' factors are on the other.***)

***Q (3 points)*** State the mathematical conditions for which *silent* would be the evolutionarily stable phenotype.  (***Refer to the given game theory model. Show your work to set up the necessary inequality(ies), and simplify so that all of the 'fitness increasing' factors are on one side and all of the 'fitness decreasing' factors are on the other.***)

***Q (2 points)*** A population comprised of all begging offspring would be evolutionarily stable when:  
(***Refer to the conditions you determined in Q\____ to choose the one correct option that completes the sentence.***)   
**a)** the likelihood of predation is less than the food obtained from the parent.   
**b)** the likelihood of predation is less than the food that the parent is able to gather.  
**c)** $e$ is actually a negative number.  
**d)** the combined fitness deficit caused by the increased likelihood of predation and energy needed to vocalize are less than half of the food that the parent is able to gather.  


### Summary 

***Q (2 points)*** Which is the more appropriate model (optimality theory or game theory) for understanding the feeding behavior of offspring, and why?   
(***Choose the one correct option***)  
**a)** Game Theory, because the fitness of the feeding behavior phenotypes likely do *NOT* depend on the strategies of conspecifics.  
**b)** Game Theory, because the fitness of the feeding behavior phenotypes likely *DO* depend on the strategies of conspecifics.  
**c)** Optimality Theory, because the fitness of the feeding behavior phenotypes likely *DO* depend on the strategies of conspecifics.  
**d)** Game theory, because a mixed population of *begging* and *silent* phenotypes is evolutionarily stable, and game theory is the only type of model that can predict a mixed population.  

***Q (2 points)*** An assumption of both of optimality theory and game theory models is that:   
(***Choose the one correct option***)  
**a)** the models can predict the evolutionarily stable behavior of a species.   
**b)** behavioral phenotypes change across phylogeny because of evolution.  
**c)** behavioral phenotypes change across phylogeny because of natural selection.
**d)** the fitness of individuals depends on the phenotype of conspecifics.
**e)** natural selection reduces phenotypic variance among a species.  

<!-- ## Section 3 Ancestral state reconstruction correction

A student who studied cannabalism among snakes for their capstone provided the following figure and explanation as part of their phylogenetic analysis of the behavior:

:::{image} ../images/Phylogeny_Snake-Cannibalism.png
:width: 400
:::

"*In this case, the ancestral trait is cannibalistic behavior because the species “Sistrurus catenatus" has a direct lineage to the common ancestor. This species does show cannibal-like behavior, thus the ancestral trait is cannibalism.*"  

***Q (3 points)*** Why was this an incorrect analysis?
 -->
<!-- 
---

## You can do it better

Improve these two excerpts from editorials on animal behavior. Make at least two major improvements to each excerpt. Highlight your changes and briefly explain the reason for the change using footnote-style annotation. 

One
:::{epigraph}
A phylogeny is a study of the relationships among a group of organisms. Animals that evolved from a common ancestor evolve in different ways. They also develop different traits at different times. Every species can be connected to one common ancestor that they all evolved from. In this case, phylogeny is used on rattlesnakes. (Figure 1) The rattlesnakes were investigated for showing the trait of cannibalistic behavior or not showing the trait. Out of many species, only 6 show cannibalistic behavior. For the species that do show the trait, they seem to come up in very distant relationships. Very few of the species that are close in evolution share the trait. Also, based on just the phylogeny the ancestral trait can be predicted. An ancestral trait is a trait that the very first ancestor, that the species evolved from, shows. In this case, the ancestral trait is cannibalistic behavior because the species “Sistrurus catenatus" has a direct lineage to the common ancestor. This species does show cannibal-like behavior, thus the ancestral trait is cannibalism.
:::

:::{figure-md} Phylogeny-example_snake-cannibal
<img src="/images/Phylogeny_Snake-Cannibalism.png" alt="fishy" class="bg-primary mb-1" width="400px">

The character mapping and ancestral state reconstruction accompanying the text. 
:::

Two 

:::{epigraph}
Infanticide has a high benefit and a low cost. The high benefit is because eating a snake's offspring can bring a lot of nutrients into the snake's diet. Some snakes eat their young because they need to compensate for their lost energy when producing offspring. The cost is low because it is easy for the snake to eat their young, there is very little risk to the parent snake itself since the offspring has no means of defending itself. Since the benefit outweighs the cost this is a viable option and could explain why rattlesnakes partake in cannibalism. The main benefit of infanticide is not losing the energy that went into reproduction.
:::

- Can you think of any alternative hypotheses or factors? -->
<!-- ---

Code breaking of escape by tentacled snake (read a Ken Catania paper?)

What is the FAP of the fish? what is the sign stimulus? What is the code-breaking behavior? How would the escape behavior of fish likely start to differ in environments where tentacled snakes live? Why might the escape behavior persist 'as-is' even in environments where tentacled snakes live (ie. what other selection pressures are there on the escape behavior)?


 -->

