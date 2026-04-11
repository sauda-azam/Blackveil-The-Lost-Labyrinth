# Blackveil: The Lost Labyrinth

## Game Description

**Blackveil: The Lost Labyrinth** is a 2D action-adventure puzzle platformer created using the **iGraphics** library in C/C++. The game follows a lone explorer venturing into a mysterious, ever-shifting labyrinth — battling fearsome bosses, collecting powerful items, and solving six unique puzzles to escape. The project demonstrates advanced graphics programming concepts including physics-based platforming, sprite animation, collision detection, procedural level generation, and multi-state puzzle systems.

---

## Features

- 3 progressively difficult levels with procedurally generated platformer stages
- 6 unique hand-crafted puzzle rooms:
  - 🔲 **Box Sequence Puzzle** — Activate boxes in the correct order before time runs out
  - 🪵 **Bridge Building Puzzle** — Place color-coded planks and power boxes to rebuild a broken bridge
  - 🧊 **Ice Slider Puzzle** — Slide across ice and navigate around obstacles to reach the treasure
  - 🔦 **Mirror Laser Puzzle** — Rotate mirrors and aim a laser through a chain of targets
  - 🧮 **Stick Math Puzzle** — Solve a math problem, then find the correct glowing stick
  - ⚙️ **Aether-Flow Puzzle** — Turn a valve, stabilize a bridge, and escape before acid rises
- Multiple boss types with unique run and attack animations
- Collectibles system: ❤️ hearts, 🪙 coins, and a 🗺️ map item
- Moving platforms — horizontal (Level 2) and horizontal + vertical (Level 3)
- Coyote time and jump buffering for responsive platformer feel
- Dynamic background music and sound effects per game state
- Intro and outro cinematic cutscenes with narrative storytelling
- Persistent health and coin count across all stages
- Full HUD with health display, coin counter, and key indicator

---

## Project Details

| Field        | Details                        |
|-------------|-------------------------------|
| **IDE**      | Visual Studio 2013             |
| **Language** | C / C++                        |
| **Platform** | Windows PC                     |
| **Genre**    | 2D Action Adventure / Puzzle Platformer |
| **Library**  | iGraphics (OpenGL/GLUT-based)  |

---

## How to Run the Project

Make sure you have the following installed:

- **Visual Studio 2013**
- **iGraphics Library** (included in this repository)
- **Windows Multimedia Library** — `winmm.lib` (linked automatically via `#pragma comment`)

### Steps

1. Clone or download this repository
2. Open **Visual Studio 2013**
3. Go to **File → Open → Project/Solution**
4. Locate and select the `.sln` file from the repository
5. Click **Build → Build Solution**
6. Run via **Debug → Start Without Debugging**

> ⚠️ Make sure the `images\`, `Images\`, and `sounds\` asset folders are placed in the same directory as the compiled executable. Without them, the game will not display correctly.

---

## How to Play

### Main Controls

| Action                        | Key                        |
|------------------------------|---------------------------|
| Move Left / Right             | `A` / `D`                 |
| Jump                          | `Space`                   |
| Attack Boss                   | `F`                       |
| Interact / Collect / Inspect  | `E`                       |
| Drop Held Item (Puzzles)      | `Q`                       |
| Close Puzzle Overlay          | `B`                       |
| Enter Room / Confirm          | `Enter`                   |
| Restart Current State         | `Backspace`               |

---

### Puzzle-Specific Controls

| Puzzle                  | Controls                                                                 |
|------------------------|-------------------------------------------------------------------------|
| **Box Sequence**        | WASD / Arrow Keys to move · `Space` to activate boxes · `E` to inspect  |
| **Bridge Building**     | WASD to move · `E` to pick up items · `Q` to drop/place                 |
| **Ice Slider**          | WASD / Arrow Keys — player slides until hitting a wall or boundary      |
| **Mirror Laser**        | WASD to move · Left-click mirrors to rotate · Hold Left Mouse to aim    |
| **Stick Math**          | Type your answer and press `Enter`, then WASD to navigate and `Space` to collect the correct stick |
| **Aether-Flow**         | `A` / `D` to move · `Space` to jump · `E` to interact with valve & door |

---

### Game Rules

- Player starts with **3 health points** (maximum of 5)
- Falling off platforms or taking boss damage reduces health
- Reaching 0 health returns you to the main menu
- Collect **❤️ hearts** to restore health
- Collect **🪙 coins** to increase your score
- Collect the **🗺️ map** to unlock the puzzle world
- Complete all puzzles and defeat all bosses to escape the Labyrinth

---

### Debug / Level Skip Keys

> These keys are available for testing and skipping to specific stages:

| Key         | Action                                      |
|------------|---------------------------------------------|
| `1`         | Jump to Level 1 platformer                  |
| `2`         | Jump to Level 2 platformer                  |
| `3`         | Jump to Level 3 platformer                  |
| `6`         | Jump to Box Puzzle (inside room)            |
| `7`         | Jump to Bridge Building Puzzle              |
| `8`         | Jump to Ice Slider Puzzle                   |
| `9`         | Jump to Mirror Laser Puzzle                 |
| `0`         | Jump to Aether-Flow Puzzle                  |
| `Backspace` | Restart current state                       |

---

## Game Flow

```
Main Menu
   └── Level 1  (15 platformer stages · 3 bosses)
         └── Outside Puzzle Area  (map collectible unlocks this)
               └── Box Sequence Puzzle  (timed, inside room)
                     └── Bridge Building Puzzle
                           └── Level 2  (12 stages · bosses · moving platforms)
                                 ├── Ice Slider Puzzle  (after stage 2)
                                 ├── Bridge Puzzle Phase 2  (after stage 5)
                                 └── Mirror Laser Puzzle  (end of Level 2)
                                       └── Level 3  (16 stages · bosses · dynamic platforms)
                                             ├── Stick Math Puzzle  (after first boss)
                                             └── Aether-Flow Puzzle  (final puzzle)
                                                   └── Outro Cutscene → Main Menu
```

---

## Screenshots

### Menu

" width="400" height="250">

### Gameplay
<img src="" width="400" height="250">

---

## Project Contributors

| Name    |
|--------|
| Sauda  |
| Nuha|
| Rabeta |

---

## YouTube Link

[▶ Blackveil: The Lost Labyrinth — Gameplay Video]()

---

## Project Report

[📄 Project Report: Blackveil: The Lost Labyrinth]()
