# Testing Cases
## Project Title: Galaxy Defender

---

## Test Case 1: Game Loads Successfully
- **Test ID:** TC-01
- **Objective:** Verify that the game opens correctly in the browser
- **Input:** Open `index.html`
- **Expected Result:** Game screen loads successfully with player spaceship, score, and lives visible

---

## Test Case 2: Player Moves Left
- **Test ID:** TC-02
- **Objective:** Verify left movement of spaceship
- **Input:** Press Left Arrow key
- **Expected Result:** Player spaceship moves left within game boundary

---

## Test Case 3: Player Moves Right
- **Test ID:** TC-03
- **Objective:** Verify right movement of spaceship
- **Input:** Press Right Arrow key
- **Expected Result:** Player spaceship moves right within game boundary

---

## Test Case 4: Player Cannot Move Outside Left Boundary
- **Test ID:** TC-04
- **Objective:** Ensure spaceship does not leave the left side of game area
- **Input:** Hold Left Arrow key at left edge
- **Expected Result:** Spaceship stops at left boundary and does not move outside the screen

---

## Test Case 5: Player Cannot Move Outside Right Boundary
- **Test ID:** TC-05
- **Objective:** Ensure spaceship does not leave the right side of game area
- **Input:** Hold Right Arrow key at right edge
- **Expected Result:** Spaceship stops at right boundary and does not move outside the screen

---

## Test Case 6: Bullet Shoots Correctly
- **Test ID:** TC-06
- **Objective:** Verify bullet firing mechanism
- **Input:** Press Spacebar
- **Expected Result:** Bullet is created at spaceship position and moves upward

---

## Test Case 7: Enemy Ships Spawn Correctly
- **Test ID:** TC-07
- **Objective:** Verify enemy generation
- **Input:** Start game and wait
- **Expected Result:** Enemy ships appear from the top at regular intervals

---

## Test Case 8: Enemy Ships Move Downward
- **Test ID:** TC-08
- **Objective:** Verify enemy movement
- **Input:** Observe spawned enemies
- **Expected Result:** Enemy ships move downward toward the player

---

## Test Case 9: Bullet Hits Enemy
- **Test ID:** TC-09
- **Objective:** Verify collision between bullet and enemy
- **Input:** Shoot bullet at enemy ship
- **Expected Result:** Enemy ship disappears and bullet is removed

---

## Test Case 10: Score Increases on Enemy Destruction
- **Test ID:** TC-10
- **Objective:** Verify score update
- **Input:** Destroy one enemy ship
- **Expected Result:** Score increases by the defined value

---

## Test Case 11: Enemy Collides with Player
- **Test ID:** TC-11
- **Objective:** Verify collision between enemy and player
- **Input:** Allow enemy ship to hit player spaceship
- **Expected Result:** Player loses one life

---

## Test Case 12: Lives Decrease Correctly
- **Test ID:** TC-12
- **Objective:** Verify lives system
- **Input:** Multiple enemy collisions with player
- **Expected Result:** Lives decrease one by one until zero

---

## Test Case 13: Game Over Trigger
- **Test ID:** TC-13
- **Objective:** Verify game over condition
- **Input:** Lose all player lives
- **Expected Result:** Game Over message is displayed and gameplay stops

---

## Test Case 14: Restart Game Works
- **Test ID:** TC-14
- **Objective:** Verify restart functionality
- **Input:** Click Restart button after Game Over
- **Expected Result:** Game resets score, lives, player position, and enemy list

---

## Test Case 15: Game Runs Smoothly
- **Test ID:** TC-15
- **Objective:** Verify performance under normal gameplay
- **Input:** Play continuously for a few minutes
- **Expected Result:** Game runs without lag or crash in a modern browser

---

## Summary
The above test cases verify the core gameplay functionality, movement, shooting, enemy behavior, collision detection, score handling, life management, game over condition, and restart functionality of the Galaxy Defender project.
