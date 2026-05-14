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
4. Yes. I planned to show the entire game progress using the pamphlet UI using a line of quests. Different game states can update which process the player is currently at. Therefore, I can use game states to update my game progress in my game controller and tell how pamphlet UI to change its UI.

## W4
### Activity 1
1. Playtest goal
My current game build contains a little bit of UI and player movement:
- UI
    - Player click on button called "pamphlet" and an empty panel will appear on the screen
    - In the panel, player click on button called "return" and the empty panel will disappear from the screen
- Player
    - player can use WASD to move, player can use ZC to move up and down
    - player can use cursor to change the direction of the camera to change direction of the player
    - right button of the mouse can increase speed of player

2. Name of playtest team members
Xichan Zheng, Jingyi Bi, Yan Zhang, Alex Ding, Tina Meng(ME)

3. Playtest notes
- Can't use the cursor to change the direction of the player
- In certain directions, W make player go forward, S make player go backward
- The UI is too simple, almost nothing in the scene, player don't know what to do
- If click on right button of the mouse, the player will immediately fly up to nowhere
- Sometimes the player can't use WASD to move around

### Activity 2
1. Yes. The programmer can use for loop to add more dialogue. They can create a list of dialogue sentences to store teh dialogue content. Then, they use the index for contents in the list to increase the sentence presenting. The body of the for loop shall be changing the specific TMP text content that shows the dialogue. 
2. I think there is no limit except for there is fixed space for all the buttons referring to the node. Like in this week's activity, prof said that, "The way I set up the UI, the player can have up to 4 options at once before the screen runs out of space". We can only put 4 option buttons on the screen. 
3. Regenerates nodes saves all the changes we do on the basic setting on the nodes. It is like refreshing the entire unity project to make sure it implements all the changes we made on the basic settings. 

## W5
### Activity 1 - NavMesh
Basic steps:
1. Randomly generates a 3D vector that located within the space of the room
2. Make the NPC move towards another random position (move randomly) using the NavMesh
Detail steps:
1. Create and bake NavMesh, try to find out if it is possible to draw the NavMesh blue print on different y levels separately
2. Create an empty game object with only Transform in the scene. Code the NPC to make its NevMeshAgent move towards the game object.
3. Add another empyt game object. Code the NPC to make the transform position of the new game object take the place of the transform position of the old game object.
4. Move the empty game objects to make sure the transform position range of the area that I want the NPC to locate.
5. Randomly generate a position for the emtpy game object in the code, test if it is within the space
6. Randomly generate one position for the empty game object in the code, make the NPC goes toward the game object using NavMesh
7. Try to test if the NPC arrive at the position generated using OnTriggerEnter on the gameobject. 
8. write codes for random wondering of the empty game object within the same y level.
9. make NPC to follow the game object using NavMesh every frame

### Activity 2
1. Created and baked NavMesh. I downloaded AI navigation from package manager. I then added component NavMeshAgent to the NPC that I want to move. I also created a NavMesh surface and lifted it up to make the fish seem to navigate in the air (swimming in the water). I then wrote a new C# script for FishNPC and attached it to the NPC fish I want to move. In the code, I used navmeshagent.setdestination() to guide the fish to a new position. I also used random.range() to generate random positions in the space to make the fish navigate to. I wrote Vector3.Distance() to make sure the fish is now close to the destination I assigned and then I call the method to generate a new random position. 


## W6
### Activity 1
1. Playtest goal
- I added NavMesh agent and surface. 
- I added 5 NPC fishes.
- I make the fishes to swim around all by themselves
- [itch link](https://tinamengxq.itch.io/33test-mile2)
2. Result
- add transparent walls on the top of the room
- make the camera can move on the y axis
- create more obvious feedback every time the fish is hurt
- increase font
- create more obvious feedback after player fixed the pipe

### Activity 2
1. While the values are all between 0.0 and 1.0, the result of multiplication between two values that are both between 0.0 and 1.0 will be small than either values. Therefore, the colors will be less saturated than the original colors. And as color values increase, they will be closer to white. If they become smaller, the color will be darker.
2. More translucent. Because multiplication between Alpha values decreases the result. As Alpha values get closer to 0, the color will be more transparent.
3. The UV coordinates of the texture's mesh?
4. Soso?

## W7
1. Vertex color node gives the vertex vector stored in the mesh ([reference]{https://docs.unity3d.com/Packages/com.unity.shadergraph@14.0/manual/Vertex-Color-Node.html}). So I think the data comes from the mesh. 
2. The vertex color in step (3) comes from a normal vector. The default value of a vector might be (0, 0, 0). In the 0-1.0 scale of RGB, 0 represents the edge of the color range. 
3. I think because the vertex color only applies the specifc color used on the model, but the texture suggests more details differences in color details between different surfaces. I imagine that the vertex color might be used for views far away in a world that don't need to show any more details.
4. I think the problem is that the color is black and white. There are many colors in the graph but the color only shows black and white. 
5. We can use simple calculation like addition and multiplication to change some small values of our vertex color vectors. I think we can use such debug shader on simple vertex values when we want to figure out what is the exact color we want to present in the game.
6. This is because the calculation of vectors in unity have directions relative to the direction of lights. This will lead to different lighting effects in different directions.
7. Because there is a color combition between two sources of colors. 

