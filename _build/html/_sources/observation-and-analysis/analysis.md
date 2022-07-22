---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Analysis

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neurologic/Comparative-Animal-Behavior/main)

## Focal versus scan sampling

+++

***Q: You are interested in how manakin birds sequence behavioral actions during courtship rituals. Would it be more appropriate to use focal or scan sampling? Why?*** 

+++

Answer

+++

***Q: You are interested in the activity budget of african elephants under captive versus wild conditions. Would it be more appropriate to use focal or scan sampling? Why?*** 

## Continuous versus interval sampling

***Q: Would it be better to use continuous or interval sampling when recording the behavior of multiple animals simultaneously? Better in what way? What would be a downside of that sampling method choice?***

## Activity budgets and transitions

Why would some behaviors happen more than others? Do some behaviors happen more than others?

***Q: What activity budget would you expect "by chance" for each behavior in an ethogram? Calculate this 'null hypothesis' for an animal with an ethogram of 5 behaviors: X, Y, Z, A, and P.***  

What about the sequence of behaviors? Are behaviors independent of each other or are some behaviors more likely to follow each other? Can you think of any examples?

For any sequence of non-independent events in the world, and where a limited number of outcomes can occur, conditional probabilities can be computed relating each outcome to one another. Often this simply takes the form of counting how often certain outcomes follow one another in an observed sequence, and normalizing by the total number of transitions to calculate a probability. 

These concepts are often used to analyze language. As an illustration of the concept, consider the following poem.

:::{epigraph} 
One fish two fish red fish blue fish.

--Dr Suess
:::

***Q: How many possible words are there (given the poem)?***

***Q: As an analogy to behavior, what is the 'activity budget' for each word?***

A *transition matrix* for an ethogram is a table that summarizes the probability that each behavior in the ethogram follows another. For each pair of sequential actions recorded, the rows represent the preceding action and the columns the succeeding action. Before doing this analysis on behavior, practice it on the Dr Suess poem.

***Q: How many time does each word follow each other word in the Dr Suess poem? Make a square table with all possible words in the rows and all possible words in the columns. To tally transitions, preceeding words are rows and suceeding words are columns. Tally the total number of each transition ($t$). Tally the total number of transitions out of each unique word ($n$). Calculate the transition probability for each word to each other word as $p = t/n$***

Here is an illustration of transition probabilities for this excerpt and how it relates to the sequencing of the poem. 

:::{figure-md} markdown-fig
<img src="../images/One-Fish-Two-Fish_Markov.gif" alt="fishy" class="bg-primary mb-1" width="600px">

Markov model of Dr Seuss' fish poem.
:::



***Q: Which of the following transition matrices (A or B) was more likely calcualted using continuous sampling methods? Which was more likely calculated using interval sampling methods? Why?***

 1.  
|  | A | B | C |
| --- | --- | --- | --- |
| A | 0 | 0.2 | 0.8 |
| B | 0.8 | 0 | 0.2 |
| C | 0.2 | 0.8 | 0 |

 2.  
|  | A | B | C |
| --- | --- | --- | --- |
| A | 0.1 | 0.6 | 0.3 |
| B | 0.1 | 0.2 | 0.7 |
| C | 0.8 | 0.2 | 0 |



## Changing priorities influence motivation: case study on vigilance

Watch [this clip](https://vimeo.com/80600820) of meerkats engaging in vigilance behaviors. 

**Vigilant**: Head raised at or above horizontal plain and eyes open. 

***Q: What function could vigilance serve?***

***Q: What behaviors do you observe when vigilance is not ocurring?***

To test whether vigilance functions in avoiding predation, you will quantify behavior based on a simplified ethogram including three behaviors:
1. vigilant (head raised at or above horizontal plain and eyes open)
2. not vigilant (eyes closed or head lower than horizontal plane) 
3. out of sight (not visible by you, the researcher)

You will watch three different videos, each with a different *predator* treatment condition.
- [No predator](https://vimeo.com/80600822)
- [Terrestrial predator](https://vimeo.com/71877438)
- [Aerial predator](https://vimeo.com/80600821)

Set a timer to go off every 10 seconds, and at each interval record the number of meerkats performing each behavior. 

***Q: Use your results to present an argument for or against the hypothesis that "vigilance serves an anti-predator function" and that "vigilance is more useful against terrestrial predators"***

***Q: What other function(s) did you hypothesize for vigilance? How would you test another possible function that you posed?***

Next, you will use continuous focal sampling to investigate whether the proximity of a detected predator influences the activity budget of meerkat behavior. Again, you will consider 'vigilant', 'not vigilant', and 'out of sight’ as the three behaviors comprising the ethogram for this study. Data should be collected for ONE meerkat at each distance of predator presentation (0 m, 2 m, 4 m, 6 m, 8 m, 10 m, 12 m, 14 m). Record the start time of each behaviour on a new line as shown:

| **Behavior** | **Start time** | **Duration** |
| --- | --- | --- |
| name of behavior | cummulative seconds | calculated | 

We will want 3 repititions (different observers) of the analysis at each distance. 

***Q: What behavioral metric (based on your continuous sampling data) do you propose to calculate to test if predator proximity influences the trade-off between vigilant and non vigilant behavior (activity budget)? Define any relevant mathematical equation(s) for your calculation(s).***

Watch [the video clip](https://vimeo.com/77501205) corresponding to the distance you are responsible for and collect your data. 
| distance | start time in video |
| ---| --- | 
| 14m | 0:10 |
| 12m | 3:11 |
| 10m | 6:32 |
| 8m | 9:39 |
| 6m | 12:46 |
| 4m | 15:52 |
| 2m | 18:58 |
| 0m | 22:01 |

We can carry out a Spearman rank correlation test to see if there is a relationship between predator distance and vigilance behaviour.

___

## Take Home Work

***Q: Carry out the same experiment, but use an interval scan sampling method instead. For simplicity, collect data only for the following distances: 14, 10, 6, 2m). Create a figure to clearly report your results. Clearly describe your sampling protocol/method. Define any calculations that you did on the raw data.***

***Q: Create an ethogram for an animal you are interested in. Give it to your partner. Use the ethogram to create a transition matrix of behavior. Make sure to include what samping method you used. Show a table of your raw transition data and describe the calculation used to obtain probability.***


___

Resources used in this workshop: 
- [denajane13 bookdown](https://bookdown.org/denajane13/BIONB_2210_Summer_2021/field-lab-2-ethograms-and-activity-budgets.html#part-1.-build-an-ethogram-from-meerkat-observations)
- [Hammond 2019, Vigilance behaviour in meerkats, ASAB Education](https://www.asab.org/s/EDU-ASAB-Vigilance-behaviour-in-meerkats-compressed.pdf)