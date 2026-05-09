# Maze Solver

A Python program that generates a random maze and then solves it in real time using a animated GUI window.

## What it does

When you run the program, a window opens and you can watch two things happen step by step:
1. **Maze generation** — a random maze is carved out using recursive backtracking, knocking down walls between cells until every cell has been visited
2. **Maze solving** — the solver uses a depth-first search (DFS) to find a path from the top-left entrance to the bottom-right exit, drawing the path in red and backtracking in grey when it hits a dead end

The maze is 12 rows × 16 columns and renders in an 800×600 Tkinter window.

## Usage

```bash
python3 main.py
```

The window opens automatically. Close it when you're done.

## Setup

1. Clone the repo
2. Install dependencies:

```bash
pip install -r requrements.txt
```

3. Run with the usage command above

> **Note:** Tkinter must be available on your system. It comes bundled with most Python installations, but on some Linux distros you may need to install `python3-tk` separately.

## What I learned

- Object-oriented programming with classes (`Maze`, `Cell`, `Window`)
- Recursive algorithms — recursive backtracking for maze generation and DFS for solving
- Drawing graphics with Tkinter (`Canvas`, lines, and animation)
- Using a seeded random number generator for reproducible mazes
- Test-Driven Development with `tests.py`
