# Arkanoid Game 🎮

A fully-functional, object-oriented Arkanoid (brick breaker) game written in Java.  
Built as a university assignment to demonstrate principles of game design, geometry, collision detection, and clean OOP architecture.

---

## 🧠 About the Game

Arkanoid is a classic arcade game in which a player controls a paddle to bounce a ball and break blocks.  
The game ends when all blocks are destroyed or the player loses all the balls.

---

## 🛠️ Features

- 🎮 Real-time game loop (60 FPS) with keyboard controls
- 🧱 Dynamic collision detection (ball ↔ blocks/paddle/walls)
- 🎯 Score tracking and event-based block removal
- 🧩 Modular architecture using:
  - `Sprite` and `Collidable` interfaces
  - `Listener` pattern for event handling
- 🎨 Paddle, balls, score area, and death zone

---

## 🧩 Class Structure Overview

### Core Game Engine
- `Game.java`: Initializes and runs the game loop
- `Ass5Game.java`: Entry point

### Geometry & Physics
- `Point`, `Line`, `Rectangle`, `Velocity`: Math for movement and collision

### Game Objects
- `Ball`, `Block`, `Paddle`: Visual and physical game objects
- `Collidable`, `Sprite`, `CollisionInfo`: Interfaces and abstractions

### Listeners
- `HitListener`, `BlockRemover`, `BallRemover`, `ScoreTrackingListener`: Handle game events cleanly

---

## 🚀 How to Run

### Requirements:
- Java 11+
- [biuoop-1.4.jar](https://github.com/arieh/biuoop) (already included)

### 🧭 Instructions (Windows CMD)

Open a terminal and navigate to the `src` folder:
   ```cmd
   cd Arkanoid-Game-main\Ass5.java\src

Compile the source code:
    ```cmd
    javac -cp ..\..\biuoop-1.4.jar game\*.java geometry\*.java listeners\*.java sprites\*.java

Run the game:
    ```cmd
    java -cp .;..\..\biuoop-1.4.jar game.Ass5Game

⚠️ Use ; as the classpath separator on Windows.
If you're using Git Bash, Mac, or Linux, use : instead of ;.
