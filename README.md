# SnowBoarder-2D-Game
SnowBoarder 2D game; Cinemachine, Surface Effector 2D, Triggers, SceneManagement etc.


# Game Mechanics We Need
    1. Move along the track
    2. Rotate forwards and backwards
    3. Ability to speed up
    4. Particle effects that only play when we’re touching ground 
    5. Finish line that restarts level
    6. Crash detection which restarts the level

<img width="573" alt="SnowBoarder1" src="https://user-images.githubusercontent.com/23366804/174950914-ede96cbb-fccf-4244-b47d-7c60fb05bcb2.png">

# Game Design
    1. Player Experience: Smooth, relaxing
    2. Core Mechanic: Don’t crash
    3. Game Loop:Reach the end to win

# What Is Cinemachine?
Cinemachine is a powerful package that lets us:
    1. manage multiple cameras in our scene
    2. Easily create rules for our cameras

<img width="573" alt="SnowBoarder2" src="https://user-images.githubusercontent.com/23366804/174950918-2c38baa4-f9ca-45d8-b99f-51e1bea41a8d.png">

# Organising Code
The more code we have, the higher likelihood of conflicts between names and behaviours. Especially on multi-person projects.
Eg. Programmer 1 working on player uses “Movement” method but Programmer 2 working on enemy also uses “Movement” method. 
So in C# our code is grouped with a particular structure to reduce conflicts.

# What Are Namespaces?
    - We use Namespaces to group together similar Classes of code (and Classes are containers for methods and variables).
    - If we want to use a particular Class then we need to tell Unity which Namespace it belongs to with the using keyword.

# SceneManagement Namespace
    - We’re going to use classes and methods from the SceneManagement namespace
    - Pre-built functionality to help us load scenes

# Creating A Delay
There are 2 useful approaches to “waiting a moment”.
    a. Invoke
    b. Coroutines
Invoke is a bit easier to understand but not as powerful. 
It also uses string reference which are clumsy.

<img width="573" alt="SnowBoarder3" src="https://user-images.githubusercontent.com/23366804/174950946-440872c2-d253-4e39-8547-449ed8a624f8.png">

# Important To Tune Now And Then
Keep your game “*playable*” as much as possible
Improve the look and feel of your on regular basis
This helps:
- Keep you motivated
- Show your game and get feedback
- Generate ideas for improving your game

# Audio Terminology
    *Audio Listener* - like a microphone, receives sounds and plays through your computer’s speakers
    *Audio Source* - Plays audio and allows us to adjust settings (eg. volume)
    *Audio Clip* - Contains the audio data to be played (mp3, Wav, OGG)
