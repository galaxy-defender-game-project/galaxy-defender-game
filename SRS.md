# Software Requirements Specification (SRS)
## Project Title: Galaxy Defender

---

## 1. Introduction

### 1.1 Purpose
The purpose of this project is to develop a simple 2D browser-based space shooter game called **Galaxy Defender**. The game allows the player to control a spaceship, shoot enemy villain ships, avoid collisions, and score points. This project is developed as part of a software engineering academic project to demonstrate the application of game logic, user interaction, modular design, and frontend development concepts.

### 1.2 Scope
Galaxy Defender is a browser-based arcade shooting game built using **HTML, CSS, and JavaScript**. The player controls a spaceship positioned at the bottom of the screen and must destroy enemy ships descending from the top of the screen. The game includes movement controls, shooting mechanics, enemy generation, collision detection, score tracking, lives system, and game over functionality.

### 1.3 Definitions, Acronyms, and Abbreviations
- **SRS** – Software Requirements Specification  
- **UI** – User Interface  
- **HTML** – HyperText Markup Language  
- **CSS** – Cascading Style Sheets  
- **JS** – JavaScript  
- **Game Loop** – The repeated cycle of updating and rendering game elements  
- **Collision Detection** – Logic used to check when two game objects touch each other  

### 1.4 References
- HTML Documentation  
- CSS Documentation  
- JavaScript Documentation  
- Browser-based game development concepts  
- Software Engineering project guidelines  

### 1.5 Overview
This document describes the functional and non-functional requirements of the Galaxy Defender project. It explains the system behavior, user interactions, software requirements, and constraints needed to develop the game successfully.

---

## 2. Overall Description

### 2.1 Product Perspective
Galaxy Defender is a standalone browser game that runs locally in a web browser without requiring server-side processing or database connectivity. It is a frontend-based project focused on user interaction and gameplay mechanics.

### 2.2 Product Functions
The main functions of the Galaxy Defender game are:
- Display the game screen and interface
- Allow player spaceship movement
- Allow the player to shoot bullets
- Generate enemy villain ships
- Move enemies downward continuously
- Detect collisions between bullets and enemies
- Detect collisions between enemies and player
- Update score when enemies are destroyed
- Reduce player lives on collision
- End the game when all lives are lost
- Provide a restart option after game over

### 2.3 User Classes and Characteristics
The main users of this system are:
- Students
- Teachers / Evaluators
- Casual players

Characteristics of users:
- Basic computer and keyboard knowledge
- Ability to use arrow keys and spacebar
- Familiarity with browser-based applications

### 2.4 Operating Environment
The game will run in the following environment:
- Operating System: Windows / macOS / Linux
- Browser: Google Chrome, Mozilla Firefox, Microsoft Edge
- Technologies: HTML, CSS, JavaScript
- No internet connection required after downloading the files

### 2.5 Design and Implementation Constraints
- The game is limited to browser-based execution only
- No backend or database is used
- Game assets such as images and sounds must be lightweight
- The project should remain simple and easy to understand for academic evaluation
- The interface should be responsive enough for standard desktop screens

### 2.6 Assumptions and Dependencies
- The user has access to a modern web browser
- Keyboard controls are available
- JavaScript is enabled in the browser
- Required game files are stored in the correct project structure

---

## 3. Specific Requirements

### 3.1 Functional Requirements

#### 3.1.1 Game Start
- The system shall display the game interface when `index.html` is opened.
- The system shall initialize the player spaceship, score, and lives at the start of the game.

#### 3.1.2 Player Movement
- The system shall allow the player spaceship to move left using the Left Arrow key.
- The system shall allow the player spaceship to move right using the Right Arrow key.
- The system shall restrict the player from moving outside the game boundary.

#### 3.1.3 Bullet Shooting
- The system shall allow the player to shoot bullets using the Spacebar key.
- The system shall create bullets from the player spaceship position.
- The system shall move bullets upward on the screen.

#### 3.1.4 Enemy Generation
- The system shall generate enemy villain ships at random horizontal positions.
- The system shall continuously spawn enemy ships from the top of the screen.
- The system shall move enemy ships downward toward the player.

