# Neural Mechanisms

[Day 1](neural_day1)
[Day 2](neural_day2)
<!-- <hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr> -->
(neural_day1)=
## Making Connections to the Past and Moving Forward

Introductory discussion based on Podcast. 

- FAPs
- Sequencing
- Hydraulic Pressure Model
- "Activation" (sign stimulus implied)
- "Circuits" versus brain areas
- Emotional state, "motivation", and behavior


## The Building Blocks 

### Cell types: neurons

:::{figure} /images/Neuron-Anatomy.png
:width: 800

Basic neuron anatomy. Neuron morphology is diverse (left), but follows a basic template of 'parts': axon, dendrite, cell body (right). Importantly, like other cells, neurons are enclosed by a barrier that controls permeability and movement of solutes across it.
:::

### Electrochemical Forces

The electrochemical force forms the basis of how the nervous system causes behavior. Changes in membrane voltage are used to *compute* and *transmit* information throughout the nervous system. 

:::{margin} Concentration Gradient
<img src="/images/concentration-gradient.png" alt="fishy" class="bg-primary mb-1" width="400px">
:::

Differences in atom concentration across a barrier result in a chemical force on atoms directed from areas of high concentration to low. 

:::{margin} Holes in barrier
<img src="/images/concentration-gradient-holes.png" alt="fishy" class="bg-primary mb-1" width="400px">
:::

If the barrier gets a hole in it, then the atoms will move due to the chemical force. 

If the atoms are charged (ie. *ions*), then an electric gradient will accumulate as the ions move in response to the chemical force. The electric gradient generates an electric force that builds up until the opposing chemical and electrical forces equal each other. The electrical force that balances the chemical force is called the **equilibrium potential** for that ion. 

:::{figure} /images/Electro-Chemical-Balance.png
:width: 800

The electrical force ($e$, green arrow) opposes the chemical force ($c$, yellow arrow) for an ion. When a membrane becomes permeable to an ion with a concentration force (A to B), the electrical force increases until it exactly opposes the (now reduced) chemical gradient (B). The result is a stable and measurable voltage (*potential*) across the membrane. 
:::

We measure the membrane potential of a neuron using a voltage meter. 
Neurons have a "*resting*" membrane potential (in the absence of any synaptic input). However, there are mechanisms for changing a neuron's relative conductance (permeability) of ions (which we will get to in a bit).

:::{figure-md} potential-meter-rest
:class: figure

<img src="/images/membrane-potential-rest-meter.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) neurons have a resting membrane potential. B) Voltage meters can measure the membrane potential. The voltage inside is referenced to the voltage outside. C) The resting membrane potential of neurons is usually negative inside relative to outside. 
:::

### Neuron membrane potential

In neurons, different ions have different concentration gradients across the membrane (and different charge). Therefore, the equilibrium potential for different ions is different. 

---
> ⏳ 5 min 

Consider the following table of values for K+, Na+, and Cl- across a neuron's membrane. From these concentrations, we can use a specific equation ([Nernst equation](https://en.wikipedia.org/wiki/Nernst_equation)) to calculate the membrane potential at which the electrical force opposes the chemical force on the ion[^nernst-calc]. We call this membrane potential the **equilibrium potential** for the ion. 

