# AI SUDOKU SOLVER
Building a Sudoku Solver with Deep Learning

## Overview:
In this tutorial, we'll create a Sudoku solver using deep learning and image processing techniques. The goal is to build a solver that can handle over 150 Sudoku puzzles per minute.

## Prerequisites:
To follow along, you'll need:

OpenCV
Python (version 3.6.7 used here)
Keras
Scikit-Learn
Jupyter Notebooks
Let's dive in!

### Part 1: Detecting the Sudoku Grid in an Image
We start by preprocessing the image to isolate the Sudoku grid. This involves converting the image to grayscale, applying Gaussian blur, thresholding, and dilation. Then, we find the largest polygon in the image, which corresponds to the Sudoku grid, and crop and warp it to obtain a rectangular grid.

### Part 2: Extracting Numbers from the Sudoku Grid
After obtaining the Sudoku grid, we extract individual cells from it. We then build a convolutional neural network (CNN) to recognize the digits in these cells. The CNN consists of convolutional layers, max-pooling layers, dropout layers to prevent overfitting, and dense layers for classification.

### Part 3: Solving the Sudoku Puzzle
Using backtracking, we solve the Sudoku puzzle represented by the grid of digits. Backtracking is an algorithmic technique that recursively tries different possibilities and backtracks when a constraint is violated. We iterate through the grid, filling empty spaces with valid digits until the puzzle is solved.

## Results:
The Sudoku solver successfully recognizes digits and solves Sudoku puzzles with high accuracy. By combining deep learning and image processing, we've created an efficient Sudoku solver capable of handling puzzles at a rapid pace.
