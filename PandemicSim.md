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
