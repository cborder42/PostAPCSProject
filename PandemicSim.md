# Disease Propagation Simulation
## Authored by Daniel Welicki, Joshua Wu, and Aryav Taneja

**Stage 1:**  Proposal

Goal: Create a simulator to accurately predict the spread of a fictional disease.

Execution: Upon starting the program, a swing GUI with several sliders and buttons will appear.
- R0 level
- CT level (not sure if this is important)
- Viral instability 
- Number of days to be modeled
- Is a vaccine available?
- Is airborne?

Structure:
- There will be 7-8 different people.
- Each person will have a variable corresponding to age, gender, immune resistance, and a random check as if they are vaccinated. If they are vaccinated, their immune resistance will recieve a boost.
- Person object will contain methods to simulate the behavior of the virus inside of the bodies, and this will be read back to the main game object or a virus object (not sure about this yet).  For example, one such method will return the amount of viruses formed in their body, if they infected anyone (determined with the r0 level), if they're infected, and if they're dead. This will all be determined in the same row of execution - No memory will be saved, that way the 7-8 people are different in each play of the game. 
- We can have a for loop that runs the infection sim, returns the results, and then repeats.
- The virus has a random chance to mutate in each body, and if this occurs this will modify the variables of the r0 level or the airborne-ness based off of the inital viral instability.

Simulation behavior: 
Note: these ideas are not final, may or may not be in the final project
-	Using Math class create a method that returns a Boolean for whether or not a person is infected. This method should take attribute from the 7-8 different archetypes of people, and have a different response for each
-	Making a method that takes values from the previous method described and runs it for the total population of the simulation, this will return 3 values that represent the number people infected, the people that are healthy, and the percentage of the total population that is infected
-	There will be another class called simulate, which will run the simulator and return all relevant values, that will be fed into the GUI, if possible
-	The age parameters will be generated off of a weighted probability, which will return age values based on population distribution of the US
-	Age will impact the virus resistance of each person, by a predetermined factor, based on real world values
-	Preexisting conditions will be simulated will real values, and have different severities, dependent on real world distribution
- The values will be adjusted by a GUI slider, that will be able to change the r0, viral instability, vaccine availability, number of days modeled
-	Sliders for value that can be adjusted, buttons for the values that are Booleans
-	Simulation graphs, of number of population dead, infected and healthy (if possible)
-	Virus growth simulated by exponential growth
-	Virus mutations, changing the r0, and difficulty to create vaccine (ie. longer vaccine time, lower availability)
-	Average age distribution adjustment, calculated based on a Gaussian curve

