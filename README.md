# Deadline Catcher

A 3D endless runner built in Python with PyOpenGL and GLUT. Guide the player across three lanes, dodge trains and barriers, and use temporary power-ups to keep a run going. This is an individual computer graphics project by **Zannaty Aziza**.

## Features

- Three-lane movement with jumping, sliding, collision detection, and a score counter.
- Procedurally generated obstacle rows with a safe-lane planner.
- Power-ups including Super Sneakers, invincibility, lane collapse, and a jetpack.
- Hoverboards that can be activated during a run.
- Character color customization, a moving camera, day/night changes, and rain effects.
- Loading, customization, ready, play, pause, and game-over screens.

## Run locally

Install Python and a working OpenGL/GLUT runtime, then install the Python dependency:

```bash
python -m pip install -r requirements.txt
python cse423_project.py
```

PyOpenGL provides the Python bindings; a GLUT or FreeGLUT implementation must also be available on the computer. See the [PyOpenGL installation guide](https://pyopengl.sourceforge.net/documentation/installation.html) if the GLUT library is missing.

## Controls

| Key or action | Effect |
| --- | --- |
| Mouse click | Choose shirt, pants, and hoverboard colors on the customization screen |
| `O` | Finish customization and enter the ready screen |
| `P` | Start the game; pause or resume during play |
| `A` / `D` | Move left / right |
| `Space` | Jump |
| `S` | Slide |
| `H` | Activate a hoverboard if one is available |
| Arrow keys | Adjust the camera position |
| `R` | Restart |

The game opens with a short loading screen before customization. Press `O`, then `P` to begin a run.

## Project structure

The game is implemented in [`cse423_project.py`](cse423_project.py). It contains the game state, obstacle spawning, physics and collision checks, rendering, and GLUT input callbacks. [`requirements.txt`](requirements.txt) lists the Python dependency.

## Status

The source has been checked for Python syntax. The game requires a graphical OpenGL/GLUT environment to run; this repository does not include a gameplay screenshot yet.
