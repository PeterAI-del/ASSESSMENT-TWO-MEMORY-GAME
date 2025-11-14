# Memory Match Game

**Project Type:** Python Game  
**Version:** Text-based (Console) & GUI (Tkinter)  
**Assessment:** Assessment Two, Keele University Python Course

---

## Description

This is a **Memory Match Game** implemented in Python.  

- Players try to find all matching pairs of cards.  
- The repository contains both:  
  - **Console version** – text-based, simple gameplay.  
  - **GUI version** – enhanced interface with visual effects, timer, restart button, and adjustable grid sizes (4×4, 6×6).  

The GUI version is developed in a separate branch (`gui-gameplay-enhancements`) for improved usability and visual experience.

---

## Features

---

### Console Version
- Text-based interface  
- Supports 4×4 and 6×6 grids  
- Tracks player **attempts** and **time elapsed**  
- Color-coded matched cards  

### GUI Version (Tkinter)
- Supports 4×4 and 6×6 grids  
- **Restart button** to reset the game without closing the window  
- **Timer** to track how fast the player finishes  
- **Scoreboard**: attempts and time  
- **Color-coded matched cards**  
- **Hover effects** on buttons  
- Dynamic font and button scaling  

---

## 🛠 Dependencies (Added dependency instructions.)


- Python 3.x  
- Tkinter (usually included with Python, otherwise install via `pip install tk`)  
- Standard Python libraries: `random`, `time`, `messagebox` from `tkinter`  

---

## Game Play Instructions

1. When the game starts, a board of hidden cards is displayed.  
2. Each turn, the player selects **two cards** to reveal.  
3. If the cards match, they remain revealed.  
4. If the cards do not match, they are hidden again.  
5. The goal is to reveal all pairs in as few turns as possible.  
6. The game ends when all pairs are found; attempts and elapsed time are displayed.  

### Example Board Layout (There's also a 6x6 grid) and the concept is the same
  1  2  3   4
A [] [] [] []
B [] [] [] []
C [] [] [] []
D [] [] [] []

- `[*]` represents a hidden card  
- Players select cards by row and column (e.g., `A1` and `B3`)  
- Matching cards are revealed as their letter/number pair  

---

## Installation & Usage

1. Clone the repository:

```bash
git clone https://github.com/PeterAI-del/ASSESSMENT-TWO-MEMORY-GAME.git

2. Navigate to the Folder using
cd ASSESSMENT-TWO-MEMORY-GAME

3. Run the game
python MemoryMatchGame/memory_game_console.py

4. Run the GUI
python MemoryMatchGame/memory_game_tk.py

### Example Turn

1. Player selects `A1` and `B3`:

   1  2  3  4
A [X] [] [] []
B [] [] [O] []
C [] [] [] []
D [] [] [] []  


- `X` and `O` are the revealed cards  
- If they match, they stay revealed: `[X] [*] [*] [*]`  
- If they do not match, they are hidden again in the next turn: `[*] [*] [*] [*]`  
