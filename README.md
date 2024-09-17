# Sudoku Generator Tool

This project is a web-based **Sudoku Generator Tool**, built using HTML, JavaScript, and CSS. It allows users to generate Sudoku puzzles of varying difficulty, copy puzzles and solutions to the clipboard, and paste them into other applications.

## Features

- **Three Difficulty Levels**: Easy, Medium, Hard.
- **Clipboard Functionality**: Copy generated puzzles and solutions as images.
- **Hide or Show Solutions**: Option to hide the solutions.
- **Customizable Puzzle Count**: Generate up to 365 puzzles at a time.
- **User Preferences**: Retain difficulty and puzzle count settings via localStorage.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/JavanXD/sudoku
   cd sudoku
   ```

2. **Open `index.html`** in any web browser to access the Sudoku Generator.

## Usage Instructions

- **Set Difficulty**: Use the dropdown to choose between Easy, Medium, or Hard.
- **Number of Puzzles**: Choose how many puzzles to generate (1 to 365).
- **Copy Puzzles or Solutions**: Click the corresponding buttons to copy them as images.
- **Hide or Show Solutions**: Use the checkbox to hide or display puzzle solutions.

## How It Works

1. **Grid Generation**: The tool generates a valid Sudoku grid using JavaScript.
2. **Puzzle Creation**: Cells are removed based on the chosen difficulty level.
3. **Rendering**: Puzzles and solutions are displayed as HTML tables.
4. **Clipboard Functionality**: The puzzle or solution can be copied as a PNG image.

## Prompt Used to Generate This Project

This project was generated with assistance from **ChatGPT**. Below is the prompt used to create the basic functionality of the Sudoku Generator:

```
"Generate a web-based Sudoku puzzle generator with HTML and JavaScript. Add three difficulty levels: Easy, Medium, and Hard. Allow users to copy the puzzle and its solution to the clipboard as PNG images, ensuring proper formatting with bold borders for 3x3 subgrids. Save user settings (difficulty and puzzle count) using localStorage."
```
