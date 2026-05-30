# Gravity Leap - DevLog #1

<img width="1376" height="768" alt="Gemini_Generated_Image_d7k5c9d7k5c9d7k5" src="https://github.com/user-attachments/assets/2ae9394c-c439-4deb-ac8a-d3560ee9f973" />

I am developing a new 2D platformer computer game as part of a computer game development course in Unity, within my Visual Communication studies.

The game tells the story of an astronaut who went on a routine mission and, following an unexpected malfunction in the spacecraft, was hit by the blast of an explosion and fell onto a nearby unidentified planet, rocky and isolated. Now, as his oxygen supply is running out, he must utilize the asteroid surfaces floating in the planet's sky on his way back to his escape pod.

Along the way, he will encounter varying gravity forces, black holes that will teleport him from place to place, and in advanced stages, he will have to deal with the aliens who control the area.!


---------------------------------




<a name="devlog-2"></a>
## Gravity Leap - DevLog #2 - making moves

Now that the visual foundation is set, it was time to breathe life into our astronaut. This week was all about transition: moving from a static design in Figma/Photoshop to a playable character in Unity.

The Physics of Space
The first challenge was gravity. In a game called Gravity Leap, the jump needs to feel just right. I spent a lot of time tweaking the Rigidbody 2D settings and writing C# scripts to ensure the movement feels responsive.

I implemented a classic platformer controller where the player can:

Move horizontally using the arrow keys.

Leap between asteroids with physics-based jumping.

Maintain upright posture using rotation constraints (no accidental astronaut somersaults... yet!).

From Pixels to Platforms
One of the most satisfying moments was replacing the placeholder "white boxes" with my custom-designed assets. Seeing the astronaut standing on a hand-drawn asteroid for the first time made the project feel real.

I also learned a crucial lesson about Colliders: a character only looks like they are standing on a surface if the physical boundaries match the visual edges. I spent some time "tightening" the hitboxes so that the landing feels solid and precise.

Setting the Scene
To complete the "Lost in Space" vibe, I integrated a deep-space nebula background. By managing the Sorting Layers, I made sure our hero stays in the spotlight while the galaxy swirls realistically behind him.

What’s next? In the next update, I’ll be diving into the "Gravity Forces" mentioned in the story—looking at how to make different asteroids have different pull strengths.


## Gravity Leap - DevLog #3 - Jumping and Flipping

https://github.com/user-attachments/assets/59e50c69-5942-4ae8-a5bb-286b792a8881


Implemented Character Movement, Jumping, and Flipping System
Refactored the core script structure into a clean and functional CharacterController2D along with a separate PlayerMovement script to handle input. Resolved physics issues causing the character to hover by adjusting colliders and configured linearVelocity to ensure crisp, responsive movement. Additionally, implemented a fully functional flipping logic (transform.Rotate) using 180-degree rotations to prevent sprite distortion, fixed the jump detection using an optimized GroundCheck system, and prepared the structural foundation for crouch mechanics.
