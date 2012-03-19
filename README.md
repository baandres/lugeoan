# MATLAB FS12 – Research Plan (Template)
(text between brackets to be removed)

> * Group Name: Lugeoan
> * Group participants names: Andrés Barreiro, Georg Zangger
> * Project Title: Festival Pedestrian Dynamics

## General Introduction

Simulative security checks for festivals could be a simple and cheap standard approach to avoid dangerous mainstream dynamics.
After the catastrophe at Loveparade 2010 in Duisburg, several autorisation offices adapted their standards.
In Zurich, they changed the prescribed placement of food and drink shops for the Longstreet Festival 2012 by reason of the new crowd management.
After that, the festival organisation cancelled the Longstreet Festival 2012.
They complained among other things about less allowed food and drink shops and new placement of them.
We are interessted in the geometic influence in general  and  beside in the question,
if there is a difference between new and old rules in aspect of crowd dynamics. Specially, 
we want to simulate pedestrians in the area of the rail subway between the bus stations 
Röntgenstrasse and Militär/Langstrasse. 

## The Model

Dirk Helbing wrote different  papers about „simulating dynamical features of escape panic“.
In his papers, he introduces a self-driven many-particle system based on a generalized force model to simulate the crowd dynamics.
A mixture of sociopsychological and physical forces gives the different weights an adapted velocity every dt.
This model allows us to observe important scalar and vector fields like pressure,
relative efficiency and pedestrian density, where relative efficiency means actual speed
projected in desired direction divided by desired velocity.

Helbing suggest some values for the parameters in his model as well.
Based on his model and values, we want to expand and adapt parts of the model
if we find important difference of simulated, observed or expected behavior.
We want to implement different kinds of people by using individual values for some parameters like:
agressiveness, panic potential and weight. For some values, we will just do assumptions,
for others short observations. We will assume and define certain start values of dangerous situations.
We wan‘t modell the dangerous situations itself with people falling on the floor and so on. 

If we will have still enough time, we are interessted in an additional model as well,
which allows us to simulate the people going throgh the system border of the first model.
The second model should be more efficient in calculation, with cellular automata and simpler rules.

## Fundamental Questions

What influence takes different  wall geometry to crowd dynamics of high density? 
If there are food and drink shops close to a narrow passage,
does it make sense to arrange them in certain angle?
What placement is dangerous or just not optimal? 

Depending on the progress, needed time of our work and the numeric problem size,
we are also interessted in possible approaches to describe the festival dynamics around the generalized force model.
The force model needs a lot of calculations, it’s just usable for limited number of pedestrians.
To calculate pedestrians going through the system border of the first model, we need the second one.
A possible reason for moving pedestrians are concerts, where several people want to go at several time.
Some pedestrians could follow the others spontaneously. The task in this optional second part
would be to find scenarios where the system border conditions of the subsystem
causes dangerous situations in the subsystem at some time.

## Expected Results

We expect generally different critical crowd behavior under and beside the narrow passage,
depending on the placement of food and drink shops and other geometric aspects.
Really important will be the passable width in key places. The distribution of shops will take an important rule as well, 
if the shops  reach certain critical density and under certain critical conditions. 

Little angulated  shops  beside the street after the narrow passage could be usefull in comparation to not angulated shops.
The entrance flow could be reduced, holding outside flow more or less on the same level... but there will be just little optimization potential. 

With geometric influence, we expect it to be possible to channelize people to the right side of the norrow passage
which has influence on efficiency. 

From the change of the prescribed placements of shops at Longstreet Festival 2012, we expect just little difference in the ovserved values. 

If we implement the full festival to simulate the boundary conditions of the critical subsystem,
we need two different, connected simulation conceptions.
We expect to find some conditions for the second model (Longstreet Festival),
that there are dangerous situations in the subsystem at some time. 

## References 

crowd turbulences -  Wenjian Yu and Anders Johansson ; 2007
self-organized pedestrian crowd dynamics – Helbing ; 2005
collective pedestrian dynamics – Schadschneider, Kirchner and Nishinari; 2002
escape panic – Helbing; 2000
social force model for pedestian dynamics – Helbing ; 1995

related projects from others:
https://github.com/mthielma/SOCIAL_MODELING
https://github.com/jjoolloo/Swiss-Slovak-misunderstanding/
http://www.crowdscontrol.net
https://github.com/tohojo/RUC-math--crowd-modeling

Collective Dynamics In Human Crowds - mehdimoussaid.com/publications.html

Modeling the 2010 Love Parade Evacuation - www.soms.ethz.ch/teaching/MatlabSpring11/projects/Loveparade_Evacuation_Fougner_Guthrie.pdf

## Research Methods

We have different options by now:
	- We started working with a contiuous model for small areas.
	- We are considering a agend based based model, cellular automata.
	- Also, we will take a look at "Collective Dynamics In Human Crowds"
We will run different scenarios several times to consider statistical fluctuations. 

## Other

For the parameters of our first model, we use the values suggested by Helbing.
We make short tests if they make sense and optionally,
we make own distributions for parameter values by own observations. 
For the second modell, we make assumptions. We will use data from the festival autorisation office of Zurich as well. 