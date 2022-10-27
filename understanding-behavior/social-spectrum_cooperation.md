# Grouping and Cooperation


## The effect of group size on vigilance

Record the following:

Flock size
The number of times they are in the ‘head up’ position
The start and stop time of each ‘head up’ position.
I recommend using a stopwatch for this. Here is a link to the video (https://www.youtube.com/watch?v=oeJHW5n-PXY):

Calculate the total number of ‘head up’ behaviors and the total duration of ‘head up’ for each flock size and enter into the following data sheet. Then share with your partner.

## Dilution versus confusion

mayflies... number versus death rate
targetting prey and ability to track 

## Mobbing

kittyhawk gulls versus cliff nesting - phylogeny

## Genetic Switch Case Study: Locusts

## Grouping versus Cooperation

Is there a difference?

## Migration

### Case Study: Pelicans and Ibis

:::{figure-md} migration-formation-ibises
:class: figure

<img src="/images/migration-formation-ibises.jpg" alt="fishy" width="500px">

Catching air. Northern bald ibises (Geronticus eremita) migrate in the perfect formation to take advantage of updrafts. MARKUS UNSÖLD (WALDRAPPTEAM).[^science-media-vformation]
:::

[^science-media-vformation]: [Why Birds Fly in a V Formation: Study in ibises suggests the animals are giving each other a lift (2014)]https://www.science.org/content/article/why-birds-fly-v-formation#

Why migrate in groups?
- Dilution hypothesis (reduced risk of predation by being in group)?
- avoid getting separated?
- selfish herd (reduce risk of predation by putting other individuals between you and predator)?
- leader is better at finding the way?
- reduced energy? (but only for the followers?)

<iframe width="560" height="315" src="https://www.youtube.com/embed/SKXUJx2tCdI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

:::{figure-md} migration-pelican
:class: figure

<img src="/images/migration-pelican.png" alt="fishy" width="400px">

Wing-beat frequency and heart rate of pelicans engaged
in various types of flight (mean51 s.d.). Birds flying over a river
following a motor boat cruising at a constant speed of 48 km h11
flew at an average altitude of 1 m above the water, initially alone
at a distance from the boat (‘alone at 1 m’), but then joining other
birds in formation (‘in formation’). Numbering of circles indicates
the position in the formation, ‘1’ being the leader. In formation
flights, only birds in or behind the third position were used to
measure heart rate, to avoid the possible effects of motor-boat
turbulence on flight pattern. Wing-beat frequency of the lead and
second birds was measured in groups flying far from the boat.
Birds flying with an ultralight aeroplane cruising at 55–60 km h11
at an altitude of about 50 m were not able or willing to fly in the
wake of the aircraft, and generally flew at a distance, using a
flapping flight, at a speed of 45–50 km h11 (‘alone at 50 m’).
Pelicans following the plane finished their flight of 3 km with a
glide of 2–3 min (‘gliding’) before landing on the water. Heart
rates averaged 77.6515.2 beats per min (b.p.m.) when resting,
and reached 198.2518.7 and 204.9515.7 b.p.m. when
paddling in water and when walking, respectively.[^Weimerskirch-2001]
:::

## The evolutionary problem with cooperation

## green beard

[Simulating the green beard effect](https://youtu.be/goePYJ74Ydg)


## Collective Defense

### Reading
- Meerkat vigilance 
- Barnacle geese [group size vigilance video](https://www.youtube.com/watch?v=oeJHW5n-PXY)

	In your notebook document the following:

	- Flock size
	- The number of times they are in the ‘head up’ position
	- The start and stop time of each ‘head up’ position.

- [vigilance behavior lab](https://bookdown.org/djc426/behaviouR-R-package-tutorials/field-lab-4-vigilance-behavior.html)


<hr>

Do you think meerkats will be more or less vigilant in the presence of predators? Will their behavior vary depending on the type of predator?

Videos for Meerkat analysis
- [No Predator](https://vimeo.com/80600822)
- [Simulated Aerial Predator](https://vimeo.com/80600821)
- [Simulated Terrestrial Predator](https://vimeo.com/71877438)

Set a timer to go off every 10 seconds, and at each interval record the number of meerkats performing each behavior. We will use a modified ethogram that includes only three categories: vigilant, not vigilant or out of site.

Vigilant: Head raised at or above horizontal plain and eyes open (to include scanning /guarding / raised guarding). Not Vigilant: Eyes closed or head lower than horizontal plane (to include foraging, moving, sleeping, resting). Out of sight: Not visible by the researcher


 
## Additional Resources
- [Neuroscience: A social hub for worms](https://doi.org/10.1038/4581124a)
- [Cooperation](http://pages.nbb.cornell.edu/Gamebug/cooperation.html)
- [V-formation flight commentary](https://www.science.org/content/article/why-birds-fly-v-formation)
- Weimerskirch, H., Martin, J., Clerquin, Y. et al. [Energy saving in flight formation](https://doi.org/10.1038/35099670). Nature 413, 697–698 (2001).
- Portugal, S., Hubel, T., Fritz, J. et al. [Upwash exploitation and downwash avoidance by flap phasing in ibis formation flight](https://doi.org/10.1038/nature12939). Nature 505, 399–402 (2014).
- Raw Data from [behavioR package](https://github.com/DenaJGibbon/behaviouR) with the following script to convert to csv:
	:::{code}
	!pip install rdata
	import rdata
	import pandas as pd
	path = '/content/MeerkatScanData.rda'
	parsed = rdata.parser.parse_file(path)
	converted = rdata.conversion.convert(parsed)
	converted['MeerkatScanData'].to_csv('MeerkatScanData.csv')
	:::
