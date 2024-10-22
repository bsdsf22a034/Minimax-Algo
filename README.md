# Minimax-Algo 
Purpose: The Minimax algorithm is designed to determine the optimal move for a player assuming that the opponent also plays optimally. It is commonly used in two-player, zero-sum games, where one player's gain is another player's loss.
Key Concepts
Game Tree:

The algorithm constructs a game tree where each node represents a game state, and edges represent possible moves. The root node is the current game state.
Players:

There are two players:
Maximizing Player: Aims to maximize their score (often referred to as "Player X").
Minimizing Player: Aims to minimize the maximizing player's score (often referred to as "Player O").
Utility Values:

Terminal nodes (end states of the game) are assigned utility values:
Win for the maximizing player: +1
Win for the minimizing player: -1
Draw: 0
Recursion:

The algorithm evaluates possible moves recursively:
The maximizing player selects the child node with the highest utility value.
The minimizing player selects the child node with the lowest utility value.
Steps of the Minimax Algorithm
Generate the Game Tree: Create a tree structure of all possible moves and game states.
Evaluate Terminal States: Assign utility values to the terminal nodes.
Backtrack: For each non-terminal node, determine its value based on its children:
If it’s the maximizing player's turn, choose the maximum value from its children.
If it’s the minimizing player's turn, choose the minimum value.
Determine the Best Move: The move leading to the child node with the best value is chosen as the optimal move for the current player.
Example Use Case
Tic-Tac-Toe: Minimax can be applied to determine the best move in Tic-Tac-Toe by evaluating all possible moves, assuming both players play optimally.
Limitations
Computational Complexity: The algorithm can be slow for games with large state spaces due to the exponential growth of the game tree.
Alpha-Beta Pruning: Techniques like Alpha-Beta pruning can optimize Minimax by eliminating branches that do not need to be evaluated, improving efficiency.
