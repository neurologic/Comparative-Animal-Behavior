# Neural Mechanisms

<!-- <hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr> -->

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
| ion | internal concentration (mM) | external concentration (mM)| Equilibrium Potential (mV) |
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


***Q1: If the membrane is only permeable to K+ ions, what would be the voltage across the cell's membrane?***

***Q2: How can you change the membrane potential of a neuron?***


⏸️ PAUSE here for class-wide discussion

---
Membrane permeability is controlled by special proteins in the membrane called *ion channels*. Different ion channels are specific for the permeability of different ions. Some ion channels always let their ion through. Some ion channels are *gated by* voltage and only let their ion through when the membrane potential is above or below certain voltage levels. Some ion channels are *gated by* the binding of molecules to their surface. 

:::{figure} /images/ion-channel-cartoon-general.jpeg
:width: 600

A cartoon of an ion channel[^ion-chan-md]. Ion channels can be either closed (left) or open (right). 
:::

[^ion-chan-md]: Image from [molecular devices](https://www.moleculardevices.com/applications/ion-channels)

---
> ⏳ 5 min 

Examine the plots of membrane potential (V) aross time in Figure 20 and the terminology used to describe the changes in membrane potential.

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

A neuron is **activated** when it is depolarized above it's spike threshold (and therefore generates a spike). Spikes are a special type of "non-linear" voltage event. They are special because they cause synaptic events. 

:::{figure} /images/voltage-spike-plot.png
:width: 300

Plot of membrane potential (y-axis) across time (x-axis; left-to-right). The membrane potential starts at "rest", then depolarizes, then depolarizes so much that it reaches spike threshold (green dotted line), and a voltage spike is generated. This voltage spike would then go on to cause a synaptic event (see next section). 
:::


## Systems and Circuits and Behavior

### Synapses

:::{figure} /images/Neuron-Synapse.png
:width: 500

Synapses between neurons transform *electrical* events into *chemical* events and back to *electrical* events. Chemical signals are released by the pre-synaptic neuron membrane when a voltage spike (large depolarization) occurs. These bind to ion channels on the post-synaptic membrane. When the ion channles bind the chemical signal, they open and let their ion through the membrane (increasing its conductance).
:::

:::{figure} /images/ligand-gated-ion-channel.png
:width: 500

An example cartoon of a ligand-gated calcium ion channel[^lgic-wiki]. When the ligand (a molecule) binds to the receptor (the ion channel), it then lets its ions through. 
:::

[^lgic-wiki]: Image from [wiki](https://en.wikipedia.org/wiki/File:LGIC.png)

Neurons effect each other via synapses. There are neurons *before* (pre-synaptic) and neurons *after* (post-synaptic) synapses. Specifically:
1. Voltage spikes in a "pre"-synaptic neuron cause the release of molecules (neurotransmitters and/or neuromodulators). Different types of neurons have different neurotransmitters.
2. Synaptic events change ion permeability in a "post"-synaptic neuron. Receptors (membrane proteins)are permeable only to specific ions and only when they bind specific molecules. Different types of neurons have different receptors.

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


***Q5: Let neuron \#2 have a K+ to Na+ conductance ratio of 0.8 to 0.2, and no Cl- conductance. What would be the resting membrane potential of neuron #2?***

***Q6: To produce the result shown in A, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-?***

***Q7: To produce the result shown in B, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-?***

***Q8: What would happen to the membrane potential of neuron \#2 if it did not have any receptors that could detect the neurotransmitter released by neuron \#1?***


### Sensors

Sensors are special types of neurons that change their voltage in response to changes in physical energy in the environment. Physical energy can take the form of light, pressure, movement, etc. 

***Q1: Consider a sensor in the eye that depolarizes and spikes in response to an increase in light. This sensor provides excitatory synaptic input to a "post-synaptic" neuron in the brain. What happens to the membrane potential of the neuron in the brain when there is a flash of light onto the eye?***


⏸️ PAUSE here for class-wide discussion

---

If more light causes more spikes in the sensor, the post-synaptic depolarizations can sum together. In this case, more spikes in the sensor would mean more depolarization in the post-synaptic neuron. More depolarization in the post-synaptic neuron could then mean more spikes. The stronger the stimulus, the stronger the response (magnitude of membrane potential change). 


### Muscles

Muscles contract (shorten) when their membrane becomes depolarized. When muscles attach across two sides of a joint, the joint angle reduces when the muscle shortens. This is the foundation of all movement, and therefore of behavior. 

:::{figure} /images/motor-output.png
:width: 700

A) Motor neurons synapse onto muscles. B) Motor neurons vary their rate (frequency) of spike events. C) Muscle cells depolarize in response to motor neuron spike events. D) Muscle cells decrease in length when they are depolarized.    
::: 


### Circuits

When groups of neurons (each with special individual identities) connect with each other to form circuits, complex outputs can emerge. 

:::{figure-md} neural-circuits
:class: figure

<img src="/images/neural-circuits.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Two excitatory synapses in a row. If the first neuron depolarized and spiked, the second neuron would then depolarize soon after and may spike as well. If the first neuron hyperpolarized, it would not spike and the second neuron would just stay at its *resting* membrane potential (no change in its output).   
B) An excitatory synapse followed by an inhibitory synapse. If the first neuron depolarized and spiked, the second neuron would then hyperpolarize soon after.     
C) Convergence and divergence in heterogeneous neural circuits. 
:::


---
> ⏳ 10 min 


***Q2: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment increases.***

***Q3: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment decreases. The motor neuron must be excitatory (an increase in spike rate causes an increase in muscle potential). Hint: think about ways that you can effect the "resting" state of a neuron.***

⏸️ PAUSE here for class-wide discussion

---

Neuroscience seeks to understand how neural circuits orchestrate behavior. Neurons must respond to stimuli that contain information about the world. Neurons must encode that information and compute on it. Computations lead to decisions about what actions are needed in response. Internal factors can also influence action selection. Neurons must orchestrate actions by dynamically coordinating sets of muscles. 


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
