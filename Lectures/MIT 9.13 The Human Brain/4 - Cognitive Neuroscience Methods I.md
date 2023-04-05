The goal of cognitive neuroscience is to understand how the mind emerges out of brain. Standard working framework is:

> Mind = a set of *computations* that extract *representations (= percepts/thoughts)* 

Hence it is very important to think, *what is computed and why.*

## Marr Computational Theory Level of Analysis

>*“Trying to understand perception by studying only neurons is like trying to understand bird flight by studying only feathers; it just cannot be done. To understand bird flight, you need to understand aerodynamics, only then can one make sense of the structure of feathers and the shape of wings. Similarly, you can't reach an understanding of why neurons in the visual system behave the way they do, just by studying their anatomy and physiology. “* - Marr

>*"The nature of the computations that underlie perception depends more upon the computational problems that have to be solved than upon the particular hardware in which their solutions are implemented. “* - Marr


So, for example, to understand why we see color, we need to first ask ourselves: **What do we use colors for?**

- For finding food
- For identifying properties of the objects
	- Is the food worth eating or is it rotten?

> It was found that macaques with 3 kinds of cone photoreceptors (just like humans) are faster at finding fruit than genetic variants with only two. (Melin, 2017)


## Problem

We want to determine the color (or **R**, "reflectance") of an object.

But all we have is the light coming from the object (L). And that L is not only a function of the object, but also of the light shining on the object (the "illuminant" or **I**): 

![[Pasted image 20230406003923.png]]

$$ L(\lambda) = R(\lambda) \times I(\lambda) $$
*Given L, what is R?*

This is known as an "Ill-posed" problem.

Implications: Inferring R from L requires other info or assumptions about I. 

<span style="color:orange;">Big point: </span>Many inferences in perception and cognition are ill-posed. So require extra knowledge/assumptions about the physics/statistics of the world. 

### Shape Perception

Each retinal image could have been cast by many diff. objects. Inverse optics is “ill-posed”, need other constraints to solve.

![[Pasted image 20230406005236.png]]

### Word Learning

Many possible meanings of a word. "Gavagai" can mean anything. Rabbit? Fur? Ears?

![[Pasted image 20230406005335.png]] 


## Maar's Levels of Analysis applied to Color Vision

1. Computational theory

	what information is extracted and why? 
		R, useful for characterizing objects 
	
	what cues are available? 
		only L! 
	
	is the inference ill-posed? 
		Yes! because I is unknown 
		
	what regularities in the world constrain the inference? what other sources of information might constrain I?

  *all of this with no data about mind or brain or machines! one way: just thinking, with a little optics, physics, ecology psychophysics!*  
  
2. Algorithm/representation 

	  how does the system do what it does, i.e. they see can we write the code to do this? for example…. what assumptions, computations representations? how would we find out?


## Functional Magnetic Resonance Imaging (fMRI)

The best spatial resolution available for measuring neural activity non-invasively in the whole brain.

"BOLD" (Blood Oxygenation Level Dependent) signal: If a bunch of neurons some place in your brain start firing a lot, it is metabolically expensive, so you have to send blood to that part.

Steps:

1. Increase in neural activity

2. Increase in local blood flow more than compensated for O2 use. 
		Active (active as in fMRI active, not "activity" active) parts of the brain, has less, not more, deoxygenated hemoglobin. This is important because oxygenated and deoxygenated hemoglobin are magnetically different in the way that the MRI signal can see. So the signal we are looking out for is the how much O2 is in the blood at a specific part of the brain, and hence how much blood flow went there, and hence how much neural activity was there.
	
3.  Decrease in deO2Hb concentration

4.  Increase in MR signal intensity (deO2Hb is paramagnetic)


### Important caveats about the BOLD fMRI signal:

BOLD response is slow, usually peaking around 5-6 seconds after stimulus onset.

This is mainly because it is very indirect. Neural activity -> blood flow change -> over compensation -> different at magnetic response. 

![[Pasted image 20230406014324.png]]

Caveats:
 - Because the BOLD signal is based on blood flow, the spatial and temporal resolution is limited.
	 - ~ 1mm; > a few 100 millisecond
 - Physiological basis of the BOLD signal is unknown.
	 - Action potentials? Synaptic activity? Inhibition?
 - Cannot measure absolute amounts of activity/metabolism, only differences between two conditions.
	 - The number you get out is the intensity of the deoxygenated hemoglobin. Does not translate directly into an absolute amount of neural activity.

### Examples of using fMRI

#### Is there a region in the brain specialized for face recognition?

1. Scan subjects as they view faces and objects 

	![[Pasted image 20230406015238.png]]

2. Does it respond to anything human? any body part? anything attended? anything curvy?

	![[Pasted image 20230406015500.png]]


This proves that there is a specific region in brain for face recognition. It's called the [[Glossary#^d42ddf|Fusiform Face Area]].
