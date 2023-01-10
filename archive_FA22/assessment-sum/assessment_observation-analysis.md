# Observation and Analysis of Behavior

:::{admonition} Deadline
Due by midnight on Monday September 26.
:::

:::{admonition} Honor Code
This exam is open note/book/web, but must be done independently. Do not consult any other people (regardless of whether they are in or out of this course) in answering the questions. Handing in responses to assignment for grading serves as your signature of the honor code.
:::

Answer all questions either electronically or by hand. Label each of your answers with the corresponding question number (Q1 - Q11). Scan or convert your document to a good quality PDF. Upload to gradescope by the deadline. 


## Section 1: Vigilance in Barnacle Geese

For this section, you will observe (by watching a pre-recorded video) *vigilant* behavior of barnacle geese (*Branta leucopsis*) during foraging. [The video](https://www.youtube.com/watch?v=oeJHW5n-PXY) starts with some background about the barnacle geese and a bit of an overview about the experiment that you will analyze. The experiment starts at 3min. You can skim the video to get a sense of its organization and camera view, but don't worry about detailed observation until reading through the experimental tasks in this section. 

**vigilant** is defined (for this experiment) as *the animal having it's head up*. Use this definition when categorizing your observations.  
All other behavior can be categorized as "other" or "out of sight" as needed.

Throughout the video, the camera focuses on single geese. The video is sectioned into different experimental bouts. For each bout, there is one focal goose. For each bout, the *flock size* (number of geese in the foraging flock) is different. 

When you watch the video for data collection, you will need to record any information/data that will enable you to calculate (for each experimental condition) both of the following metrics of vigilant behavior:
1. the number of *vigilant* events per minute (ie. rate) 
2. the percent of time spent *vigilant*

Organize a table for data collection that will enable you to calculate both of these quantities without needing to watch the video more than once (mimicking a scenario in which you are observing in real time). Try to make a plan that is as efficient as possible so that you are not trying to record too much information at the same time.

***Q1 (2 points): List and explain the information/data that you plan to record while observing. Do not include data that you can calculate after you have observed. (There may be some variety among correct answers to this question. Just try to be efficient with your data collection plan and make sure that you will be recording all information necessary for completing both analyses.)***

Now, watch the video and record your data.

***Q2 (2 points): For just one example experimental condition, provide a table of the raw data you collected. The table should include only the information that you recorded while observing the geese.***

***Q3 (4 points):  
a) Make (and show) a scatterplot of the number of vigilant events per minute for each experimental condition. (The scatterplot can either be done by hand on paper and photographed, or by using a plotting program on the computer)  
b) Was this data that you explicitly recorded while watching; or did you calculate it after?  
c) If you did not explicitly record it, how did you calculate the number of vigilant events per minute from the data that you did record?***

***Q4 (4 points):  
a) Make (and show) a scatterplot of the percent of time devoted to vigilance for each experimental condition. (The scatterplot can either be done by hand on paper and photographed, or by using a plotting program on the computer)  
b) Was this data that you explicitly recorded while watching; or did you calculate it after?  
c) If you did not explicitly record it, how did you calculate the percent of time spent vigilant from the data that you did record?***

This experiment was designed to test the effect of flock size on vigilance behavior. To test this, vigilant behavior was quantified by treating vigilant behavior both as events (1: number of events per minute) and as states (2: percent time).  

***Q5 (4 points):  
a) Based on your results, what conclusion would you draw about the effect of flock size on vigilant behavior?  
b) Did both metrics (number of vigilant events per minute and percent time spent vigilant) yield the same conclusion, or did the conclusion depend on the analysis method? (NOTE: you do not need to do any formal statistics because we did not cover that in class. Just base your answer on the trends you observe in the data.)  
c) Explain your reasoning for your answer in 'b'.***

***Q6 (1 point): You have now had experience with both focal and scan sampling methods. Which did you prefer, and why? (1-4 sentences; There is not one correct answer. Use your experiences to formulate and explain your opinion.)***

***Q7 (1 point): You have now had experience with both continuous and interval sampling methods. Which did you prefer, and why? (1-4 sentences; There is not one correct answer. Use your experiences to formulate and explain your opinion.)***


## Section 2: Activity Budgets and Sequencing

:::{admonition} Note
It takes a lot of observation hours/days/etc to obtain enough data to estimate conditional probabilites among actions in an animal's ethogram. So for this section, you will not be conducting the data collection. Instead, use the provided data to answer the questions.
:::

Grooming in Drosophila melanogaster is characterized by repeated execution of distinct, stereotyped actions: head (h), front leg (f), abdomen (a), back leg (b), wing (w), and walk (wk).[^fig-refs]

