# Components of Behavior, Observation, and Analysis


:::{admonition} Deadline
Due by 11pm on Friday February 24.
:::

:::{admonition} Honor Code
This exam is open note/book/web, but must be done independently. Do not consult any other people (regardless of whether they are in or out of this course) or artificial intelligence (AI) in answering the questions. Handing in responses to assignment for grading serves as your signature of the honor code.
:::

Answer all questions either electronically or by hand. Label each of your answers with the corresponding question number. Scan or convert your document to a good quality PDF. Upload to gradescope by the deadline -- make sure to tag all appropriate page(s) in your PDF for each question. 

**Please don’t hesitate to ask for clarifation on the wording of questions and/or expectations**. Key expectations are highlighted with font style. For any multiple choice question that asks for an explanation of your reasoning: I am looking for a correct answer selection as well as reasoning for selecting that answer - the reasoning should logically (and unabiguously) explain for your answer selection. Not all multiple choice questions require for reasoning.



## Section 1 

Bechard and Mason (2010) were the first to research the independence of lab mice compared to wild mice. To do this, they used a novel lab housing system that allowed young, developing mice (pups) to choose between spending time in the home cage (HC) with the mother, or an identical distant cage (a ‘dispersal cage’: DC) which the mother could not access. Their objective was to determine the age at which young lab mice prefer to spend time in a distant cage not containing their mother. To do so, they used the experimental ethogram shown in Table 1. They used live observation techniques rather than video recording (due to the ability of a live observer to move around and keep tracking animals when they go out of sight). 

:::{image} /images/bechard-mason-2010.png
:width: 700
:align: center
:::


**Q: (2 points)** In this study, the researchers needed to calculate the activity budget of mouse pups, but they did not care about the action transition probabilities. Therefore, they could implement [***choose an option from below***], which they would not have been able to do if they needed to calculate transition probabilities among actions. 
- continuous scan sampling
- continuous focal sampling
- interval focal sampling
- interval scan sampling

**Q: (4 points)** Mice spend the majority of time inactive, and so the place where they spend most of their inactive time is suggested to be the ‘preferred location’ (Blom et al., 1992) of a healthy animal. To determine which cage location (HC or DC) the pups preferred, the activity and location of the entire litter were calculated as a percentage of pups per cage. Which of the following data tables (1 or 2) is most likely an excerpt from the one the researchers collected. Explain why you chose that answer. 

Table 1
| behavior | location | time (min) | duration (min) |
| :---:  | :---: | :---: | :---:  |
| active  |  HC |  0:00 | N/A  |
| inactive  | HC  | 1:10  | 1:10  |
| active  |  DC |  1:30 | 0:20  |
| active | HC  | 2:30  |  1:00 |

Table 2
| time (min) | HC active | HC inactive | DC active | DC inactive |
| :---:  | :---: | :---: | :---:  | :---: |  
| 0:00  | 3 | 2 | 1  | 0 |  
| 1:00  | 2 | 1 | 2  | 1 |  
| 2:00  | 3 | 3 | 0  | 0 |  
| 3:00  | 0 | 0 | 4  | 2 |  


**Q: (2 points)** These researchers were also interested in the parental care behavior of mouse mothers (dams). They wanted to compare both the activity budget and the action sequencing (ie action transition probabilities) of wild versus lab dams. Therefore, they needed to implement [***choose an option from below***] to record behavioral data for dams.
- continuous scan sampling
- continuous focal sampling
- interval focal sampling
- interval scan sampling


The following sequence of actions was observed for a dam:  
**GO, GF, GO, R, GF, GO, GP, N, GP, L, PR, N, GF, GO, R, N, GF, L, PR, L, GO, R, N, R, PR, R, PR, R, L, GO, GF** 
> R: resting with pups, GO: grooming on, GF: Grooming off, GP: grooming pups, N: nursing, L: licking pup, PR: pup retrieval


**Q: (2 points)** From the sequence of observed Dam behaviors, calculate and show the transition probability matrix. 

**Q: (2 points)** Using the same data, calculate and plot the activity budget among the 7 actions observed. 

**Q: (2 points)** Calculate the null hypothesis for the activity budget and then report the comparison of the calculated activitiy budget against that null hypothesis. 


## Section 2 

Herring gull chicks need help obtaining food. They have a stereotyped "begging" behavior: when chicks see their parent's head, they peck at the beak. The pecking then causes their parents to regurgitate partially-digested food that the chicks can eat ([though I guess the results are not guaranteed to please](https://youtu.be/a-ek4225__I)). The hunger level of the chicks can also effect the liklihood that they will beg (their motivation to beg). Tinbergen and Perdeck tested a wide variety of herring gull features to determine sign stimuli for begging[^tinbergen-gulls-1950]. Figure 1 shows the results of a small subset of their experiment for you to examine. 

[^tinbergen-gulls-1950]: No need to read it to complete this exam, but here is the reference if you are interested:	[Tinbergen, N., & Perdeck, A. C. (1950). On the Stimulus Situation Releasing the Begging Response in the Newly Hatched Herring Gull Chick (Larus Argentatus Argentatus Pont.). Behaviour, 3(1), 1–39](http://www.jstor.org/stable/4532715)

:::{image} /images/tinbergen-expt-gulls.png
:width: 600
:::

**Figure 1:** Results from one of Tinbergen and Perdeck's experiments on the begging behavior of herring gull chicks. Each of the three stimuli (models of a gull head) were presented to chicks. Tinbergen and Perdeck counted the number of pecks directed toward each stimulus during a 30 second period. They then calculated and reported the peck rate (purple). 

**Q: (4 points)** Would you conclude that a gull-shaped head is a sign stimulus for pecking FAPs? Answer *YES* or *NO*. Then support your conclusion with specific quantitative comparisons from the reported experimental results.     


:::{image} /images/stimulus-threshold-in-action.png
:width: 700
:::

**Figure 2:** Examples of behavior expression in two scenarios (A and B) depiced using a Lorenz-style model. FAP=fixed action pattern. a.u.=arbitrary units. 

**Q: (4 points)** Refer to Figure 2. Which stimulus was presented in A? 
**a)** stimulus 2 (egg-shaped head with a red dot on the beak)  
**b)** stimulus 3 (gull-shaped head without any red the beak)
Explain why you chose that answer.

**Q: (2 points)** Question about stimulus threshold and behavioral threshold.

