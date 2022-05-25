# Neural Mechanisms

<hr>

> {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

<hr>

## Electrochemical Forces

:::{index} ion, charge, voltage
:::

:::{figure-md} sodium-atom-ion
:class: figure

<img src="/images/Sodium-Atom-Ion.png" alt="fishy" class="bg-primary mb-1" width="500px">

A simplefied schematic of a sodium (Na) atom and a sodium ion (Na+). 
:::

***Q: Based on the simplified schematic in Fig. 1, what are the two fundamental differences between an atom and an ion?***

***Q: WHat does the "+" stand for in Na+?***

:::{margin} Concentration Gradient
<img src="/images/concentration-gradient.png" alt="fishy" class="bg-primary mb-1" width="400px">
:::

Differences in atom concentration across a barrier result in a chemical force on atoms directed from areas of high concentration to low. 

:::{margin} Holes in barrier
<img src="/images/concentration-gradient-holes.png" alt="fishy" class="bg-primary mb-1" width="400px">
:::

If the barrier gets a hole in it, then the atoms will move due to the chemical force. 

If the atoms are charged (ie. *ions*), then an electric gradient will accumulate as the ions move in response to the chemical force. The electric gradient generates an electric forse that builds up until the opposing chemical and electrical forces equal each other. The electrical force that balances the chemical force is called the *equilibrium potential* for that ion. 

:::{figure-md} electrochemical-balance
:class: figure

<img src="/images/Electro-Chemical-Balance.png" alt="fishy" class="bg-primary mb-1" width="500px">

The electrical gradient (which opposes the chemical gradient for an ion), sets up a measurable voltage (*potential*) across a barrier that is permeable to that ion.
:::

The electrochemical gradient forms the basis of how the nervous system causes behavior. Changes in membrane voltage are used to compute and transmit information throughout the nervous system. 


## Neuron membrane potential

In neurons, different ions have different concentration gradients across the membrane (and different charge). Therefore, the equilibrium potential for different ions is different. 

Consider the following table of values for K+ and Na+ across a neuron's membrane.

<a id="table1"></a>
| ion | internal concentration (mM) | external concentration (mM)| Equilibrium Potential (mV) |
| :---: | :---: | :---: | :---: |
| Na+ | 15 | 145 | +61 |
| K+ | 150 | 4 | -97 |

***Q: If the membrane is only permeable to K+ ions, what would be the voltage across the cell's membrane?***

***Q: If the membrane is only permeable to Na+ ions, what would be the voltage across the cell's membrane?***

***Q: If the membrane is equally permeable to BOTH K+ and Na+ ions, what would be the voltage across the cell's membrane?***

***Q: How can you change the membrane potential of a neuron?***

We measure the membrane potential of a neuron using a voltage meter. 
Neurons have a "resting" membrane potential (in the absence of any synaptic input) and synaptic input can *depolarize* or *hyperpolarize* the membrane potential elative to that resting state. 

:::{figure-md} potential-meter-rest
:class: figure

<img src="/images/membrane-potential-rest-meter.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) neurons have a resting membrane potential. B) Voltage meters can measure the membrane potential. C) The resting membrane potential of neurons is usually negative inside relative to outside. 
:::

:::{figure-md} depolarize-hyperpolarize
:class: figure

<img src="/images/depolarize-hyperpolarize.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Red: depolarized. Blue: hyperpolarized.  
B) Red: depolarizing. Blue: hyperpolarizing.  
:::


## Synapses

Neurons effect each other via synapses. Voltage spikes cause synaptic events. Synaptic events change ion permeability. 

Synaptic events involve both neurotransmitter release from one neuron and neurotransmitter receptors on another neuron. Receptors are proteins that come in many types, and the function of each type is very specific. Each type of receptor detects the presence of specific neurotransmitters (and/or hormones). Each type of receptor is permeable only to specific ions. Different types of neurons have different receptors and neurotransmitters. Two broad types of neurons are *excitatory* and *inhibitory*. 

:::{figure-md} synaptic-potential
:class: figure

<img src="/images/synaptic-potential.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Excitatory synaptic connection. Ai) Depolarization above a specific value causes a brief voltage *spike* event. B) Inhibitory synaptic connection.  
::: 

Consider the K+ and Na+ equilibrium potentials established in [table1](#table1). Let neuron 2 have an equal ratio of (small) permeability to K+ and Na+.

***Q: What would be the resting membrane potential of neuron #2?***

***Q: To produce the result shown in A, would neuron #2 have neurotransmitter receptors that were permeable to K+ or Na+?***

***Q: To produce the result shown in B, would neuron #2 have neurotransmitter receptors that are permeable to K+ or Na+?***

***Q: What would happen to the membrane potential of neuron #2 if it did not have any receptors that could detect the neurotransmitter released by neuron #1?***


## Sensors

Sensors are special types of neurons that change their voltage in response to changes in physical energy in the environment. Physical energy can take the form of light, pressure, movement, etc. 

***Q: Consider a sensor in the eye that depolarizes and spikes in response to an increase in light. This sensory provides excitatory synaptic input to a neuron in the brain. What happens to the membrane potential of the neuron in the brain when there is a flash of light onto the eye?***

***Q: If more light causes more spikes in the sensor, what will happen to the membrane potential of the neuron in the brain when there is more light?***

***Q: How does the brain "know" how much light there is in the eye? (In other words, what is the neural code for light intensity?)***

## Muscles

Muscles conctract when their membrane becomes depolarized. When muscles attach across two sides of a joint, the joint angle reduces when the muscle shortens. This is the foundation of all movement, and therefore of behavior. 

:::{figure-md} motor-output
:class: figure

<img src="/images/motor-output.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Motor neurons synapse onto muscles. B) Motor neurons vary their rate (frequency) of spike events. C) Muscle cells depolarize in response to motor neuron spike events. D) Muscle cells decrease in length when they are depolarized.    
::: 

***Q: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment increases. ***

***Q: Draw a neural circuit composed of a light sensor neuron, a motor neuron and a muscle. The circuit should contract the muscle when light in the environment decreases. The motor neuron must be excitatory (an increase in spike rate causes an increase in muscle potential).***

## Circuits

When groups of neurons (each with special individual identities) connect with each other to form circuits, complex outputs can emerge. 

:::{figure-md} neural-circuits
:class: figure

<img src="/images/neural-circuits.png" alt="fishy" class="bg-primary mb-1" width="500px">

A) Two excitatory synapses in a row  
B) An excitatory synapse followed by an inhibitory synapse  
C) Convergence and divergence in heterogeneous neural circuits. 
:::

Neuroscience seeks to understand how neural circuits orchestrate behavior. Neurons must respond to stimuli that contain information about the world. Neurons must encode that information and compute on it. Computations lead to decisions about what actions are needed in response. Internal factors can also influence action selection. Neurons must orchestrate actions by dynamically coordinating sets of muscles. 