:::{image} /images/drosophila-grooming-ethogram.png
:width: 500
:align: center
:::

**Figure 1**: Most grooming actions are categorized according to the body part at which a rubbing motion is directed ("walk" action is included as a grooming action, but is not pictured).


### Activity Budget

***Q8 (2 points): What is the null hypothesis for the activity budget (percent time) across grooming actions in Drosophila?***

***Q9 (2 points): How do the published results shown in Figure 2 compare to the null hypothesis for each action?  
a) List the actions that occur more than expected.  
b) List the actions that occur less than expected.***

:::{image} /images/drosphila-grooming-activity-budget.png
:width: 250
:align: center
:::

**Figure 2**: Activity budget reported in Mueller et al (2019)[^fig-refs] for drosophila grooming actions. 

### Action Sequencing

Grooming actions do not always occur in the same order. Mueller et al (2019) annotated over 40 hours of video data of flies covered in dust and developed mathematical models (Markov models) to examine action sequencing in D. melanogaster grooming (Figure 2).[^fig-refs] 

[^fig-refs]: *Figures 1-3* are from the paper titled: [Drosophila melanogaster grooming possesses syntax with distinct rules at different temporal scales](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007105). No need to read the paper to answer any of these exam questions.  


:::{image} /images/drosphila-grooming-markov.png
:width: 700
:align: center
:::

**Figure 3**: Left: Ball and arrow diagram showing the probability of transitions among grooming actions. Right: Same data (conditional probabilities between current and future state), but presented as a table. *High* conditional probabilities in *yellow*. *Low* conditional probabilities in *blue*. 

Imagine that you are an undergraduate student working in this research lab. One day, the Principle Investigator (Dr. Carlson) asks you to run more repetitions of a new experiment they just tried. They are excited to collect more data and publish these results (Figure 4) because they think they found a huge effect of temperature on action sequencing during grooming. They hand you their preliminary results (Figure 4). You look at the results and immediately hand it back, telling them not to get too excited yet. ***You confidently tell Dr. Carlson that they have analyzed their data incorrectly***! 

:::{image} /images/conditional-probability-analysis_incorrect-example.png
:width: 700
:align: center
:::

**Figure 4**: The preliminary results that Dr. Carlon handed to you. Both tables show the conditional probabilities that Dr. Carlson calculated among grooming actions under two different temperature conditions. 

***Q10 (2 points): How did you know that Dr. Carlson did something wrong with their data analysis by looking only at their results tables (Figure 4)?***

***Q11 (3 points): In Figure 4, you also notice that Dr Carlson likely used (continuous / interval) sampling methods to collect their data rather than (continuous / interval) sampling methods. You suggest that they re-do their experiment using (continuous / interval) sampling.  
a) Choose one word from each parenthesis and re-write the provided sentence (replace "you" with "I").  
b) Explain how you could infer which sampling method they used.  
c) Explain why you think they should use a different method to test a hypothesis about action sequencing.***





<!-- Not used this time...

## Section X: Vigilance in Meerkats

Like you did in class, you will consider 'vigilant', 'not vigilant', and 'out of sight’ as the three behaviors comprising the ethogram for this study. Data should be collected for ONE meerkat at each distance of predator presentation (2 m, 6 m, 10 m, 14 m). 

***Q: This experiment was designed to test the effect of ______________ on _____________.*** 

### Continuous Focal Sampling 

Record the start time of each behaviour on a new line as shown:

| **Behavior** | **Start time** | **Duration** |
| --- | --- | --- |
| name of behavior | cummulative seconds | calculated | 


***Q: What behavioral metric (based on your continuous sampling data) do you propose to calculate to test if predator proximity influences the trade-off between vigilant and non vigilant behavior (activity budget)? Define any relevant mathematical equation(s) for your calculation(s).***

[This video](https://vimeo.com/77501205) is split into time windows according to the following table. 
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

For each time window, there was a predator at a different distance ('distance' column in the table). Watch and collect data for only the sections that correspond to predator distances of 14, 10, 6, and 2 meters.   

***Q: Plot your results.***

***Q: How is vigilance behavior being quantified using this sampling method?*** 

### Instantaneous Scan Sampling

Carry out the same experiment, but use an interval scan sampling method instead. For simplicity, collect data only for the following distances: 14, 10, 6, 2m). 

***Q: Create a figure to clearly report your results. Clearly describe your sampling protocol/method. Define any calculations that you did on the raw data.***

***Q: Plot your results.***

***Q: How is vigilance behavior being quantified using this sampling method?*** 


 -->