# GDIM 33 In-Class Activities
## W1
### Activity 1
[inspo board](https://docs.google.com/drawings/d/1G2mFoFEvYl0a3oEj7IO_SSPYTYIiMpLpZvGJVYucGEA/edit?usp=sharing)

For the images I put on my inspo board, I included screen shots when I was playing Genshin Impact and Honkai: Star Rail. And I also put pictures when I was relaxing and travelling around. There are also photos my by dear cat. I believe that I am currently interested in fictional games and stories, cute characters, and things related to cats, delicious food, travelling, and ficion stories. 
I wish to do a visual novel game, but I worry if it requires a lot of graphical sources and writing works. And I may also make a 2D platformer game, but I don't have much ideas about what content I will include in the 2D platformer game. 

I chatted with the girl next to me, and she planned to make a 2D platformer game. In her game, she plans to present some very cute and lovely animals. But when players go closer to these games, the animals will turn immediately into fierce monsters. We have similar personal styles such as cute pets. She put a doggy on her inspo board, and I put my cat on my inspo board. We both love lovely pets around us.  

I randomly grabbed Eric to take about his tastes. He was interested in PVP games. Totally different from my tastes of games. But I also like playing with many strangers together. 

### Activity 2
I will make a 3D survival game. But it may not be a horror game because I am always afraid of horror games. In my plan, the player will appear in an enclosed space filled with water. Water keep getting into the space. The player needs to find the positions where water pipe breaks. Once the player fixes the water pipe, it will stop leaking water and it will decrease the total amount of water in the space. I will use NavMesh to navigate the positions of broken water pipes. I will also use timeline to show cutscenes and VFX sequencing. For cutscenes, I plan to place the camera in different positions between when the player is fixing the pipe and when the player is finding the pipe. For VFX sequencing, when player has stayed inside water for too long, the color tone will be dark and the screen will seem to be distorted. The player will repeat movements as go under water -> find the problematic pipe -> find the tool to fix the pipe -> go out to water to breathe. 

[break down](https://docs.google.com/drawings/d/1DVmkJuQFL1z7H0Tt06RomRasbgyEpttTVnYgcJZo0co/edit?usp=sharing)

## W3
### Activity 1
[Break down](https://docs.google.com/drawings/d/1DVmkJuQFL1z7H0Tt06RomRasbgyEpttTVnYgcJZo0co/edit?usp=sharing)

### Activity 2
1. Scene variable can be accessed by all the script machines in the entire unity project. While we need to trigger the custom event in another graph, we have to have access to the event in the graph in the game controller. If we save the event name for the event inside the game controller, we can access the name of the event in the graph in another graph by setting it as the scene variable.
2. It can help me know if an event is triggered. For example, when the game controller is currently in explore state, debug log will print "OK!" In the explore state, the animals will be falling. It is hard to see the animals immediately after we exit the dialogue because we have to move our cursor quickly up, which is a hard work for the fingers. When I see "OK!", I will be happy to know that the animals are falling now without hurting my finger.
3. Yes. I planned to hide the cursor in the middle of the screen when player is not using the mouse. And if player want to use the mouse to change the direction of the camera, they can call the cursor and find it located in tme middle of the screen. 
4. Yes. I planned to show the entire game progress using the pamphlet UI using a line of quests. Different game states can update which process the player is currently at. There for, I can use game states to update my game progress in my game controller and tell how pamphlet UI to change its UI.