[^nernst-calc]: [Equilibrium Potential Calculator](https://www.physiologyweb.com/calculators/nernst_potential_calculator.html)

<a id="table1"></a>
| ion | internal <br> concentration (mM) | external <br> concentration (mM)| Equilibrium <br> Potential (mV) |
| :---: | :---: | :---: | :---: |
| Na+ | 15 | 145 | +61 |
| K+ | 150 | 4 | -97 |
| Cl- | 10 | 110 | -64 |

Consider the following table of relative ion permeability ("*conductance*", $g$) across a neuron's membrane and the total difference in electrical potential across that membrane.

<a id="table2"></a>
| $g_{Na+}$ | $g_{K+}$ | $g_{Cl-}$| membrane potential (mV) |
| :---: | :---: | :---: | :---: |
| 0.2 | 0.8 | 0 | 0.2\*(+61) + 0.8\*(-97) = **-65.4** |
| 0 | 0 | 1 | 1\*(-64) = **-64** |
| 0.8 | 0.2 | 0 | 0.8\*(+61) + 0.2\*(-97) = **+29** |


***Q1: If the membrane is only permeable to K+ ions, what would be the voltage across the cell's membrane (ie. the membrane potential)?***

***Q2: How can you change the membrane potential of a neuron?***


⏸️ PAUSE here for class-wide discussion

---
Membrane permeability is controlled by special proteins in the membrane called *ion channels*. Different ion channels are specific for the permeability of different ions. Also, different ion channels have different criteria for being "open" (ie. increasing the conductance for their ion).  
- Some ion channels always let their ion through. 
- Some ion channels are *gated by* voltage and only let their ion through when the membrane potential is above or below certain voltage levels. 
- Some ion channels are *gated by* the binding of molecules to their surface. 

:::{figure} /images/ion-channel-cartoon-general.jpeg
:width: 600

A cartoon of an ion channel[^ion-chan-md]. Ion channels can be either closed (left) or open (right). 
:::

[^ion-chan-md]: Image from [molecular devices](https://www.moleculardevices.com/applications/ion-channels)

---
> ⏳ 5 min 

Examine the plots of membrane potential (V) aross time in Figure 21 and the terminology used to describe the changes in membrane potential.

:::{figure} /images/depolarize-hyperpolarize.png
:width: 400

Grey: membrane potential (voltage)  
A) Red: depolarized. Blue: hyperpolarized.  
B) Red: depolarizing. Blue: hyperpolarizing.  
:::

***Q3: How would you define 'depolarized'?***

***Q4: How would you define 'depolarizing'?***

⏸️ PAUSE here for class-wide discussion

---

A neuron is **activated** when it is depolarized above it's spike threshold (and therefore generates a spike). Spikes are a special type of "non-linear" voltage event. They are special because they cause "*synaptic events*" (see next section). 

:::{figure} /images/voltage-spike-plot.png
:width: 300

Plot of membrane potential (y-axis) across time (x-axis; left-to-right). The membrane potential starts at "rest", then depolarizes, then depolarizes so much that it reaches spike threshold (green dotted line), and a voltage spike is generated. This voltage spike would then go on to cause a synaptic event (see next section). 
:::


## Systems and Circuits and Behavior

### Synapses

:::{figure} /images/Neuron-Synapse.png
:width: 600

Synapses between neurons transform *electrical* events into *chemical* events and back to *electrical* events. Chemical signals are released by the pre-synaptic neuron membrane when a voltage spike ("electrical signal"; large depolarization) occurs. These bind to ion channels on the post-synaptic membrane. When the ion channels bind the chemical signal, they open and let their ion through the membrane (increasing its conductance).
:::

:::{figure} /images/ligand-gated-ion-channel.png
:width: 500

An example cartoon of a ligand-gated calcium ion channel[^lgic-wiki]. When the ligand (a molecule) binds to the receptor (the ion channel), it then lets its ions through. 
:::

[^lgic-wiki]: Image from [wiki](https://en.wikipedia.org/wiki/File:LGIC.png)

Neurons effect each other via synapses. There are neurons *before* (pre-synaptic) and neurons *after* (post-synaptic) synapses. Specifically:
1. Voltage spikes in a "pre"-synaptic neuron cause the release of molecules (neurotransmitters and/or neuromodulators). Different types of neurons have different neurotransmitters.
2. Synaptic events change ion permeability in a "post"-synaptic neuron. Receptors (membrane proteins) are permeable only to specific ions and only when they bind specific molecules. Different types of neurons have different receptors.

For a neurotransmitter to change ion permeability of a neuron, the neuron must have receptors for the neurotransmitter. Two broad types of neurotransmitter-receptor pairs are *excitatory* and *inhibitory*. 

---
> ⏳ 15 min 

:::{margin} Table 1: Ion equilibrium potential.
| ion | Equilibrium <br> Potential (mV) |
| :---: | :---: |
| Na+ | +61 |
| K+ | -97 |
| Cl- | -64 |
:::

:::{margin} Table 2: Conductances and membrane potential.
| $g_{Na+}$ | $g_{K+}$ | $g_{Cl-}$| membrane potential (mV) |
| :---: | :---: | :---: | :---: |
| 0.2 | 0.8 | 0 | 0.2\*(+61) + 0.8\*(-97) = **-65.4** |
| 0 | 0 | 1 | 1\*(-64) = **-64** |
| 0.8 | 0.2 | 0 | 0.8\*(+61) + 0.2\*(-97) = **+29** |
:::

:::{figure} /images/synaptic-potential.png
:width: 700

Example synaptic connectivity and the result on post-synaptic membrane potential. A) Excitatory synaptic connection. Ai) Depolarization above a specific value causes a brief voltage *spike* event. B) Inhibitory synaptic connection.  
::: 

