# wonky puzzle game proposed by felix celina and zoe (checking if fiona wants to join)

**Stage 1:**  Proposal

So the basic idea is that we're making a digital puzzle game. 

A picture could be pre-uploaded/prepared or the player could upload a picture themselves (still have to decide which one we're doing) then selects the number of puzzle pieces (preferably a composite number). Our code would split the original picture into the determined number of pieces, marking each piece going left to right, top to bottom to keep track of where the puzzle pieces are supposed to be. Then the puzzle gets scrambled and pieces now get labeled left to right, top to bottom again, except their pre-scramble-assigned numbers stay with them. The scrambled image, which will probably be like a 2D array of smaller pictures or something (still have to understand how images work), will then be displayed, with their post-scramble numbers displayed somewhere for the player to keep track. A grid will then be displayed, corresponding to the puzzle size, and the player can enter their answers there by entering the post-scramble numbers back into the right boxes. We then would have to compare the pre- and post-scramble numbers and see if they match somehow (perhaps each puzzle piece would have two integer variables, a pre- and post-scramble number). If they do, then we congratulate the player and display the original image. If they don't match, then we tell them wrong, redisplay the scrambled image and answer grid, and the game goes on. If the player wants to quit at any point they should be able tojust enter "stop" or something else and the game should end right there. 

Anticipated file structure: 
- A puzzle piece class that has the picture, pre-scramble number, and post-scramble number
- A puzzle class would probably have the dimensional structure of the puzzle, along with a solved boolean variable
- A scramble method that calls the splice method and randomizes the composition of the image 
- (We'd also have to either keep on asking the player for a composite number if they keep entering a prime number, or we just have an extra large piece)
- A splice method that creates this 2D array of images, along with determining the dimensions based on the nnumber of pieces the player wants
- A game method to play the game
- Another class to call the game method to play the game

New Java: 
- We'd have to learn how to import, display, and splice up an image (most crucial part of this)
- We'd also have to learn how to display this grid that the user can click around and enter their answers into

A proposal for a project requires at least three students,
with at least one student from each block!  (This will require
you to utilize GitHub and learn about branches, commits, and pulls.)
The proposal must address each of the following:

- [ ] General description of the goal or purpose.  What are you trying to make happen or solve?  Feel free to design projects which utilize content from other courses (simulations, for example), address and analyze real daata and problems (the environment, anyone?), or have other useful impacts.
- [ ] Anticipated file structure (i.e. what classes will you write, where will the `main` method exist?  Show me that you have thought enough about this problem or project to begin to recognize some of the complexity you will need to account for.
- [ ] New Java - your proposal/project must require you to utilize some new code structures.  This could include learning how to read/write files into a JAVA program, rudimentary graphics, or some utilize some other `class` for your project.
- [ ] Division of labor:  who will do what in this project?  Is there enough required to justify the time and number of people?  This will be the sole task which you will be engaged in during class time, but there is minimal expectation for work outside of class (unless you are not meeting your goals).
