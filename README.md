######################################################################
##           Race Challenge (Gyrosphere-style OpenGL Game)          ##
######################################################################

## Author
Mai Waheed AbbdelGhany


A 3D two-player racing game built using **OpenGL** and **FreeGLUT**, featuring multiple game modes, dynamic tracks, smooth camera-following, checkpoint-based scoring, and a GUI-based start menu.

---

## 🎮 Features

- **Single Player and Multiplayer support**
- **Four Game Modes**:
  - 🧍 Single Player
  - 🏁 Race (Reach the end with 40+ points)
  - ⏱️ Timed Score Attack (Score the most points in 2 minutes)
  - 💰 Treasure Hunt (Collect hidden treasures before time runs out)
- Split-screen support for multiplayer
- Floating HUD text and score updates
- Dynamic directional arrows and track generation
- Health, lives, and pickups
- Visual end screen with scores and replay option

---

## Tech Stack

- **C++**
- **OpenGL**
- **FreeGLUT**
- **GLU**
- **STB Image** for loading textures (e.g. heart icons)

---

## 📁 File Structure

| File | Description |
|------|-------------|
| `main.cpp` | Core gameplay logic, physics, rendering, player management |
| `screen.cpp` | Menu system: game mode selection, name input, color selection |
| `stb_image.h` | Image loader for OpenGL textures (must be in the same directory) |
| `heart.png` | Texture used for displaying player lives |

---

## 🕹️ Controls

### Player 1
- `W/A/S/D`: Move
- `Enter`: Confirm
- `Backspace`: Delete character (in name input)

### Player 2
- Arrow keys: Move
- `Enter`: Confirm
- `Esc`: Back


### 🧱 Prerequisites

- C++ compiler (e.g. g++)
- OpenGL, FreeGLUT libraries installed

### Compilation (Linux/macOS)
```bash
g++ main.cpp -o main -lGL -lGLU -lglut
g++ screen.cpp -o screen -lGL -lGLU -lglut