Consider the K+, Na+, and Cl- equilibrium potentials established in [table 1 and 2](#table1) (shown in the margin to the right). 


***Q5: Let neuron \#2 have a "resting" K+ to Na+ conductance ratio of 0.8 to 0.2, and no Cl- conductance. What would be the "resting" membrane potential of neuron #2?***

***Q6: To produce the result shown in A, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-? Why?***

***Q7: To produce the result shown in B, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-? Why?***

***Q8: What would happen to the membrane potential of neuron \#2 if it did not have any receptors that could detect the neurotransmitter released by neuron \#1?***


⏹️ STOP here for today

---

(neural_day2)=
### Muscles

Muscles contract (shorten) when their membrane becomes depolarized. When muscles attach across two sides of a joint, the joint angle reduces when the muscle shortens. This is the foundation of all movement, and therefore of behavior. 

:::{figure} /images/motor-output.png
:width: 700

A) Motor neurons synapse onto muscles. B) Motor neurons vary their rate (frequency) of spike events. C) Muscle cell membrane potential depolarizes in response to motor neuron spike events. More spikes = more depolarization D) Muscle cells decrease in length when they are depolarized.    
::: 

### Sensors

::::{margin} Transduction cascade uses photon absorption to change ion permeability.
:::{image} /images/rhodopsin-conductance-activation.png
:::
::::

Sensors are special types of neurons that change their membrane potential in response to changes in physical energy in the environment. Physical energy can take the form of light, pressure, movement, etc. 

Let's consider a sensor that hyperpolarizes in response to an increase in light (example mechanism in the margin figure) and depolarizes in response to an increase in light. The hyperpolarization decreases its synaptic release of molecules (*neurotransmitters*). This sensor provides inhibitory synaptic input to a "post-synaptic" neuron. 

:::{figure} /images/sensor-circuit.png
:width: 600

**A)** A sensor neuron (SN) that hyperpolarizes in response to light synapses onto a post-synaptic neuron (PN). The synapse is inhibitory for the PN. **B)** Synaptic release from the sensor is proportional to its membrane potential. **C)** Example changes in membrane potential for the SN and PN in response to a change in the light stimulus over time. 
:::

***Q1: What happens to the membrane potential of the post-synaptic neuron when there is a flash of light onto the sensor?***


### Circuits

When groups of neurons connect with each other via inhibitory or excitatory synapses to form circuits, complex outputs can emerge. 

:::{figure-md} neural-circuits
:class: figure

<img src="/images/neural-circuits.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Two excitatory synapses in a row. If the first neuron depolarized and spiked, the second neuron would then depolarize soon after and may spike as well. If the first neuron hyperpolarized, it would not spike and the second neuron would just stay at its *resting* membrane potential (no change in its output).   
B) An excitatory synapse followed by an inhibitory synapse. If the first neuron depolarized and spiked, the second neuron would then hyperpolarize soon after.     
C) Convergence and divergence in heterogeneous neural circuits. 
:::


---
> ⏳ 5 min 

***Q2: Draw a neural circuit composed of an auditory sensor neuron, a motor neuron and a muscle. The sensor neuron is depolarized by sudden increases in the amplitude of sound. The circuit should contract the muscle when the sound amplitude in the environment suddenly increases.***

***Q3: Draw a neural circuit composed of the same three neurons as in Q2. The circuit should contract the muscle when the sound amplitude in the environment suddenly decreases. Hint: you can make any neuron have a "resting" membrane potential above spike threshold (so that it is spiking in the absense of synaptic input).***

