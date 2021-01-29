
# Chess  :chess_pawn:

 > Authors: (names listed in alphabetical order)<br />
[Chun Ho Wong](https://github.com/cwong165) :space_invader:  <br />
[Danial Mirza](https://github.com/danialmirza99) :ghost: <br />
[Francisco Quiroz](https://github.com/FrankyQuiroz01) :japanese_goblin: <br />
[Jared Tanuwidjaja](https://github.com/matchasaur) :speech_balloon: <br />
 
<br />

**Description**:video_game:

The Project itself is interesting because it will not be a straightforward chess game, in the sense that we are required to have boards that are saved in case we ever want to hold off the game to a later date in which we would continue the game. 

Not only that, we would also love to include A.I. in which we will have the computer be our opponent. This means we at the minimum must have an A.I. smart enough to recognize that
 - (1) A move is possible
 - (2) The importance of the king to prolong the game so that it does not end quickly

*This is slightly more challenging and may be subject to change.*
<br />

**Languages/Tools/technologies**:man_technologist:
 >  * C++


**Input/output**:robot:
 > * Keyboard
 > * Mouse(optional)
 > * Monitor
 > * Speaker(optional) 

**Design Patterns**:speech_balloon:
 - Prototype (Creational Pattern)
   - We chose this pattern to allow for prototypes of the chess game itself. This will allow us to test individual pieces and how they move, without the need of a fully developed class for y piece when we are testing x piece. This will be especially useful as we have 7 unique chess pieces. Not only that, we will be able to find issues in a single class much earlier than if we had fully developed all classes which saves us a large amount of time. This will further help us understand how the classes interact with each other and if any problems occur, when a prototype of the final project itself is made.
      * We expect that some of our individual pieces will have issues regarding the rules of their movement, i.e. the pawn moves forward and can only move diagonally to take a piece. By making a copy of the class and running it, we may be able to see if it absolutely obeys these rules or if it breaks under specific circumstances. Another thing we can do is make a copy that implements multiple of our classes to see how they interact with each other. If any problems occur or worse our program crashes, we will be able to see it on a prototype and fix it on the main product.
         * Prototype will allow us to make a copy of our code in certain stages that we want or will be critical to the overall project. This way we will be able to tell if our code can execute up to this point, or if it breaks. If it breaks then we know the code has an issue somewhere before this point that does not allow the program to execute correctly. If we want to be extremely direct we can also copy each bit of code and make a prototype for each individual function and that will serve as our unit tests for the program and not just the code.
 
- Strategy (Behavioral Pattern)
    - We chose this pattern because it will allow us to implement movement for each unique piece while maintaining organization and avoiding redundant code. Chess has six unique pieces, each with different movement patterns. Utilizing the Strategy pattern would allow us to construct a base ChessPiece class and divide each movement algorithm into separate strategies. This will allow us to reuse code if a chess piece shares a movement pattern identical to a different chess piece.
        



**References:**\
https://en.wikipedia.org/wiki/Chess  <br />
https://en.wikipedia.org/wiki/Chess_symbols_in_Unicode  <br />

 





**__________________________________________________________________________________________________________________**
<br />
<br />
<br />
<br />
<br />
<br />
<br />



 
 > ## Phase II
 > In addition to completing the "Class Diagram" section below, you will need to 
 > * Set up your GitHub project board as a Kanban board for the project. It should have columns that map roughly to 
 >   * Backlog, TODO, In progress, In testing, Done
 >   * You can change these or add more if you'd like, but we should be able to identify at least these.
 > * There is no requirement for automation in the project board but feel free to explore those options.
 > * Create an "Epic" (note) for each feature and each design pattern and assign them to the appropriate team member. Place these in the `Backlog` column
 > * Complete your first *sprint planning* meeting to plan out the next 7 days of work.
 >   * Create smaller development tasks as issues and assign them to team members. Place these in the `Backlog` column.
 >   * These cards should represent roughly 7 days worth of development time for your team, taking you until your first meeting with the TA
## Class Diagram
 > Include a class diagram(s) for each design pattern and a description of the diagram(s). Your class diagram(s) should include all the main classes you plan for the project. This should be in sufficient detail that another group could pick up the project this point and successfully complete it. Use proper OMT notation (as discussed in the course slides). You may combine multiple design patterns into one diagram if you'd like, but it needs to be clear which portion of the diagram represents which design pattern (either in the diagram or in the description). 
 
 > ## Phase III
 > You will need to schedule a check-in with the TA (during lab hours or office hours). Your entire team must be present. 
 > * Before the meeting you should perform a sprint plan like you did in Phase II
 > * In the meeting with your TA you will discuss: 
 >   - How effective your last sprint was (each member should talk about what they did)
 >   - Any tasks that did not get completed last sprint, and how you took them into consideration for this sprint
 >   - Any bugs you've identified and created issues for during the sprint. Do you plan on fixing them in the next sprint or are they lower priority?
 >   - What tasks you are planning for this next sprint.

 > ## Final deliverable
 > All group members will give a demo to the TA during lab time. The TA will check the demo and the project GitHub repository and ask a few questions to all the team members. 
 > Before the demo, you should do the following:
 > * Complete the sections below (i.e. Screenshots, Installation/Usage, Testing)
 > * Plan one more sprint (that you will not necessarily complete before the end of the quarter). Your In-progress and In-testing columns should be empty (you are not doing more work currently) but your TODO column should have a full sprint plan in it as you have done before. This should include any known bugs (there should be some) or new features you would like to add. These should appear as issues/cards on your Kanban board. 
 
 ## Screenshots
 > Screenshots of the input/output after running your application
 ## Installation/Usage
 > Instructions on installing and running your application
 ## Testing
 > How was your project tested/validated? If you used CI, you should have a "build passing" badge in this README.
 
