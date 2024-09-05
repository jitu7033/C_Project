# Sudoku Solver in C

This is a command-line based Sudoku solver written in C. It provides users with the option to either input their own puzzle or solve a pre-defined puzzle. The solver uses a backtracking algorithm to find the solution for the Sudoku puzzle.

## Features

- Solve random or user-input Sudoku puzzles.
- The program verifies if the user's puzzle is solvable.
- Users can solve the puzzle themselves or let the computer solve it.
- Highlights the differences between the user's solution and the computer's solution (if the user attempts to solve it).
- Visual representation of the Sudoku grid with colored output.

## How It Works

1. **Initial Prompt**:
   - Choose whether to enter your own puzzle or to solve a pre-defined random puzzle.
   
2. **Input Mode**:
   - Enter your puzzle where `0` represents an empty cell, and numbers from `1-9` represent filled cells.
   
3. **Solution Mode**:
   - Once the puzzle is valid, the program will either solve it using a backtracking algorithm or allow you to input your solution.

4. **Validation**:
   - If you input a solution, the program will compare it with the computed solution and highlight the mismatches.

## How to Play

1. Clone or download the source code.
2. Compile the code using a C compiler (e.g., GCC).
3. Run the executable and follow the on-screen prompts.

## Compilation

You can compile the program with `gcc`:

```bash  
gcc -c  functionlib.c -o library  
ar rcs lib.a library  
gcc -o run main.c -L. lib.a  

./run  

WELCOME TO SUDOKO SOLVER  

click 1. To enter your own puzzle:  
click Any Key Integer. TO take random puzzle:  
1  

Enter your puzzles, fill zero for empty cells and numbers 1 to 9 for values:  
  

+-------+------+---------+  
| 0 2 0 | 4 5 6 | 7 0 9  |  
| 4 0 6 | 7 8 9 | 1 2 3  |  
| 7 8 9 | 1 2 3 | 4 5 6  |  
|-------+------+---------|  
| 2 0 4 | 3 6 5 | 8 9 7  |  
| 3 6 5 | 0 9 7 | 2 1 4  |  
| 8 0 7 | 2 1 4 | 3 6 0  |  
|-------+------+---------|  
| 5 3 1 | 6 4 2 | 9 7 8  |  
| 6 4 2 | 0 7 8 | 5 0 1  |  
| 9 7 8 | 5 3 0 | 6 4 2  |  
+-------+------+---------+  
...  
  
if you want to input your own solution, Enter 3.  
Or press any other integer to let the computer solve the puzzle.  
3  
  
Enter your answer for each cell: 
+-------+------+---------+  
| 1 2 3 | 4 5 6 | 7 8 9  |  
| 4 5 6 | 7 8 9 | 1 2 3  |  
| 7 8 9 | 1 2 3 | 4 5 6  |  
|-------+------+---------|  
| 2 1 4 | 3 6 5 | 8 9 7  |  
| 3 6 5 | 8 9 7 | 2 1 4  |  
| 8 9 7 | 2 1 4 | 3 6 5  |  
|-------+------+---------|  
| 5 3 1 | 6 4 2 | 9 7 8  |  
| 6 4 2 | 9 7 8 | 5 3 1  |  
| 9 7 8 | 5 3 1 | 6 4 2  |  
+-------+------+---------+ 
...

output 
puzzle are  solved By the  computer  | answer is :


+-------+------+---------+  
| 1 2 3 | 4 5 6 | 7 8 9  |  
| 4 5 6 | 7 8 9 | 1 2 3  |  
| 7 8 9 | 1 2 3 | 4 5 6  |  
|-------+------+---------|  
| 2 1 4 | 3 6 5 | 8 9 7  |  
| 3 6 5 | 8 9 7 | 2 1 4  |  
| 8 9 7 | 2 1 4 | 3 6 5  |  
|-------+------+---------|  
| 5 3 1 | 6 4 2 | 9 7 8  |  
| 6 4 2 | 9 7 8 | 5 3 1  |  
| 9 7 8 | 5 3 1 | 6 4 2  |  


