# Neural Mechanisms

<!-- <hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr> -->

## Making Connections to the Past and Moving Forward

Introductory discussion based on Podcast. 

- FAPs
- Hydraulic Pressure Model
- Neural circuits versus areas


## The Building Blocks 

### Cell types: neurons

:::{figure} /images/Neuron-Anatomy.png
:width: 800

Basic neuron anatomy. Neuron morphology is diverse (left), but follows a basic template of 'parts': axon, dendrite, cell body (right). Importantly, like other cells, neurons are enclosed by a barrier that controls permeability and movement of solutes across it.
:::

### Electrochemical Forces

The electrochemical gradient forms the basis of how the nervous system causes behavior. Changes in membrane voltage are used to compute and transmit information throughout the nervous system. 

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

The electrical gradient ($e$), which opposes the chemical gradient ($c$) for an ion, sets up a measurable voltage (*potential*) across a barrier that is permeable to that ion. The electrical gradient increases until it exactly opposes the (now reduced) chemical gradient.
:::


### Neuron membrane potential

In neurons, different ions have different concentration gradients across the membrane (and different charge). Therefore, the equilibrium potential for different ions is different. 

---
> ⏳ 10 min 

Consider the following table of values for K+ and Na+ across a neuron's membrane.[^nernst-calc]

[^nernst-calc]: [Equilibrium Potential Calculator](https://www.physiologyweb.com/calculators/nernst_potential_calculator.html)

<a id="table1"></a>
| ion | internal concentration (mM) | external concentration (mM)| Equilibrium Potential (mV) |
| :---: | :---: | :---: | :---: |
| Na+ | 15 | 145 | +61 |
| K+ | 150 | 4 | -97 |
| Cl- | 10 | 110 | -64 |

Consider the following table of relative ion permeability (*conductance*, $g$) across a neuron's membrane and the total difference in electrical potential across that membrane.

<a id="table2"></a>
| $g_{Na+}$ | $g_{K+}$ | $g_{Cl-}$| membrane potential (mV) |
| :---: | :---: | :---: | :---: |
| 0.2 | 0.8 | 0 | 0.2\*(61) + 0.8\*(-97) = **-65.4** |
| 0 | 0 | 1 | 1\*(-64) = **-64** |
| 0.8 | 0.2 | 0 | 48.4 19.4 = **+29** |


***Q1: If the membrane is only permeable to K+ ions, what would be the voltage across the cell's membrane?***

***Q2: How can you change the membrane potential of a neuron?***


⏸️ PAUSE here for class-wide discussion

---

We measure the membrane potential of a neuron using a voltage meter. 
Neurons have a "*resting*" membrane potential (in the absence of any synaptic input). However, there are mechanisms for changing a neuron's relative conductance (permeability) of ions (which we will get to in a bit).

:::{figure-md} potential-meter-rest
:class: figure

<img src="/images/membrane-potential-rest-meter.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) neurons have a resting membrane potential. B) Voltage meters can measure the membrane potential. The voltage inside is referenced to the voltage outside. C) The resting membrane potential of neurons is usually negative inside relative to outside. 
:::

---
> ⏳ 5 min 

:::{figure-md} depolarize-hyperpolarize
:class: figure

<img src="/images/depolarize-hyperpolarize.png" alt="fishy" class="bg-primary mb-1" width="500px">

Grey: membrane potential (voltage) 
A) Red: depolarized. Blue: hyperpolarized.  
B) Red: depolarizing. Blue: hyperpolarizing.  
:::

***Q3: How would you define 'depolarized'?***

***Q4: How would you define 'depolarizing'?***

⏸️ PAUSE here for class-wide discussion

---

## Systems and Circuits and Behavior

### Synapses

:::{figure} /images/Neuron-Synapse.png
:width: 500

Synapses between neurons transform *electrical* events into *chemical* events and back to *electrical* events. 
:::

Neurons effect each other via synapses. Voltage spikes cause synaptic events. Synaptic events change ion permeability. 

Synaptic events involve both *neurotransmitter* release from one neuron and *neurotransmitter receptors* on another neuron. Receptors are proteins that come in many types, and the function of each type is very specific. Each type of receptor detects the presence of specific neurotransmitters (and/or hormones). Each type of receptor is permeable only to specific ions. Different types of neurons have different receptors and neurotransmitters. In order for a neurotransmitter to cause a change in ion permeability of a neuron, the neuron must have receptors for the neurotransmitter. Two broad types of neurotransmitter-receptor pairs are *excitatory* and *inhibitory*. 

:::{figure-md} synaptic-potential
:class: figure

<img src="/images/synaptic-potential.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Excitatory synaptic connection. Ai) Depolarization above a specific value causes a brief voltage *spike* event. B) Inhibitory synaptic connection.  
::: 

---
> ⏳ 15 min 

Consider the K+, Na+, and Cl- equilibrium potentials established in [table 1](#table1). 

***Q5: Let neuron \#2 have a K+ to Na+ conductance ratio of 0.8 to 0.2, and no Cl- conductance. What would be the resting membrane potential of neuron #2?***

***Q6: To produce the result shown in A, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-?***

***Q7: To produce the result shown in B, would you predict that neuron \#2 had neurotransmitter receptors that were permeable to K+, Na+, or Cl-?***

***Q8: What would happen to the membrane potential of neuron \#2 if it did not have any receptors that could detect the neurotransmitter released by neuron \#1?***


### Sensors

Sensors are special types of neurons that change their voltage in response to changes in physical energy in the environment. Physical energy can take the form of light, pressure, movement, etc. 

***Q9: Consider a sensor in the eye that depolarizes and spikes in response to an increase in light. This sensor provides excitatory synaptic input to a "post-synaptic" neuron in the brain. What happens to the membrane potential of the neuron in the brain when there is a flash of light onto the eye?***


⏸️ PAUSE here for class-wide discussion

---

If more light causes more spikes in the sensor, the post-synaptic depolarizations can sum together. In this case, more spikes in the sensor would mean more depolarization in the post-synaptic neuron. More depolarization in the post-synaptic neuron could then mean more spikes. The brain therefore "knows" how much light there is in the eye based on the depolarization (and spiking) of the post-synaptic neuron. In other words, a neural code for light intensity is spike number and depolarization. 


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


***Q10: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment increases.***

***Q11: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment decreases. The motor neuron must be excitatory (an increase in spike rate causes an increase in muscle potential).***

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