⏸️ PAUSE here for class-wide discussion

---

## Behavior

Neuroscience seeks to understand how neural circuits orchestrate behavior. In general, this involves examining all of the following processes:
1. Sensors must respond to stimuli that contain information about the world. 
2. Neurons must use that information and compute with it. 
3. Computations lead to decisions about what actions are needed in response. 
4. Internal factors can also influence action selection. 
5. Neurons then orchestrate actions by dynamically coordinating sets of muscles. 

### Case Study: Cricket Acoustic Communication

:::{figure} /images/crickets-singing-behavior.png
:width: 600

Acoustic behavior of *Gryllus campestris*[^hedwig-2006].  A male sings in front of its burrow by rubbing the elevated front wings together. The calling song consists of single sound pulses (syllables) grouped
into chirps. Attracted by the calling song a female performs phonotaxis and walks towards the singing male using acoustic cues for orientation. 
:::

[^hedwig-2006]: Figure from [Hediwg (2006) Pulses, patterns and paths: neurobiology of acoustic behaviour in crickets. J Comp Physiol A](https://doi.org/10.1007/s00359-006-0115-8). Modified after Roesel von Rosenhof (1749).

<iframe width="560" align="center" height="315" src="https://www.youtube.com/embed/CQFEY9RIRJA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Command versus Pattern

Stereotyped motor patterns (for example, FAPs) are orchestrated by neural circuits that pattern the contraction among sets of muscles. These circuits need to be activated by a ***command*** signal. But, remarkably, the command signal itself (the spiking output of a neuron) does not need to be patterned. 

:::{figure} /images/cricket-singing-command-neuron.png
:width: 700

Command neuron controlling calling song[^hedwig-2006]. Neuron: A recording of the command neuron's membrane potential across time in the brain of Gryllus bimaculatus. Increasing the neurons spike activity (AP/s) elicits the generation of calling song (Sound): the cricket lifts its wings and starts to sing (Forewing).
:::

The **command neuron** causes the cricket to sing, but its activity is unpatterned. What causes the patterning of the movement required to produce the patterned song?

:::{glossary} 
central pattern generator (CPG)
  A neural circuit that can produce patterned output in the absence of patterned input. In other words, it is a circuit that is self-sufficient at producing a stereotyped pattern of spikes that regularly changes over time.
:::

:::{figure} /images/cricket-cpg-diagram.png
:width: 800

**A)** The anatomy of a chirp. The cricket's wings have a file and a scraper. When the cricket closes both of its wings together, the scraper rubs the file and vibrates the wings, producing sound. **B)** The pattern of activity among wing opener and closer muscles, wing movement (open and closed), and sound. **C)** A central pattern generator for wing movement that is comprised of motor neurons (MN) that synapse on wing opener and closer muscles and interneurons (IN). The INs provide excitatory input to MNs. MNs provide excitator input to muscles (thus contracting them). INs are also provide synaptic input to each other. 
::: 

***Q4: The synaptic input from each IN to the other was left undefined in C. Do these need to be excitatory or inhibitory synapses? Why?***

::::{margin} 
:::{image} /images/cricket-hemisection.png
:::
::::

:::{figure} /images/cricket-cpg-bilateral-coordination.png
:width: 400

The entire CPG circuit in Figure 31 can be represented by a circle with a tilde symbol. Often, multiple CPGs need to be coordinated with each other. There is a wing CPG on each side of the animal's body. A command neuron can excite the CPG circuits with unpatterned input. 
:::

***Q5: The CPGs for wing movement on each side of the cricket's body need to be coordinated with each other. What synaptic connection is needed from each CPG to the other?***

:::{index} sensory filter
:::

#### Sensory Filtering

Not all sensory stimuli are the same. Stimuli have lots of different ***features***. In the case of cricket song, we will consider two features: the *syllable period* (SP) and the loudness (amplitude). Both of these features can vary across a wide range. 

***Sensory filtering*** results from the stimulus specificity of sensors. Sensors only respond to specific types of physical energy in the world (light, sound, odor) - we refer to these as *modalities*. Then within each modality, different sensors respond best to specific features of a stimulus (frequency of sound, wavelength of light). Each stimulus feature can vary along a continuum, and sensors are even specific to a range of feature values (500 nanometer light, 200 Hz sound). 

