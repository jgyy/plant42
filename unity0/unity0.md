# Unity Piscine - Module00

Learn Unity basics by building a 3D game with movement, jumping, level design, and simple game-over logic.

**Version:** 2

## Summary

Here is the subject Module00 for the Unity piscine.

---

## Table of Contents

1. [Instructions](#chapter-i-instructions)
2. [Piscine Unity Starter Kit](#chapter-ii-piscine-unity-starter-kit)
3. [Introduction](#chapter-iii-introduction)
4. [Exercise 00: Floor Is Lava](#chapter-iv-exercise-00-floor-is-lava)
5. [Exercise 01: Path Of Exile](#chapter-v-exercise-01-path-of-exile)
6. [Exercise 02: My Even More Beautiful World](#chapter-vi-exercise-02-my-even-more-beautiful-world)
7. [Exercise 03: The Floor Is 'Always' Lava](#chapter-vii-exercise-03-the-floor-is-always-lava)
8. [Submission and Peer Evaluation](#chapter-viii-submission-and-peer-evaluation)

---

## Chapter I: Instructions

- If you have trouble installing the required tools for your project on the 42 computers, you may use a virtual machine. In this case, you must:
  - Install the virtual machine software on your computer.
  - Install the operating system of your choice.
  - Install the necessary tools for your project.
  - Ensure that you have enough space on your session to install all of it.
  - Have everything installed before the evaluation.

- Only this page will serve as reference. Do not rely on rumors.
- Carefully read the entire document before starting.
- Your exercises will be evaluated by your fellow piscine participants.
- This document is your reference. Do not blindly trust demos or example pictures, which may include unnecessary additions.
- Got a question? Ask the peer to your right. If not, try the one on your left.
- By Odin, by Thor! Use your brain!!!

⚠️ **Important Notice:**

Intra shows the date and time when your repositories close. This also marks the beginning of the peer-evaluation period for that piscine day. The peer-evaluation lasts exactly 24 hours. After that, any missing evaluations will be scored as 0.

---

## Chapter II: Piscine Unity Starter Kit

Welcome to the first module of the Unity Piscine. To get off to a good start, here is a list of useful tips and links that will help you throughout the Piscine.

### Resources

- **[Official Unity documentation](https://docs.unity3d.com/)** - You will also find a blue book icon in the Inspector near each component that links directly to its specific documentation.
- **[Official C# documentation](https://docs.microsoft.com/en-us/dotnet/csharp/)**

### Important Tips

- The subject prevails. Don't fully trust the demos as they may contain additional elements not required.

- If you create reusable generic utility scripts unrelated to gameplay, they will save you time in future modules.

- Once the module is completed, don't keep your project in your home directory. Unity tends to generate a huge number of files that will quickly eat up your 5 GB quota (and slow down your session).

- These modules are long, so don't waste time on unnecessary details. You'll have time to enhance your game once the mandatory parts are complete.

- If you or one of your neighbors has the answer to a **TECHNICAL** problem, you can share it on the forum using the Unity Piscine tag.

---

## Chapter III: Introduction

### "The Floor is Lava"

"The Floor is Lava" is a game in which players pretend the floor is made of lava (or another dangerous substance like acid or quicksand), and must avoid touching the ground or risk being "killed".

Players stay off the floor by standing on furniture or structures. They usually have to keep moving and can't stay on one object for long due to imaginary limitations (e.g., it's sinking or melting).

The game can be played solo or with others. It might include goals or races, and can be set up indoors or outdoors, with obstacles like padded chairs to increase difficulty. It resembles an obstacle course.

### Game Mechanics

- Anyone can start the game by shouting "The floor is lava!"
- Anyone still on the floor within seconds is out and must sit out temporarily.
- Some versions include items or locations that restore health or body parts, with tasks ranging from silly to simple, like finding someone.
- In "Hot Lava Monster" (also called "Skies in the Ringuss"), often played on playgrounds, the "monster" can walk on the lava and tries to tag others, who must stay on the play structure.
- The monster may have limitations like avoiding certain colors or platforms.
- The game is similar to "Puss in the Corner", where children must move from corner to corner without being tagged by the "Puss" in the center.

---

## Chapter IV: Exercise 00: Floor Is Lava

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | Exercise 00: Floor Is Lava |
| **Turn-in directory** | unityModule00 |
| **Required elements** | FloorIsLavaScene scene, Floor, Pathway GameObjects and any relevant elements |
| **Forbidden functions** | None |

### Objective

The purpose of this module is to get you familiar with the different tools provided by Unity.

To start, create a new 3D project and name it **Module00**. A sample scene has already been created—you can work directly in it. Rename this sample scene to **FloorIsLavaScene**.

You'll only need one scene for all the exercises.

### Project Setup

To create this game, you'll need:

- The floor!
- A pathway.
- A player.
- Some decorations.
- A camera.

### Implementation

#### The Floor

- Create a **Floor** GameObject using a primitive square.
- Choose its size (it doesn't need to be huge).

#### The Pathway

- Create an empty GameObject named **Pathway**, in which you'll place all the different GameObjects (stairs, bridges, or whatever you like) that will make up your pathway.
- When building it, keep in mind the goal of the game: move along the pathway without touching the floor!

#### Decoration

- Your scene must include at least one composite structure (with colors, because it looks nicer!).
- Example: A tree (but feel free to come up with your own creations)
- The example shows a scene with a green tree, textured ground, and various platforms

#### The Player

- Your player will look like a ball, so choose an appropriate 3D object.
- Make it look nice by adding a material, color, reflections, whatever you like.
- Place it at the start of the pathway.
- You'll add movement in the next exercise.

#### The Camera

- The main camera is automatically created when you start the project.
- For this module, you don't need to modify it.
- Just position it high enough so the player can see the entire pathway.

---

## Chapter V: Exercise 01: Path Of Exile

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | Exercise 01: Path Of Exile |
| **Turn-in directory** | unityModule00 |
| **Required elements** | A FloorIsLava scene, PlayerController script and any relevant elements |
| **Forbidden functions** | None |

### Objective

Now that you've got your structure and your player, it's time to make them move along the path.

### Implementation

#### Player Movement Script

- Create a script named **PlayerController.cs**
- Attach it to your player GameObject
- The player should be able to move using the **WASD** keys ('ZSQD', depending on your keyboard) or the **arrow keys**
- Both options should work

#### Jumping Mechanic

- Your player should also be able to jump
- Place some obstacles along your pathway that the player will need to jump over
- Implement jumping in your **PlayerController** script

---

## Chapter VI: Exercise 02: My Even More Beautiful World

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | Exercise 02: My Even More Beautiful World |
| **Turn-in directory** | unityModule00 |
| **Required elements** | A FloorIsLava scene and any relevant elements |
| **Forbidden functions** | None |

### Resources

You can find the texture pack needed for this exercise on the **[Official Unity Asset Store](https://assetstore.unity.com/)**.

### Objective

Right now, your scene is looking a bit dull. Let's fix that by adding some texture and life to it using assets from the Unity Asset Store.

### Implementation

- Make your floor look like lava
- Your pathway can look like stone or other materials
- Add some leafy vegetation as obstacles or decorations
- Let your imagination run wild, but don't spend too much time on it either

---

## Chapter VII: Exercise 03: The Floor Is 'Always' Lava

### Exercise Information

| Field | Value |
|-------|-------|
| **Name** | Exercise 03: The Floor Is 'Always' Lava |
| **Turn-in directory** | unityModule00 |
| **Required elements** | A FloorIsLava scene file, the assets and scripts specific to the exercise |
| **Forbidden functions** | None |

### Objective

Now we get to the heart of the matter, and the end of it too.

### Game Over Logic

The floor is still lava!

So you'll need to make sure that if your player falls off the pathway, it's game over.

**Requirements:**

- For now, you don't need a dramatic title screen or fancy effects
- Just a simple `Debug.Log` that displays "Game Over" in the console will do
- The Player GameObject must be destroyed when the game is over

---

## Chapter VIII: Submission and Peer Evaluation

### Submission Instructions

Submit your assignment in your Git repository as usual. Only the work inside your repository will be evaluated during the defense. Don't hesitate to double-check the names of your folders and files to make sure everything is correct.

### Important: Git and Unity

⚠️ **Critical:**

You should **NOT** upload the entire Unity project to Git, as this can unnecessarily increase the size of your repository.

**To optimize your repository:**

- Make sure Unity saves as many files as possible in **text format** rather than binary
  - In Unity, go to: **Edit > Project Settings > Editor**
  - Under **Asset Serialization**, set it to **Force Text**

- Ensure that the **.gitignore** file automatically generated by Unity is present

### Evaluation

ℹ️ **Important:**

The evaluation will take place on the computer of the learner or group being evaluated.

---

## Project Structure

```
unityModule00/
├── Assets/
│   ├── Scenes/
│   │   └── FloorIsLavaScene.unity
│   ├── Scripts/
│   │   └── PlayerController.cs
│   └── Materials/
│       └── (textures and materials)
├── ProjectSettings/
└── .gitignore
```

## Key Learning Outcomes

By completing this module, you will learn:

1. **Unity Fundamentals:**
   - Creating and managing 3D scenes
   - Working with GameObjects and primitives
   - Using the Inspector and Hierarchy
   - Camera positioning and management

2. **Game Development Basics:**
   - Player movement mechanics (WASD/Arrow keys)
   - Jumping and collision detection
   - Game-over logic
   - Physics and rigidbodies

3. **C# Scripting:**
   - Creating and attaching scripts to GameObjects
   - Input handling
   - Object destruction
   - Debug logging

4. **Level Design:**
   - Creating pathways and obstacles
   - Spatial layout and difficulty progression
   - Visual design with materials and colors

5. **Best Practices:**
   - Version control with Git
   - Project optimization
   - Asset management
   - Code organization

---

## Requirements Summary

### Exercise 00: Build the World
✓ Create 3D scene with Floor, Pathway, Player (ball), Decorations, Camera

### Exercise 01: Add Interactivity
✓ PlayerController script with WASD/Arrow key movement
✓ Jumping mechanics
✓ Obstacles to jump over

### Exercise 02: Polish the Visuals
✓ Add textures and materials from Asset Store
✓ Make the scene visually appealing
✓ Lava-themed floor, stone pathway

### Exercise 03: Implement Game-Over
✓ Detect when player falls off pathway
✓ Log "Game Over" to console
✓ Destroy Player GameObject

---

**Last Updated:** Version 2
**Framework:** Unity 3D
**Language:** C#
**Genre:** 3D Platformer / Obstacle Course
