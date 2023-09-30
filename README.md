# GeneticSimulation
******************************************
 Population Genetics Simulation
******************************************

************************************************
Authors: Wangari Mbuthia ,Majd Ayyad

************************************************


******************
Instructions: 
*******************
	•	Use the first slider (Population Size) to select your desired population size.
	•	Use the second slider (Frequency of Allele A) to select your desired frequency. This must be a number from 0 to 1. The frequency of allele B will be calculated.
	•	(Optional) Use the input boxes to enter  the fitness of the different genotypes. The default will be set to 1 i.e equal fitness)
	•	(Optional) Use the third and fourth slider to set the forward mutation rate of allele A → B and the backward mutation rate of allele B → A. The default is set to zero for both rates.
	•	Use the Number of Generations to set the number of generations that you want the simulation to run. The default is set to the max 1000. 
	•	(Optional) Use the Phenotypic Desired Generation box to enter the generation that you want to see visualized. If the number of generations is N, this number can be in the range of 0 to N-1. The default is set to generation 0.
	•	Click the Run Simulation button and the frequency of alleles will appear in the figure.
	•	Repeat the Simulation with different population sizes, allele frequencies, mutation rates, fitness values and monitor the differences to study their effects.
**************
Summary:
*************
Our project is a Population Genetics Simulation. Population genetics is the study of the genetic composition of populations and how they change over time in response to processes such as natural selection, genetic drift, and mutation. The purpose of this project is to visualize the variations in allele frequency of two alleles (A and B) in a fictional population. It is useful for students studying topics in biology courses. 

Our simulation will help visualize concepts and theories like natural selection, genetic drift, genetic equilibrium and mutation (between existing alleles only). Natural selection can be visualized by changing the fitness of the different genotypes. Genetic drift is visualized in small populations and genetic equilibrium can be visualized in large populations. The effect of mutations can als be seen by setting forward and reverse mutation rates.

When the simulation is run a graph is produced to show the change in allele frequencies over time; a visual of the phenotypic distribution for a specific generation; and the generation where one allele (if any) became fixed (i.e its frequency in the population became 1) is also displayed. 

The code utilized some principles from population genetics equations to determine the frequency of genotypes and to account for varied fitness. It also uses a series of random decisions to build the population so each trial with the same parameters will have some variation. The creation of these decisions was  based on a paper explaining how a population genetics simulation works.

We utilized Matlab programming skills learnt in the semester to make the decisions using while and for loops with new skills in Matlab App Designer with regard to the user interface to finalize simulation and make it interactive for users. 

A challenge we faced was making the simulation responsive once it has run. For example we wanted to allow the user to continuously be able to enter in a generation to visualize the phenotypic distribution and that plot to update using previously stored data. The problem was that  we wanted to save from each simulation the three arrays (AA,AB,BB) referred to in the code as (AA,Aa,aa) in the properties section.Then, call the arrays in the callback of another button. We kept running into the same error which is not having the right property for the value. Our research about this error showed that the method we used was meant to save a single input variable, not an output array. We tried to look for methods used by other programmers but it did not work for our code. This is a challenge for us to solve outside the class and we will use the resources and the knowledge we learnt during this semester to overcome it.


************************************
Attributions and Citations:
**********************************
Resources that helped understand genetic concepts:
	•	https://www.nature.com/scitable/topicpage/the-evolgenius-population-genetics-computer-simulation-how-1167841/ - This paper help us create the logic of the simulation
	•	https://www.biologysimulations.com/population-genetics - This simulation was the inspiration to create ours 
	•	https://sites.radford.edu/~rsheehy/Gen_flash/popgen/ - This simulation that helped with inspiration to create ours

All code was generated by authors


********************
Dependencies: 
*******************
Matlab app designer (UIFigures and UIAxes)

