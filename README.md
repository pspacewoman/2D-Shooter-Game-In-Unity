**2D Shooter Game in UNITY** 

![Unity](https://img.shields.io/badge/Unity-100000?style=for-the-badge&logo=unity&logoColor=white)

My Objective:
- Creating 2D Game
- Working with 2D Sprites
- Create 2D Animations
- Implement 2D Mechanics
- Create a complete game loop
- Create UI elements that work across multiple resolutions and aspect ratios
- Build the game for multiple platforms

___

**UNITY INPUT**
- Input Manager (built-in)
- Input System (package) --- For this project, I used this input system.
- 3rd-party Input (ex: rewired)

___

**Setting up 2D Game on Unity**

1. Assets
2. Animation
3. Animator
4. Player Health & Damage Setup
   -  Physics Interactions: collider, RigidBody component, Custom Script Component
5. Player Shooting Setup: added player effect, shooting component and audio, converted player object to player prefab for iterative use
6. Camera Setup: created 2 camera prefabs - a large camera and a small camera with different sizes
7. Level Setup: created borders, backgrounds and test movement around the space

___

**Game Flow and UI Setup**

1. Game Manager and UI Manager Setup
- Created Game Manager and UI manager
- Created Canvas and EventSystem

2. UI Setup: Score
-  User Interface (UI): UNITY supports multiple methods for creating UI.
   + IMGUI
   + UI Toolkit
   + Unity UI package (uGUI): using this in my project
- Created Score and High Score buttons in canvas

3. UI Setup: Pause Screen
-  Created pause and unpause button
-  And added components on it and actions like escape and toggle when it appears during gameplay

4. Responsive and Scalable UI
-  Created new Aspect Screen 4:3
-  Set the 'score' and 'high score' static on the screen and fixed while moving around by: selecting anchor presets

5. UI Setup: Other IN-GAME UI
-  Adding 2 screens: one for when a player loses and one for when a player wins
-  GameOverScreen
-  LevelVictoryScreen
-  Added a 'main menu' button on the pause screen as well

6. UI Setup: Main Menu
-  Setting up the main menu within a new UNITY Scene
-  Assets > _Scenes > MainMenu (scene created)
-  Added all the scenes level1 and mainmenu on Build profiles > all scenes and tested the flow

7. Finish the Gameplay Loop
-  For scene Level1:
-  Added 2 more enemies in the game
-  Changed CANVAS > InGameUI and made it a prefab under UIpages

8. MUSIC
-  Adding 2 music in one main menu and another on the game levels
-  heirarchy > create empty > music name > added component 'audio source' > prefab drag drop music to component > done

___

**Finishing Up GAME Development**

1. Adding More Levels
-  Duplicate Scene Level1 to Level2 and Level3 and add them to build profiles
-  Goto Scene Leve1 > NextLevelScreen > set to Level2
-  Same for Level2 > Level3
-  Now, while testing, I noticed once the Level is complete I am asked to jump to next level scene

2. A Deeper Dive Into TextMesh Pro
-  
