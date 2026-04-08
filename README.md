# Rocket Game

A 2D OpenGL/GLUT shooting game built in C++. Shoot incoming enemy rockets from the bottom of the screen before the timer runs out.

**Author:** Arda Saritas  
**Course:** CTIS164 Section 01

## Demo 

https://github.com/user-attachments/assets/f8b86542-3f4c-4ebb-be42-b85a9a297f92

## Gameplay

Five enemy rockets fly across the screen from left to right. You control a turret at the bottom and fire a projectile upward to intercept them. Points are awarded based on how close to the center of the rocket you hit.

### Scoring

| Hit Accuracy | Points |
|---|---|
| Near center (distance ≤ 60) | 5 pts |
| Middle ring (distance 60–70) | 3 pts |
| Outer edge (distance 70–75) | 1 pt |

Earn **20+ points** before the timer expires to activate **Streak Mode** — the projectile speed increases.

### HUD

The top bar displays:
- Remaining time
- Total rockets passed
- Rockets burst (hit)
- Last hit point value
- Total points

## Controls

| Key | Action |
|---|---|
| `SPACE` | Fire projectile |
| `←` / `→` | Move turret left/right |
| `F1` | Pause / Resume; restart after game over |
| `ESC` | Quit |

## Building

Requires macOS with Xcode and the GLUT/OpenGL frameworks (included in the Xcode project).

Open `rocket-game.xcodeproj` in Xcode and build with `Cmd+B`, or run from the scheme selector.

## Project Structure

```
rocket-game/
├── rocket-game/
│   └── main.cpp          # All game logic and rendering
└── rocket-game.xcodeproj # Xcode project
```
