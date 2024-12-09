[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/0_yE0bFY)
# Implementing graph theory in minesweeper game

## Introduction on how graph theory is implemented
This game treats each cell in the grid as a "node" in a graph, with connections to its neighboring cells forming the "edges." The grid is designed as a network of interconnected cells, inspired by the mechanics of Minesweeper. Each cell can link to up to eight neighbors—above, below, to the sides, and diagonally—based on simple rules that define these relationships. Bombs are randomly scattered across the grid, and when one is placed in a cell, the surrounding cells update to display how many bombs are nearby. To reveal cells during gameplay, the Breadth-First Search (BFS) algorithm is used. This method efficiently spreads through the network of cells, uncovering all connected, non-bomb areas in one go. It creates a seamless experience, allowing large sections of the grid to be revealed with a single click when no bombs are in the vicinity. The design ensures the game feels intuitive and responsive, delivering smooth gameplay.

## How to run
1. Download live server extension in Visual Studio Code
   ![image](https://github.com/user-attachments/assets/ad14cf94-ab10-4fd1-9259-e989410e618e)
2. Then, on bottom right, press `Go Live` button, then it will appear this way
   ![image](https://github.com/user-attachments/assets/0910e0cd-be66-45e0-b69f-3d2484bcfe55)

## Input and Output
User can do right click to reveal the cells and left click to mark the bombs.

## Summarize
To sum up, the Minesweeper implementation mostly depends on the Breadth-First Search (BFS) algorithm to effectively identify cells that don't contain explosives. O(V + E) is the time complexity, where V is the number of vertices (cells) and E is the number of edges (connections between cells), since the BFS method makes sure each cell is processed only once. This approach handles user interactions, refreshes the grid dynamically, and preserves the game state. It makes use of a number of JavaScript files, such as `controller.js`, `grid.js`, `queue.js`, and `stopwatch.js`, each of which performs a particular task such as game logic, grid creation, queue operations, and stopwatch administration. The style of the gaming interface is handled by the CSS file `index.css`. The BFS technique used to disclose neighboring cells free of explosives is also described in the pseudocode that is given. 
