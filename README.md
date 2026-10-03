# CS464 - Lab 04: Player Controller & Greybox Arena

**Student:** Muhammad Tayyab  
**Roll Number:** BSSE23018  

---

## Overview
A 3D physics-based character controller and greybox test level developed in Unity 6 (URP). The project demonstrates Rigidbody movement, reliable ground detection, and an obstacle course designed for testing player traversal.

---

## Controls
| Action | Key / Input |
| :--- | :--- |
| **Move** | `W` / `A` / `S` / `D` or Arrow Keys |
| **Jump** | `Spacebar` |

---

## Key Features & Scripts

- **Player Controller (`PlayerController.cs`):**
  - Horizontal movement using `Rigidbody.linearVelocity`.
  - Reliable ground check using `Physics.OverlapSphereNonAlloc` with self-collider filtering to prevent mid-air double jumps.
  - Mass-independent jump force using `ForceMode.VelocityChange`.

- **Follow Camera (`FollowCamera.cs`):**
  - Smooth third-person camera following the player capsule.

- **Greybox Obstacle Course:**
  - **Hurdles:** Low barriers to test jump height and clearance.
  - **Ramp & High Deck:** Sloped incline to test movement on angled surfaces.
  - **Stairs:** Ascending blocks to test stepping and gravity.
  - **Parkour Pads:** Floating platforms to test jump timing and distance.
  - **Slalom Pillars:** Zigzag obstacles to test turning responsiveness.
  - **Perimeter Walls:** Boundary barriers keeping the player inside the arena.