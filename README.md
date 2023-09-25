# Connect_4
This is an AI bot that uses minmax algorithm to find the optimal solutions for the game
Connect 4 is a popular two-player board game where the objective is to be the first to connect four of your colored discs in a row, either horizontally, vertically, or diagonally. In this documentation report, we will discuss the implementation of an AI player for Connect 4 using the Alpha-Beta Pruning algorithm.

1. Alpha-Beta Pruning:
Alpha-Beta Pruning is a search algorithm used in game-playing AI to reduce the number of nodes that need to be evaluated in the game tree. It is an extension of the Minimax algorithm and helps optimize the search process by eliminating unnecessary branches.

2. Connect 4 AI Implementation:
To implement the Connect 4 AI using Alpha-Beta Pruning, we need to define the following components:

a. Game State Representation:
We represent the Connect 4 game state using a 2D array, where each cell can be empty or occupied by a player's disc. We assign values to represent empty cells, player 1's discs, and player 2's discs.

b. Evaluation Function:
The evaluation function assigns a score to each game state, indicating the desirability of that state for the AI player. It considers factors such as the number of connected discs, potential threats, and opportunities for the AI player.

c. Alpha-Beta Pruning Algorithm:
The Alpha-Beta Pruning algorithm is implemented using a recursive function that explores the game tree. It maintains two values, alpha and beta, which represent the best achievable score for the maximizing and minimizing players, respectively. The algorithm prunes branches that are guaranteed to be worse than the current best move.

d. Move Generation:
The AI player generates possible moves by iterating through each column of the game board and checking if it is a valid move. It then evaluates each move using the Alpha-Beta Pruning algorithm and selects the best move based on the evaluation scores.