Withouth sensory filtering, there would be no specificity in behavioral responses to stimuli.   

Female crickets move toward male cricket song. We call this *phonotaxis* and it is an FAP. It would not be adaptive for female crickets to phonotax in response to all sound, so there are sensory filters in their nervous system that are more *sensitive to* the song of a male cricket than to anything else. Different species of crickets have songs with different *syllable period*. The sensory filters are most *sensitive to* conspecific song. 

So what does *sensitive to* mean?  

:::{figure} /images/crickets-phonotaxis-sensory-filter.png
:width: 800

Sensory filtering for species-specific song[^hedwig-2006]. **A**) Trackball system for analysing cricket phonotaxis. [See also this video of the behavior](https://youtu.be/oVL82zuPbLU) **B**) Sound patterns to test sensory tuning for conspecific song. **C**) Tuning curve of phonotaxis demonstrates the strongest response to SP34–SP42, which corresponds to the natural range of SP. Phonotaxis declined at shorter or longer syllable periods.
:::

So, at a basic level, what is a neural mechaism of phonotaxis? Sensory stimuli are transformed into changes in neuron membrane potential by sensors. Sensors then synapse onto *decision* centers in the brain, which trigger specific FAPs. If a certain threshold is reached by a sensory filter, then the FAP will be triggered.  
The flow of information is: sensory stimuli --> sensory filter --> decision --> FAP. 

:::{figure} /images/cricket-sensory-filtering.png
:width: 600
:align: center

Both the amplitude and the SP of song effect the membrane potential of a sensory filter. 
:::

***Q6: The song amplitude needed to evoke an FAP is most closely related to the:  
a. sensory threshold in Lorenz's model  
b. behavioral threshold in Lorenz's model   
c. the action specific potential in Lorenz's model***

***Q7: The data shown in Fig 35 are from an experiment measuring the membrane potential response of sensory filter neurons to song. Songs with two different SP levels were tested. Which color corresponds to 38 SP and which color corresponds to 60 SP?***

:::{figure} /images/sensory-filtering-amplitude-vm.png
:width: 600
:align: center

The membrane potential response (y-axis) to stimuli of different amplitudes (x-axis) and SP values (color). If the sensory filter spike threshold is reached, an FAP is produced in response. 
:::


### Case Study: Aggression in Mice

Aggression is a social behavior essential for securing resources and defending oneself and family. Many animals have aggressive FAPs. Across animals, we find that the release of FAPs depends, not just on the presence of external *sign stimuli*, but on the internal state of the animal. 

:::{image} /images/aggression-summary-factors.png
:width: 800
:::

"Regions of the brain in the core aggression circuit are more specialized for aggression: activating any of those regions evokes attack, often in a time-locked manner, while inactivating any of those regions impairs or even abolishes natural aggression. The fact that aggression can be triggered as well as blocked from each of those regions supports the idea that these regions form one integrated circuit. 

The ventrolateral nucleus of the ventromedial hypothalamus (VMHvl) is perhaps the best studied region for aggression in recent years, with the vast majority of the studies done in mice. Electrical stimulation or pharmacological manipulation in the VMHvl can elicit aggression in cats, chickens, opossums and monkeys. In male and female mice, optogenetic activation of VMHvl cells, especially those expressing estrogen receptor alpha (Esr1), elicited time-locked attack toward both natural (other mice) and suboptimal targets (gloves filled with water or air; or socially inappropriate attacks at conspecifics). Upon male-intruder introduction, VMHvl cells show an elevation in baseline activity, which is sustained throughout the duration of the intruder’s presence and minutes after removal of the intruder. During male–male investigation and attack, VMHvl activity increases further, and then returns to the elevated baseline at the offset of the behavioral episode. Thus, the VMHvl cells appear to carry information regarding aggressive arousal state, aggression-provoking sensory cues and the motor execution of
attacks."[^dayu-review]

[^dayu-review]: [Lischinsky, J.E., Lin, D. Neural mechanisms of aggression across species. Nat Neurosci 23, 1317–1328 (2020).](https://doi.org/10.1038/s41593-020-00715-2)

:::{figure} /images/aggression-neuroanatomical-mouse.png
:width: 800

Neuroanatomical pathways for aggression in mice. Yellow indicates regions for processing sensory inputs; orange indicates regions belonging to core aggression circuit (CAC); red indicates regions relevant for motor output; purple indicates regions for top-down control and lilac indicates regions where dopamine neurons reside. AOB, accessory olfactory bulb; MOB, main olfactory bulb; CoAp, posterior cortical amygdala nucleus; Hyp, hypothalamus; MPOA, medial preoptic area; Hip, hippocampus; Str, striatum. From [Neural mechanisms of aggression across species](https://doi.org/10.1038/s41593-020-00715-2), a by Julieta E. Lischinsky and Dayu Lin (2020).
:::

:::{figure} /images/5HT-1B_receptor-signalling.png
:width: 500

Serotonin receptor mechanism of action on neuron membrane conductance
:::

:::{figure} /images/aggression-circuit-mice-ala-Lorenz.png
:width: 700

A Lorenz model of behavior for a male mouse defending its territory. Top: action-specific potential across time (black). Middle: the time during which external or internal stimuli (orange, green and blue) were present. Bottom: time of attack FAPs. 
:::

***Q8: Which color most likely corresponds to the presence of a dominant (threatening) intruder? In terms of the data in the top figure, what is your evidence for this?***

***Q9: Which color most likely corresponds to the presence of a submissive (non-threatening) intruder? In terms of the data in the top figure, what is your evidence for this?***

***Q10: Which color most likely corresponds to the presence of serotonin in the animals? In terms of the data in the top figure, what is your evidence for this?***

***Q11: The action-specific potential most closely models the membrane potential of:  
a. sensory neurons in the olfactory bulb  
b. VMHvl neurons  
c. neurons in the motor output circuits  
Why did you select the choice you made versus the other options?***

## Additional Resources
- [BI 054 Kanaka Rajan: How Do We Switch Behaviors?](https://braininspired.co/podcast/54/)
- [Huberman Lab: UNDERSTANDING & CONTROLLING AGGRESSION](https://hubermanlab.com/understanding-and-controlling-aggression/)
- [Basic NeuroAnatomy](https://learn.genetics.utah.edu/content/neuroscience/neurons)
- [Ronacher, B. Innate releasing mechanisms and fixed action patterns: basic ethological concepts as drivers for neuroethological studies on acoustic communication in Orthoptera. J Comp Physiol A 205, 33–50 (2019).](https://doi.org/10.1007/s00359-018-01311-3). This paper provides a framework for linking fundamental course concepts discussed so far
- [The Neural Control of Movement (2020) FULL BOOK. Edited by: Patrick J. Whelan and Simon A. Sharples](https://doi.org/10.1016/C2018-0-00499-5)
- ::::{dropdown} Review of atoms versus ions
  :::{image} /images/Sodium-Atom-Ion.png
  :width: 600
  :::
  A simplefied schematic of a sodium (Na) atom and a sodium ion (Na+). Based on the simplified schematic in Fig. 1, what are the two fundamental differences between an atom and an ion? What does the "+" stand for in Na+?
  ::::
- [Retinal Circuits sensing light](https://openbooks.lib.msu.edu/neuroscience/chapter/vision-the-retina/)
- [Stridulation after hemisection](https://link.springer.com/content/pdf/10.1007/BF00616745.pdf)
- [Pedro F. Jacob and Berthold Hedwig (2019) Structure, Activity and Function of a Singing CPG Interneuron Controlling Cricket Species-Specific Acoustic Signaling. Journal of Neuroscience, 39 (1) 96-111](https://doi.org/10.1523/JNEUROSCI.1109-18.2018)
- [Lischinsky, J.E., Lin, D. Neural mechanisms of aggression across species. Nat Neurosci 23, 1317–1328 (2020).](https://doi.org/10.1038/s41593-020-00715-2)
- :::{figure} /images/predatory-hunting-CeA-graphical-abstract.jpeg
    :width: 400

    From [Han et al 2019 Integrated Control of Predatory Hunting by the Central Nucleus of the Amygdala](https://doi.org/10.1016/j.cell.2016.12.027)
    :::
