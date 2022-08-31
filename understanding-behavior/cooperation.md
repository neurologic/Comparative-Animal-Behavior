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

<hr>

### Raw Data

From [behavioR package](https://github.com/DenaJGibbon/behaviouR) with the following script to convert to csv:

:::{code}
!pip install rdata
import rdata
import pandas as pd
path = '/content/MeerkatScanData.rda'
parsed = rdata.parser.parse_file(path)
converted = rdata.conversion.convert(parsed)
converted['MeerkatScanData'].to_csv('MeerkatScanData.csv')
:::
 
## Reading

- [Cooperation](http://pages.nbb.cornell.edu/Gamebug/cooperation.html)
- [V-formation flight commentary](https://www.science.org/content/article/why-birds-fly-v-formation)
- Weimerskirch, H., Martin, J., Clerquin, Y. et al. [Energy saving in flight formation](https://doi.org/10.1038/35099670). Nature 413, 697–698 (2001).
- Portugal, S., Hubel, T., Fritz, J. et al. [Upwash exploitation and downwash avoidance by flap phasing in ibis formation flight](https://doi.org/10.1038/nature12939). Nature 505, 399–402 (2014).
