# Argon Assault

### Introduction
    Realm Rush is a rail shooter game in which the player controls a ship that can fire laser bullets. The player 
    guides the ship to avoid obstacles and destroy enemies by shooting them.

### Features
    - Intuitive and Responsive Controls:
        - Easy-to-use controls for smooth navigation and shooting.
        - Skillfully maneuver the ship with pitch, yaw, and roll controls, ensuring responsive and precise control.
        
     - Cinematic Enemy Ship Arrival:
        - Experience cinematic moments as enemy ships elegantly enter the scene, enhanced with Unity's Cinemachine
          for a visually engaging gameplay experience.
          
     - Dynamic Level Design: 
        - Well-crafted levels with dynamic environments, including enemy ships firing missiles and large enemy ships incoming.
        - Spacious vibes and immersive sound effects to enhnace the overall atomsphere.
    
### Screenshots

   ![StartMenu](./Screenshots/MainMenu.png)
   ![TowerShooting](./Screenshots/TowerShooting4.png)
   ![TowerShooting](./Screenshots/TowerShooting.png)
   ![TowerShooting2](./Screenshots/TowerShooting2.png)
   ![EnemyDestroyed](./Screenshots/EnemyDestroyed.png)
   ![GameOver](./Screenshots/GameOver.png)

   
### Implementation and Game Design
#### Implementation
    - PathFinder: Responsible for finding the shortest path on the grid using the breadth-first search algorithm 
                  implemented using data sturctures like dictionary and a queue.
    
    - TowerFactory: Responsible for limiting the instantiation of towers to a maximum of 7 and reusing already 
                  spawned towers for performance using the queue.
                  
    - Tower: Responsible for finding the nearest enemy and targeting them. After destroying the targeted enemy, 
                  it selects the next nearest one.
             
    - EnemySpawner: Spawns enemies at fixed intervals.
    
    - EnemyMovement: Obtains the shortest path from the PathFinder and follows it.
    
    - EnemyDamage: Manages hit processing and destruction of enemies.
    
    - GameManager: Responsible for managing game states, such as running, pausing, or activating the game over 
                   screen if the player is defeated.
                   
    - Cube Editor: An editor script for placing grid blocks (waypoints) only at integer coordinates, crucial for 
                   pathfinding, as it relies on integer coordinates.

 
 #### Game Design
     - Designed strategic level independently using provided assets.
     - Implemented an editor script(CubeEditor) to facilitate the placement of blocks (waypoints) with restricted 
       integer coordinates.
       
#### Focus
    - Learn Unity's Terrain component to create terrain, utilize terrain tools, and apply texturing and trees.
    - Learn Unity's Timeline for creating cinematic scenes, such as the entrance of enemies as the player enters 
      a specific area.
    - Learn about quaternions for rotation, including pitch, yaw, and roll.
    - Become familiar with using a Particle System for firing laser bullets.
    
### Gameplay Demonstration
    - For a visual demonstration of the gameplay, watch video on YouTube:
 [Youtube video link](https://youtu.be/cmyqPkxtXsE)

### Play the Game
    - To experience the game firsthand, play it directly by following this playable link:
[Play in browser(WebGl)](https://rahul-pargi.itch.io/realm-rush)
