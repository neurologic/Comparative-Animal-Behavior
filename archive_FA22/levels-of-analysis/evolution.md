# Evolution

[Day 1](evolution_day1); [Responses template for use on computer if desired](https://docs.google.com/document/d/1Tz0iU8VG9O7BDL44alGmGt5CVBvecdRQEe_dC-J_a2M/edit?usp=sharing)  
[Day 2](game-theory); [Responses template for use on computer if desired](https://docs.google.com/document/d/1Tz0iU8VG9O7BDL44alGmGt5CVBvecdRQEe_dC-J_a2M/edit?usp=sharing)

:::{admonition} Complete this section prior to class and bring your responses with you (but you do not need to hand them in)
:name: natural-selection-simulation

> ⏳ 10-20 min 

Use the ***Intro*** section of the following simulation to examine the interaction between selection pressures and the phenotypic distribution of a population. Focus on the phenotypes, phenotype frequencies, and selection pressures. Do not focus on the issues of dominant/recessive alleles and allele frequency. 

Once you start the simulation, *add a mate* and introduce a dominant mutation. Let the populaton grow for 2-3 generations before manipulationg any of the other factors in the simulation. Then experiment with different available manipulations and take notes on the results you observe across manipulations that you try. 

<iframe src="https://phet.colorado.edu/sims/html/natural-selection/latest/natural-selection_en.html"
        width="800"
        height="600"
        allowfullscreen>
</iframe>

***HQ1: In this simulation, which bunny phenotype could vary?***

***HQ2: In this simulation, what were the three potential selective pressures that you could manipulate?***

***HQ3: In this simulation, what were the selective pressures that effected relative phenotype distributions in the bunny species?***

:::

(evolution_day1)=
## General evolutionary concepts

A soft warm-up for class.

---
> ⏳ 5 min 

To the best of your group's ability...

***Q1: Define 'adaptation'***

***Q2: What is the main difference between 'evolution' and 'natural selection'?***

***Q3: Does natural selection cause trait variation?***


⏸️ PAUSE here for class-wide discussion

---

## Selective Pressure

:::{admonition} Why?
A fundamental assumption in the contemporary study of animal behaivor, is that behavior is both **heritable**[^heritability] and an **adaptation** (to changing needs and to a changing environment) that maximizes evolutionary fitness[^fitness] (ie. it evolves by **natural selection**). 
:::

[^fitness]: In other words, behavior can convey reproductive advantage. We won't by more explicit about fitness from the perspective of alleles themselves until we have reviewed Genetics as a class. When we talk about fitness, we can think about how well an animal survives. When we talk about phenotypes as adaptations and their evolution, we ultimately do need to think about fitness in terms of the frequencies of gene alleles that give rise to those phenotypes. Allele frequency over generations depends little on the survivability of an individual animal, and more on how much that animal reproduces (and how well its offspring reproduce).

[^heritability]: A key assumption is that behavioral phenotypes are *heritable* across generations (that there is a strong *genetic* component, though we won't get into any actual genetics yet). If an individual has an advantageous trait, then it is more likely to reproduce. Since traits pass from parents to offspring (*heritability*), then offspring are likely to inherit advantageous traits. Over time, advantageous traits become more common in a population.



### Case Study on adaptation: exploitation of behavioral patterns

Behavioral patterns that are stereotyped (ie. FAPs) are, by definition, predictable. As you know from [experiments that test for sign stimuli of FAPs](FAPs-sign-stimuli), if a sign stimulus is encountered, then the FAP will be released, regardless of the source of that sign stimulus[^unless-inhibited]. This ***sign stimulus*** **:** ***FAP*** pair can be thought of as a *code*. ***Code breaking*** describes the "inappropriate" release of an FAP by another animal. 

[^unless-inhibited]: There are many examples of the effect of a sign stimulus being inhibited by a concurrent, but different, stimulus. The effects of sign stimuli can also be enhanced by additional stimuli. 

In solitary ground nesting bee species (that includes the bee families: *Andrenidae*, *Apidae*, *Colletidae*, and *Halictidae*), females dig nests in which they deposit and provision their fertilized eggs with pollen after mating[^Neff-2008].

[^Neff-2008]: [Neff, J.L. Components of nest provisioning behavior in solitary bees (Hymenoptera: Apoidea). Apidologie 39, 30–45 (2008).](https://doi.org/10.1051/apido:2007055)

:::{figure-md}
:class: figure

<img src="/images/solitary-bee-female.png" alt="fishy" class="bg-primary mb-1" width="500px">

**Left**: a female solitary bee collecting pollen. **Right**: a female solitary bee provisioning its egg in a nest.
:::


Males desperately seek females to mate with. They patrol nesting areas in large numbers and form [‘mating balls’ in which multiple males grapple with each other and attempt to pair up with the female](https://drive.google.com/file/d/1T7isPKjRl9pPdahiWVQ_21c2Z3nN3vq-/view?usp=sharing)[^entomology-today][^Russell2018]. The mating sequence of males comprises several **FAP**s that are organized according to *stereotyped transition probabilities*[^Russell2018]. 

[^entomology-today]: [Busy Bees: An Up-Close Look at One Bee Species’ Scramble to Mate](https://entomologytoday.org/2018/09/13/busy-bees-up-close-look-one-bee-species-scramble-mate-diadasia-rinconis/)
[^Russell2018]: [Avery L Russell, Stephen L Buchmann, William de O Sabino, Daniel R Papaj, (2018) Brawls Bring Buzz: Male Size Influences Competition and Courtship in Diadasia rinconis (Hymenoptera: Apidae), Journal of Insect Science, 18(4)](https://doi.org/10.1093/jisesa/iey083)

*But*, males *also* "mate" with aggregates of larval blister beetles. During attempted copulation, the larvae hitch a ride on the male. When the male bee later mates with a female bee, the larvae can then transfer to the female and hitch a ride back to the female's nest. The larvae are parasitic and feed off of the provisions in the nest that were intended for the bee larvae.

:::{figure-md}
:class: figure

<img src="/images/blister-beetle-aggregates.png" alt="fishy" class="bg-primary mb-1" width="400px">

**Top Left**: A female blister beetle depositing eggs on a plant stalk. **Top Right**: Days after hatching, the larval blister beetles aggregate with their brown heads pointing outward. **Bottom**. A male mates with a female bee after a mating attempt with the aggregation of larval blister beetles.
:::

---
> ⏳ 10 min 

***Q4: Based on the information given, what do you think could be the sign stimulus that releases mating FAPs in the male bee? Name at least two potential alternatives.***

***Q5: Under the assumption that behaviors are adaptations, what is the paradox exhibited by this example of solitary bee mating behavior?***

***Q6: Brainstorm potential selective pressures effecting the existence of this mating behavior (sign stimulus : FAP pair) in male bees*** 


⏸️ PAUSE here for class-wide discussion

---

## Evolutionary Models

:::{admonition} Why?
Ultimately, to *understand* a behavioral phenotype from an evolutionary perspective means to be able to predict phenotypes of extant species. This involves both correctly identifying the adaptive role of the behavior and the selective pressures on the behavior. 

Mathematical models are abstractions that strive to have predictive power (with varying degrees of precision). Models represent a best informed guess as to the ***identity and function of important variables*** and ***how these variables interact***.
:::

Two of the most common types of evolutionary models are [Optimality Theory](optimality-theory) and [Game Theory](game-theory)

:::{index} optimality theory
:::

(optimality-theory)=
### Optimality Theory

Remember observing and quantifying [vigilance behavior in meerkats](activity-budget-assignment)? From an evolutionary perspective, let's learn how to understand vigilance behavior using an optimality theory modeling approach. 

Consider the two alternative behavioral phenotypes: 
1. ***vigilant***: animals are sometimes vigilant
2. ***not vigilant***: animals are never vigilant.  

Let's start by examining two factors that likely exert selective pressure on this behavioral variation:
- time available to forage (searching for and eating food)
- probability of avoiding/escaping a predator

---
> ⏳ 5

***Q7: In terms of time foraging and/or probability of escape from predation, what is the 'benefit' of a vigilant phenotype compared to not vigilant?***

***Q8: In terms of time foraging and probability of escape from predation, what is the 'cost' of a vigilant phenotype compared to not vigilant?***

***Q9: In terms of time foraging and probability of escape from predation, what is the 'benefit' of a not vigilant phenotype compared to vigilant?***

***Q10: In terms of time foraging and probability of escape from predation, what is the 'cost' of a not vigilant phenotype compared to vigilant?***


⏸️ PAUSE here for class-wide discussion

---

We often come across evolutionary explanations in terms of *costs* and *benefits*. As you see from this example, these terms are relative. Therefore, it is more *generalizable* to talk in terms of ***factors*** rather than costs or benefits per se. 

---
> ⏳ 10

Let's formalize an optimality theory model for $F$, the net fitness of a phenotype, in terms of the two factors you just examined.

$$
  F = t + e
$$
where $t$ = foraging success (amount and quality of food eaten) and $e$ = predator escape success.  

If there are multiple possible phenotypes (in this case *vigilant* or *not vigilant*), then, by optimality theory, the phenotype that confers greater total fitness to the animal will be favored by natural selection. Therefore, the solution to an optimality model is to figure out which phenotype has a highest net fitness ($F$).

***Q11: Would the vigilant phenotype or the not vigilant phenotype have a higher value of $t$?***

***Q12: Would the vigilant phenotype or the not vigilant phenotype have a higher value of $e$?***

***Q13: Given this information, can you determine which phenotype has a higher net fitness? Choose some arbitrary (but logical) values for the variables $t$ and $e$ in the model to make your prediction.***

***Q14: What kinds of issues are you encountering in using the model to predict which phenotype is more fit?***


⏸️ PAUSE here for class-wide discussion

---

Consider how environments can differ. Do all environments have the same amount or quality of food? What about predators? As you experienced in the [Natural Selection Simulation](natural-selection-simulation), environments exert selective pressure on phenotypes, which means that changing environments can change the relative fitness of two phenotypes... but how?  

Let's account for the effect of environment by adding two new variables to the model: 
- $q$ = the quality or amount of food available
- $p$ = the number of predators

Consider this revised formulation of the model 

$$
  F = q*t + p*e
$$

---
> ⏳ 10

***Q15: Based on this revised model, in an environment with a lot of predators and low food quality, which phenotype would you predict to be favored by natural selection?***

***Q16: Does this revision of the model change your ability to solve the model? If so, then in what ways? If not, then why not?***

***Q17: Given that the models you just explored were examples of 'Optimality Theory Models,' how would you define 'optimality theory'?***

***Q18: What would you do next if your model did not correctly predict vigilance behavior of a population that you were studying?***

⏹️ STOP here for today

---
:::{index} game theory
:::

(game-theory)=
### Game theory

There are many cases in which the fitness associated with a particular behavior depends on what other *conspecifics*[^conspecifics-def] are doing. Thus, what is evolutionarily favored will depend on the distribution of phenotypic variation in the population (and therefore on the likelihood of certain phenotypes interacting, each with different fitness consequences). Game theory is like optimality theory in many ways, but it takes into account ***selective pressure from conspecifics*** and ***the proportion in which other phenotypes exist***. 

[^conspecifics-def]: *Conspecifics* are individuals of the same species. In understanding the evolution of behavior, we consider phenotypic variation *within* a species, not between species.  

---
> ⏳ 15

Let's work through the logic of a game theory modeling approach by role-playing a common example from conflict resolution behavior. In the basic form of this model, there are two possible behavioral phenotypes: *fighter* and *pacifist*. 

(gt-model-setup_fp)=
:::{admonition} Setting up the conflict resolution game theory model
There are two possible behavioral strategies (phenotypes)
1. *Fighters* always fight when challenged until the resource is won. In the simplest case, each fighter has a 50% chance of winning the resource. 
2. *Pacifists* share the resource, and back down immediately when challenged with a fight (they don't engage in any fighting, which means they give up the resource completely when challenged, but also don't get injured from fighting).  

There are two factors that can contribute to an animal's fitness
1. $v$ = the energy gained by obtaining the limited resource
2. $c$ = the damage done by losing a fight over a resource
:::

What happens when each set of behavioral strategies interact?  

:::{admonition} Play it out 
Choose two people from the group to be the 'players'. Players act out the game from the perspective of the behavioral *strategies*. There are two different conditions to act out, as described below.
Choose one person from the group to be the moderator. The moderator starts each round.
Choose one person from the group to keep track of each player's fitness in the game.

**Condition 1: A population of Pacifists** 
Each player represents the pacifist behavior.  

The moderator places one blue pen on the table. This pen is the 'resource' and it is worth +2 units of fitness.  
When the moderator says *go*, both players interact over the resource. Decide how the resource will be allocated according to the 'pacifist' behavioral strategy described [in the model setup](gt-model-setup_fp).
After the resource has been allocated, tally the net change in each player's fitness as a consequence of the encounter.  

The moderator places the blue pen back on the table and the interaction repeats (trial \#2) when the moderator says *go*.  
Repeat the interaction for 10 trials total (tallying each player's change in net fitness after every encounter)

**Condition 2: A population of Fighters**
Each player represents the fighter behavior.  

The moderator places one blue pen on the table. This pen is the 'resource' and it is worth +2 units of fitness.  
The moderator places one red pen on the table. This pen is the consequence of losing a figth and it is worth -1 unit of fitness.

When the moderator says *go*, both players interact over the resource. Decide how the resource and consequence will be allocated according to the 'fighter' behavior described [in the model setup](gt-model-setup_fp).
After the resource and consequence have been allocated, tally the net change in each player's fitness as a consequence of the encounter.  
:::

***Q1: Which behavioral strategy would result in a "more fit" population?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 10

:::{admonition} Play it out 
**Condition 3: Pacifist and Fighters mix**
One player represents the pacifist behavior. 
The other player represents the fighter behavior.  

The values of $v$ and $c$ are the same as in Condition #2. The moderator places one blue pen on the table representing a 'resource' worth +2 units of fitness. The moderator places one red pen on the table representing the consequence of losing a fight and it is worth -1 unit of fitness.

When the moderator says *go*, both players interact over the resource. Decide how the resource and consequence will be allocated according to the 'pacifist' behavior encountering a 'fighter' behavior (and vice versa) as described [in the model setup](gt-model-setup_fp). After the resource and consequence have been allocated, tally the net change in each player's fitness as a consequence of the encounter.  
:::

***Q2: Based on your results of all three simulations, make a table that shows the average net fitness that you tallied for each behavioral strategy (pacifist and fighter) in each behavioral context (pacifist and fighter).***

⏸️ PAUSE here for class-wide discussion

---

The game theory model that you have been playing out can be summarized in general terms according to the following equations.

|  | In a population of fighters | In a population of pacifists |
| :--- | :---: | :---: |
| **Average net fitness for a fighter** | ${(v-c)}/2$ | $v$ |
| **Average net fitness for a pacifist** | 0 | $v/2$ |

After a fighter encounters another fighter, its fitness changes by $ F = v $ if it wins but $ F = -c $ if it loses. Since it wins 1/2 the time, the average fitness is $v/2 - c/2$.
After a pacifist encounters another pacifist, its fitness changes by $ F = v/2 $ because they share the resource.
Fighters always gain the resource against pacifists and do so without a fight, which means pacifists end up with nothing against fighters.

The conditions that you acted out were: $v=2$ and $c=1$.  

Under these conditions, let's use the model equations to determine which strategy has a greater net fitness in a population of all fighters. By doing so, we can determine whether (*under these conditions*) fighting is a **stable** behavior or a behavior that would be **invaded by** pacifist behavior.

---
> ⏳ 10

***Q3: Under the conditions that you acted out, use the model equations to determine which strategy has a greater net fitness in a population of all pacifists.***

***Q4: According to this evolutionary model, the fitness of the fighter phenotype (DOES / DOES NOT) depend on the behavioral phenotype of conspecifics. When conspecifics are all fighters, the average fitness of fighting is ________. When conspecifics are all pacifists, the average fitness of fighting is (ALSO / INSTEAD) ________. (choose one parenthetical option and fill in the blanks)***

Consider a new set of conditions. For example, what about an environment in which there are more predators. In this environment, the cost of losing a fight may be greater because if you are injured, you have a high probability of being eaten by a predator. Consider that $v=2$ and $c=3$.  

***Q5: In this different environment, where $v=2$ and $c=3$, which strategy has a greater net fitness in a population of all fighters?***

***Q6: In this different environment, where $v=2$ and $c=3$, which strategy has a greater net fitness in a population of all pacifists?***


⏸️ PAUSE here for class-wide discussion

---

Game theory models like the pacifist : fighter model you have been considering, are often represented in the following tabular format. It is worth getting familiar with this way of representing game theory models, because using the table aids in model analyis (makes the process of solving the model more *algorithmic*).

:::{figure} /images/game-theory-figher-pacifist.png
:width: 600

A tabular representation of the game theory model of conflict resolution behavior that includes *pacifist* and *fighter* phenotypes. **A**) Each box of the table is split by a diagonal line. The fitness of each phenotype in each player role (green or purple) is written to the left or right (respectively) of each diagonal line. **B**) An equivalent representation of this model. Because this model is *symmetric* (there is only one type of individual/role that could exhibit each behavior), the payoffs can be represented once for individuals (left) in each phenotype context (top).
:::

#### Solving the model

Game theory models are solved a bit differently than Optimality Theory. The task is to determine ***under what conditions*** (values of the variables/factors) is each behavior(s) ***stable***. 

For example, fighting is stable when the strategy *cannot be invaded by* the pacifist strategy. This is only true when pacifists have a lower average fitness than fighters when in a population of fighters (ie. a *mutant* pacifist). Mathematically, this statement would be written:
Fighting is a stable strategy when ${(v-c)}/2 > 0$. Simplifying the equation gives the condition: $v > c$.

---
> ⏳ 10

***Q7: Are there conditions under which pacifist would be a stable behavior? To solve, set up the relevant inequalities and simplify to find the conditions under which pacifist would be stable. Then state in terms of a sentence.***

***Q8: Are there conditions under which the evolutionarily stable state of a species would include both pacifists and fighters? How many inequalities do you need to set up for this analysis? What are the conditions that need to be satisfied? Solve for the conditions under which a population at evolutionary equilibrium would comprise both pacifists and fighers simultaneously.***


⏸️ PAUSE here for class-wide discussion

---

(multiple-mating-systems-lizard)=
#### Understanding MIXED behavioral phenotypes

It is possible that there are conditions under which neither behavioral phenotypes alone are evolutionarily stable, but a population consisting of both co-existing phenotypes is. For example, we know of behavioral phenotypes that have higher fitness than the alternative only when that alternative exists.

Here are a few as examples:
- *sitter* versus *rover* foraging behavior ([fruit flies](https://doi.org/10.1038/nature05764))
- *singing* versus *silent* mate attraction behavior ([crickets](https://doi-org.ezproxy.wesleyan.edu/10.1098/rsbl.2006.0539)) 
- *fighter* versus *pacifist* resource conflict resolution (when the cost of losing a fight is high)
- *sneaky* versus *dominant* versus *monogamous* mating behavior (side-blotched lizards... see video and game theory model below)

<div class="pbs-viral-player-wrapper" style="position: relative; padding-top: calc(56.25% + 43px);"><iframe src="https://player.pbs.org/viralplayer/2365819768/" allowfullscreen allow="encrypted-media" style="position: absolute; top: 0; width: 100%; height: 100%; border: 0;"></iframe></div>

The game theory model below summarizes the relative fitness of each mating behavior in the context of all others. These mating phenotypes have also been observed simultaneously in several other species of anmimals. $F$ is the baseline fitness. 

|  | Dominant | Sneaky | Monogamous |
| :--- | :---: | :---: | :---: |
| **Dominant** | F | F - 1 | F + 1 |
| **Sneaky** | F + 1 | F | F - 1 |
| **Monogamous** | F - 1 | F + 1 | F |

Simulating this game theory model gives the following result:

:::{image} /images/game-theory-simulation-lizards.png
:width: 600
:::

All three behavioral phenotype exists *simultaneously* at evolutionary equilibrium (after many generations of time). No one individual behaivor is ever evolutionarily stable (ie. we would never predict a population of only Dominant mating behavior). The three phenotype variants exist with a frequency of 33.333% (1/3).

Let's think about the following together:
1. If the population was initialized with fewer dominant phenotypes (ie. there are very few dominant individuals in the population) and equal sneaky and monogamous, which phenotype would we expect to increase in frequency: sneaky or monogamous? 
2. Once that phenotype dominated, which phenotype would then have the highest net fitness?

We can simulate \#1 and \#2 to test our predictions. This [Demo Simulation](http://pages.nbb.cornell.edu/Gamebug/gbg/gbg.html) (popup) is a good resource for gaining more intution for the interactions among phenotypes. 

⏹️ STOP here for today

---

## Additional Resources

- [This video](https://youtu.be/YNMkADpvO4w) is a simulation on the evolution of conflict resolution behaviors that provides a nice perspective on the logic of game theory models in understanding behavior. Think about, what is the paradox here? 
- Silent versus Satellite Crickets: [To mate or be eaten: tree cricket behaviour in the presence of a predator](https://www.britishecologicalsociety.org/to-mate-or-be-eaten-tree-cricket-behaviour-in-the-presence-of-a-predator/) and [Silent night: adaptive disappearance of a sexual signal in a parasitized population of field crickets](https://doi-org.ezproxy.wesleyan.edu/10.1098/rsbl.2006.0539) and [A simulation model of the effects of frequency dependence,
density dependence and parasitoid flies on
the fitness of male field crickets](https://doi.org/10.1016/j.ecolmodel.2003.07.001)
- [Optimality Theory section from Rubenstein and Alcock text](https://drive.google.com/file/d/11ixpv0rAw6nJ9arHLuvGWjU15dcFxF7B/view?usp=sharing)
- [Game Theory section from Rubenstein and Alcock text](https://drive.google.com/file/d/1M4vDEonIg9XLL4c8I5S4Xe0E5Rw5EiME/view?usp=sharing)
- [Observations of the blister beetle Stenoria analis (SCHAUM, 1859) in a colony of the ivy bee Colletes hederae SCHMIDT & WESTRICH, 1993 in the botanical garden of Gießen in 2016 and 2017](https://www.kerbtier.de/Pages/Themenseiten/enStenoria.html) © Hans Bahmer, 2017
- [Modeling Behavior: Game and Optimality Theory](https://college.holycross.edu/faculty/kprestwi/behavior/ESS/ESS_introModels.html) from Holy Cross College
- [Game Theory and Evolutionarily Stable Strategies](https://college.holycross.edu/faculty/kprestwi/behavior/ESS/games_intro.html) from Holy Cross College
- [Game Theory Tutorial: Conflict, Probability, Stable Strategies](http://pages.nbb.cornell.edu/Gamebug/conflict.html)
- [PHET Natural Selection Lab](https://phet.colorado.edu/en/simulations/natural-selection)
- [Kahn Academy](https://www.khanacademy.org/science/biology/her)
- [Berkeley's *Understanding Evolution*](https://evolution.berkeley.edu/)
- [*Primer* playlist on Evolution at YouTube](https://www.youtube.com/playlist?list=PLKortajF2dPBWMIS6KF4RLtQiG6KQrTdB)
- [Game Theory 101: The Hawk-Dove Game at YouTube](https://youtu.be/RAKjII7xCdk)
- [Fitzpatrick, M., Feder, E., Rowe, L. et al. Maintaining a behaviour polymorphism by frequency-dependent selection on a single gene. Nature 447, 210–212 (2007).](https://doi.org/10.1038/nature05764) provides and example of negative frequency-dependent selection in which the underlying genes for the behavioral variation is known. 
- [Common Descent Podcast, Episode 56: The Evolution of Evolutionary Theory](https://www.youtube.com/watch?v=dPFwp7zC8RY&list=PLfdiT8Klm_YPa0lNVa9ygwAjy_1Lpz9_S&index=60)
- [Game Theory Tutorial: Conflict, Probability, Stable Strategies](http://pages.nbb.cornell.edu/Gamebug/conflict.html)
- [Game Theory Tutorial: Territoriality (conflict II)](http://pages.nbb.cornell.edu/Gamebug/conflict2.html)