#### 3.1.5 Collision Detection
- The system shall detect collision between bullets and enemy ships.
- The system shall remove the enemy ship when hit by a bullet.
- The system shall remove or reset the bullet after collision.
- The system shall detect collision between enemy ships and the player spaceship.

#### 3.1.6 Score System
- The system shall increase the score whenever an enemy ship is destroyed.
- The system shall display the updated score in real time.

#### 3.1.7 Lives / Health System
- The system shall assign a fixed number of lives to the player at the beginning.
- The system shall reduce one life when an enemy collides with the player.
- The system shall display remaining lives on the screen.

#### 3.1.8 Game Over
- The system shall end the game when all player lives are lost.
- The system shall display a game over message.
- The system shall stop enemy movement and player actions after game over.

#### 3.1.9 Restart Functionality
- The system shall provide a restart option after game over.
- The system shall reset score, lives, enemies, and player position when the game restarts.

---

## 4. Non-Functional Requirements

### 4.1 Performance Requirements
- The game should load within a few seconds in a standard browser.
- The game should run smoothly without noticeable lag on normal desktop systems.
- Player movement and shooting should respond instantly to keyboard input.

### 4.2 Usability Requirements
- The user interface should be simple and easy to understand.
- Controls should be clearly defined and easy to use.
- The score and lives display should be visible during gameplay.

### 4.3 Reliability Requirements
- The game should run without crashing under normal use.
- Game restart should properly reset all values.
- Collision detection should work consistently.

### 4.4 Maintainability Requirements
- The code should be modular and separated into logical files.
- The project structure should be easy to understand for future updates.
- Additional features like boss levels and power-ups should be easy to add later.

### 4.5 Portability Requirements
- The game should work on any modern browser.
- The project should be portable by simply copying the project folder to another system.

---

## 5. External Interface Requirements

### 5.1 User Interface Requirements
- The game screen shall include:
  - Background (space theme)
  - Player spaceship
  - Enemy ships
  - Score display
  - Lives display
  - Game over message
  - Restart button

### 5.2 Hardware Interface Requirements
- Keyboard is required for gameplay controls.
- Display monitor is required for visual output.

### 5.3 Software Interface Requirements
- The system requires a web browser that supports HTML, CSS, and JavaScript.

### 5.4 Communication Interface Requirements
- No communication interface is required because the project runs locally without networking.

---

## 6. System Requirements

### 6.1 Minimum Hardware Requirements
- Processor: Dual-core CPU
- RAM: 2 GB or higher
- Keyboard
- Monitor / Display

### 6.2 Minimum Software Requirements
- Operating System: Windows 10/11, macOS, or Linux
- Browser: Google Chrome / Mozilla Firefox / Microsoft Edge
- Code Editor (optional for development): VS Code or any text editor

---

## 7. Use Case Summary

### 7.1 Use Case: Start Game
- **Actor:** Player
- **Description:** Player opens the game in a browser and starts playing.
- **Outcome:** Game interface loads successfully.

### 7.2 Use Case: Move Spaceship
- **Actor:** Player
- **Description:** Player presses arrow keys to move the spaceship.
- **Outcome:** Spaceship moves left or right.

### 7.3 Use Case: Shoot Enemy
- **Actor:** Player
- **Description:** Player presses Spacebar to fire bullets.
- **Outcome:** Bullet moves upward and can destroy enemy ships.

### 7.4 Use Case: Game Over
- **Actor:** System / Player
- **Description:** Player loses all lives due to enemy collisions.
- **Outcome:** Game ends and game over screen is displayed.

### 7.5 Use Case: Restart Game
- **Actor:** Player
- **Description:** Player clicks restart after game over.
- **Outcome:** Game resets and starts again.

---

## 8. Future Enhancements
- Boss enemy ship
- Power-up items
- Shield system
- Multiple levels
- Background music and sound effects
- High score / leaderboard system
- Pause and resume functionality

---

## 9. Conclusion
Galaxy Defender is a simple and interactive 2D browser-based shooting game designed for academic purposes. The project demonstrates the use of software engineering principles such as modular development, requirement analysis, user interaction, functional decomposition, and testing preparation. This SRS document provides the complete requirement specification needed for the successful development of the project.

---
