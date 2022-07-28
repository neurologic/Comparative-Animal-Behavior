# Analysis

> ⏳ 10 min

***Q: Discuss your summaries of the sampling methods defined by Altmann[^Altmann] and come up with a single list according to group concensus.***

[^Altmann]: [Jeanne Altmann 1973 *Observational Study of Behavior: Sampling Methods* Behaviour
49(3/4).](https://www.jstor.org/stable/4533591)

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 5 min

## Focal versus scan sampling

***Q: You are interested in how manakin birds sequence behavioral actions during courtship rituals. Would it be more appropriate to use focal or scan sampling on a group of 5 birds? Why?*** 

***Q: You are interested in the activity budget of african elephants under captive versus wild conditions. Would it be more appropriate to use focal or scan sampling on a group of 5 elephants? Why?*** 

## Continuous versus interval sampling

***Q: Would it be better to use continuous or interval sampling when recording the behavior of multiple animals simultaneously? Better in what way? What would be a downside of that sampling method choice?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 

## Activity budgets

Do some behaviors happen more than others? Why might some behaviors happen more than others? 

As an illustration of the concept, consider the following poem.

:::{epigraph} 
One fish two fish red fish blue fish.

--Dr Suess
:::

***Q: How many possible words are there (given the poem)?***

***Q: As an analogy to behavior, what is the 'activity budget' for each word?***

***Q: What 'activity budget' would you expect 'by chance' for each behavior in an ethogram? Calculate this 'null hypothesis' for an animal with an ethogram of 5 behaviors: X, Y, Z, A, and P.***  


## Changing priorities influence motivation: case study on vigilance

Watch [this clip](https://vimeo.com/80600820) of meerkats engaging in vigilance behaviors. 

**Vigilant**: Head raised at or above horizontal plain and eyes open. 

***Q: What function could vigilance serve?***

***Q: What behaviors do you observe when vigilance is not ocurring?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 

To test whether vigilance functions in avoiding predation, you will quantify behavior based on a simplified ethogram including three behaviors:
1. vigilant (head raised at or above horizontal plain and eyes open)
2. not vigilant (eyes closed or head lower than horizontal plane) 
3. out of sight (not visible by you, the researcher)

You will watch three different videos, each with a different *predator* treatment condition.
- [No predator](https://vimeo.com/80600822)
- [Terrestrial predator](https://vimeo.com/71877438)
- [Aerial predator](https://vimeo.com/80600821)

For each video, record the number of meerkats performing each behavior at 10 second intervals. 

***Q: What type of sampling method[^Altmann] is this?***

***Q: Use your results to present an argument for or against the hypothesis that "vigilance serves an anti-predator function"***

***Q: Use your results to present an argument for or against the hypothesis that "vigilance is more useful against terrestrial predators"***

***Q: What other function(s) did you hypothesize for vigilance? How would you test another possible function that you posed?***

***Q: How do you think the proximity of a predator would influence the activity budget of meerkat behavior?***

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 

## Sequences of behavior

What about the sequence of behaviors across time? Are behaviors independent of each other or are some behaviors more likely to follow each other? Can you think of any examples?

For any sequence of non-independent events in the world, and where a limited number of outcomes can occur, *conditional probabilities* relate each outcome to one another. For example, if you smile at me, you are more likely to hug me than to hit me (the conditional probability of a hug following a smile is bigger than a hit following a smile). 

A *transition matrix* for an ethogram is a table commonly used to summarize the probability that each behavior in the ethogram follows another. Before doing this analysis on behavior, practice it on the Dr Suess poem.

:::{epigraph} 
One fish two fish red fish blue fish.

--Dr Suess
:::

***Q: Make a square table with all possible words in the rows and all possible words in the columns. Count how many times each word follows each other word in the Dr Suess poem and log it in the table. For each pair of sequential words, the rows represent the preceding word and the columns the succeeding word.***

***Q: Calculate transition probabilities for each word to each other word as $p = t/n$, where $t$ is the total number of each transition and $n$ is the total number of transitions out of the preceeding word (usually the total number of times the word occurred).***

You now have a model that describes how Dr. Suess' poem is sequenced. 

The model that you just created can be visualized graphically for a different perspective on the concept.  

:::{figure-md} markdown-fig
<img src="../images/One-Fish-Two-Fish_Markov.gif" alt="fishy" class="bg-primary mb-1" width="600px">

Markov model of Dr Seuss' fish poem.
:::

⏸️ PAUSE here for class-wide discussion

---
> ⏳ 

Examine the following two transition matrices. 

One:  
|  | A | B | C |
| --- | --- | --- | --- |
| A | 0 | 0.2 | 0.8 |
| B | 0.9 | 0 | 0.1 |
| C | 0.4 | 0.6 | 0 |  

Two:  
|  | X | Y | Z |
| --- | --- | --- | --- |
| X | 0.1 | 0.7 | 0.3 |
| Y | 0.1 | 0.4 | 0.5 |
| Z | 0.8 | 0.2 | 0 |

There are two 'rules' to follow in constructing a transition matrix.

***Q: First, the rows of the transition matrix must total to ________ (fill in the blank with a number).***

***Q: Second, there has to be ( the same / a different ) number of rows as columns (pick one answer).***

But how do you *read* a transition matrix to predict (and therefore understand) an animal's behavior over time?

***Q: According to matrix \#1, which behavior is most likely to follow behavior A?***

***Q: According to matrix \#1, which behavior is most likely to follow behavior C?***

These transition matrices can also be represented graphically with circles (behaviors) and arrows (transition probabilities). Examine [this animation of transition matrix number one](https://setosa.io/markov/index.html#%7B%22tm%22%3A%5B%5B0%2C0.2%2C0.8%5D%2C%5B0.9%2C0%2C0.1%5D%2C%5B0.4%2C0.6%2C0%5D%5D%7D) and [this animation of transition matrix number two](https://setosa.io/markov/index.html#%7B%22tm%22%3A%5B%5B0.1%2C0.7%2C0.2%5D%2C%5B0.1%2C0.3%2C0.6%5D%2C%5B0.8%2C0.2%2C0%5D%5D%7D). Examine how the transition matrix is annotated in these animations. You will use this tool later to create your own.

***Q: What corresponds to each row of transition matrix \#1? Which corresponds to each column of transition matrix \#1?***

***Q: According to matrix \#1, what is the most likely behavioral sequence (of 5 elements) generated by this species?.***

***Q: According to matrix \#2, what is the most likely behavioral sequence (of 5 elements) generated by this species?***

***Q: According to matrix \#2, what is the least likely behavioral sequence (of 5 elements) generated by this species?***

***Q: Which of the two transition matrices was more likely calculated using continuous sampling methods? Which was more likely calculated using interval sampling methods? Why (what evidence do you have to support that conclusion)?***

⏹️ STOP here for today

Extension project...
***Q: Create an ethogram for an animal you are interested in. Trade ethograms with someone else. Use the ethogram to create a transition matrix of behavior. Make sure to include what samping method you used. Show a table of your raw transition data and describe the calculation used to obtain probability. Use [this url address](https://setosa.io/markov/index.html#%7B%22tm%22%3A%5B%5B0.5%2C0.5%5D%2C%5B0.5%2C0.5%5D%5D%7D) to create an animation of your transition matrix. Edit the transition matrix at the top right based on your results. Then copy the new url and provide the link in your answer.***


---
## Additional Resources

- [Transition Matrices and Markov Chains](https://setosa.io/blog/2014/07/26/markov-chains/index.html)
- [And extended description of the *One fish Two fish* example for building a markov model](https://hackernoon.com/from-what-is-a-markov-model-to-here-is-how-markov-models-work-1ac5f4629b71)
- If you are interested in computer programming and Markov models for various applications beyond animal behavior, [this example notebook for analyzing markov models of text](https://www.kaggle.com/code/nulldata/meaningful-random-headlines-by-markov-chain/notebook) might be of interest to you.

---
Resources used in this workshop: 
- [denajane13 bookdown](https://bookdown.org/denajane13/BIONB_2210_Summer_2021/field-lab-2-ethograms-and-activity-budgets.html#part-1.-build-an-ethogram-from-meerkat-observations)
- [Hammond 2019, Vigilance behaviour in meerkats, ASAB Education](https://www.asab.org/s/EDU-ASAB-Vigilance-behaviour-in-meerkats-compressed.pdf)

---
Markov simulation code

:::{code}
import numpy as np

def make_pairs(corpus):
    for i in range(len(corpus)-1):
        yield (corpus[i], corpus[i+1])

<!-- # Trump's speeches here: https://github.com/ryanmcdermott/trump-speeches
trump = open('/content/speeches.txt', encoding='utf8').read()

corpus = trump.split()

 -->
s = 'one fish two fish red fish blue fish '
corpus = s.split()

pairs = make_pairs(corpus)

word_dict = {}

for word_1, word_2 in pairs:
    if word_1 in word_dict.keys():
        word_dict[word_1].append(word_2)
    else:
        word_dict[word_1] = [word_2]
 
first_word = np.random.choice(corpus)

while first_word.islower():
    first_word = np.random.choice(corpus)

chain = [first_word]

n_words = 20

for i in range(n_words):
    chain.append(np.random.choice(word_dict[chain[-1]]))

' '.join(chain)
:::