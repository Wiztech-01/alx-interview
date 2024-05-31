
### 0x05-nqueens
---

# 0x05. N Quueens

`Algorithm` `Python`

![Chess grandmaster-Judit Polgar](https://www.crestbook.com/files/Judit-photo1_602x433.jpg)

The N queens puzzle is the challenge of placing N non-attacking queens on an N×N chessboard. Write a program that solves the N queens problem.

* Usage: `nqueens N`
	* If the user called the program with the wrong number of arguments, print `Usage: nqueens N,` followed by a new line, and exit with the status `1`
* where N must be an integer greater or equal to `4`
	* If N is not an integer, print `N must be a number,` followed by a new line, and exit with the status `1`
	* If N is smaller than `4,` print `N must be at least 4,` followed by a new line, and exit with the status `1`
* The program should print every possible solution to the problem
	* One solution per line
	* Format: see example
	* You don’t have to print the solutions in a specific order
* You are only allowed to import the `sys` module
**Read:** [Queen](https://en.wikipedia.org/wiki/Queen_%28chess%29), [Backtracking](https://en.wikipedia.org/wiki/Backtracking)

```
mily@ubuntu:~/0x08. N Queens$ ./0-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
mily@ubuntu:~/0x08. N Queens$ ./0-nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
mily@ubuntu:~/0x08. N Queens$ 

```




The task focuses on solving the N queens problem, a classic problem in computer science and mathematics. The N queens problem involves placing N non-attacking queens on an N×N chessboard. The main objective is to find all possible arrangements of queens such that no two queens threaten each other (i.e., they are not in the same row, column, or diagonal).

The solution to this problem requires employing backtracking algorithms and recursion. Backtracking is a systematic method for exploring all possible solutions to a problem by trying different choices and backtracking when a solution cannot be completed. Recursion, a programming technique where a function calls itself to solve smaller instances of the same problem, is often used in conjunction with backtracking to explore different paths and choices.

In the provided code, the `n_queens` function recursively searches for all possible solutions to the N queens problem by trying out different column positions for each row while ensuring that no two queens threaten each other. Once a valid solution is found, it is added to a list of solutions.

The importance of this task lies in its application of fundamental concepts in computer science such as backtracking and recursion. Additionally, the N queens problem serves as a benchmark for algorithmic problem-solving skills and is commonly used in interviews and programming competitions. By understanding and implementing solutions to this problem, programmers can enhance their problem-solving abilities and gain insight into more complex algorithmic challenges.

---

### Usage:
---

To use the provided code for solving the N queens problem, follow these steps:

1. **Clone the Repository**: If the code is available in a repository, clone or download the repository to your local machine.

2. **Navigate to the Directory**: Open a terminal or command prompt and navigate to the directory containing the Python script (`nqueens.py` or any other filename).

3. **Run the Script**: Execute the script by running the following command in the terminal:

   ```
   ./nqueens.py N
   ```

   Replace `N` with the size of the chessboard (the number of rows and columns). This is the only required argument.

4. **View Solutions**: After running the script, the terminal will display all possible solutions to the N queens problem for the specified chessboard size. Each solution will be printed in a format that represents the positions of the queens on the chessboard.

5. **Interpret Results**: Analyze the output to understand the valid placements of queens on the chessboard. Each solution represents a configuration where no two queens threaten each other.

6. **Modify the Script (Optional)**: If needed, you can modify the script according to your requirements. However, ensure that you maintain the correct structure and functionality to continue solving the N queens problem effectively.

By following these steps, you can easily use the provided code to solve the N queens problem for different chessboard sizes and analyze the solutions generated.